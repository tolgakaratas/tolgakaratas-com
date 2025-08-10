---
title: "Bölüm 12: Kapsamlı Test Senaryoları Üretimi"
weight: 5
type: docs
summary: "Bir özelliği sadece 'çalışıyor' diye bırakmayın. Bir yapay zeka gibi düşünerek, insan aklının gözden kaçırabileceği tüm olası durumları ve akışları nasıl test edeceğinizi öğrenin."
tags: ["test", "kalite", "otomasyon", "permutative", "recursive"]
---

[Seviye: İleri]

Bir özelliği test etmek, sadece doğru çalıştığını görmek değildir. Aynı zamanda aklınıza gelmeyecek tüm tuhaf ve beklenmedik durumlarda bile "kırılmadığından" emin olmaktır. İnsanlar bu "köşe senaryolarını" (edge cases) gözden kaçırabilir, ancak bir AI agent'e doğru düşünce yapısını öğretirsek, sistematik olarak tüm olasılıkları test edebilir.

### 12.1. Permütatif Test: "Ya şöyle olsaydı?" Kombinatorikleri

Bu yaklaşım, bir özelliğin tüm girdi ve durum kombinasyonlarını test etmektir. "Kullanıcı Girişi (Login)" senaryosu bunun için mükemmel bir örnektir. Bir login ekranı basit görünür, ancak sayısız hata olasılığı barındırır. Bir AI Test Agent'i, bu olasılıkların tamamını sistematik olarak test edebilir.

- **Değişkenleri Belirleme:** Bir kredi onay sistemini test ettiğimizi düşünelim. Manuel olarak test edilmesi imkansız olan binlerce senaryo vardır. Ancak bir AI Test Agent için bu bir kombinasyon problemidir. Sistemin karar mekanizmasını etkileyen temel değişkenleri ve bu değişkenlerin alabileceği durumları bir tablo ile netleştirelim:

| Değişken (Variable)    | Durumlar (States)             | State Sayısı           |
| :--------------------- | :---------------------------- | :--------------------- |
| **Kredi Skoru**        | Düşük, Orta, Yüksek           | 3                      |
| **Gelir Seviyesi**     | Yetersiz, Yeterli, Çok Yüksek | 3                      |
| **Mevcut Borç Durumu** | Var, Yok                      | 2                      |
| **İstenen Kredi Türü** | Tüketici, Konut, Taşıt        | 3                      |
| **Toplam Kombinasyon** |                               | **3 x 3 x 2 x 3 = 54** |

Bu tabloya göre, AI Test Agent'inin, müşterinin reddedilmesi veya onaylanması gereken tam **54 farklı senaryoyu** otomatik olarak oluşturup test etmesi gerekir. Bu, hiçbir insanın manuel olarak yapamayacağı bir titizlik seviyesidir.

### 12.2. Özyinelemeli (Recursive) Test: Domino Taşları Gibi Akışlar

Bu yaklaşım, adımları birbirine bağlı olan karmaşık kullanıcı akışlarını test etmek için kullanılır. Mantık şudur: Bir akışın tamamının doğru çalışması, her bir adımın tek tek doğru çalışmasına VE bir önceki adımdan doğru veriyi alıp bir sonraki adıma doğru veriyi iletmesine bağlıdır.

"ATM'den Para Çekme" akışını düşünelim: `Kartı Oku` -> `PIN Doğrula` -> `Tutar Gir`...

- **Mantık:** AI agent, önce `Kartı Oku` adımını tek başına test eder. Başarılıysa, o adımın çıktısını alıp `PIN Doğrula` adımını test eder. Başarılıysa, onun çıktısıyla `Tutar Gir` adımını test eder... Bu, bir domino taşının bir sonrakini devirmesi gibidir. Eğer bir adım başarısız olursa, akışın o noktada durması ve hatanın tam olarak nerede olduğunun raporlanması beklenir.
- **AI Test Prompt (Örnek Prosedür):**
  "**Hedef:** Yetersiz bakiye durumunda akışın sonlandırılmasını test et.
  **Adım 1:** Müşteri bakiyesini 100 TL olarak ayarla.
  **Adım 2:** `PIN Doğrula` adımına kadar olan akışı başarılı olarak çalıştır.
  **Adım 3:** `Tutar Gir` adımında `150 TL` değerini gir.
  **Adım 4:** Sistemin 'Yetersiz Bakiye' mesajı verdiğini VE bir sonraki adıma geçmediğini doğrula."

{{% callout note %}}
**Bu Bölümden Akılda Kalanlar**

- **Permütatif Test,** bir özelliğin "tüm olası durum kombinasyonlarına" karşı ne kadar sağlam olduğunu ölçer.
- **Özyinelemeli Test,** adımları birbirine bağlı bir "akışın" baştan sona tutarlı ve doğru çalışıp çalışmadığını ölçer.
- Bu iki ileri seviye düşünce yapısı, AI test agent'lerine insan sezgisinin ötesinde bir kapsama alanı sağlar.
  {{% /callout %}}

{{% callout note %}}
**Sıra Sizde! (Düşünce Egzersizi)**

Bir e-ticaret sitesindeki "Sepete Ekle" düğmesini düşünün. Bu düğme için test edilebilecek permütatif durumlar neler olabilir? (İpuçları: Ürünün stok durumu, kullanıcının üye olup olmaması, sepette kupon olup olmaması...)
{{% /callout %}}
