---
title: "Bölüm 8: Atölye Çalışması: Akıllı Kahve Makinesi Gereksinimlerini Yazmak"
weight: 1
type: docs
summary: "Gerçek bir proje simülasyonu. Müşteriden gelen belirsiz bir e-postayı alıp, adım adım net EARS gereksinimlerine nasıl dönüştüreceğimizi uygulamalı olarak öğrenin."
tags: ["atölye", "vaka analizi", "pratik", "uygulama"]
---

[Seviye: Orta]

Teoriyi öğrendik, şimdi kollarımızı sıvama zamanı! Bu bölümde, sanki bir proje ekibindeymişiz gibi, bize gelen dağınık ve belirsiz bir fikri alıp, adım adım net EARS gereksinimlerine dönüştüreceğiz. Ana kahramanımız, tabii ki, meşhur "Akıllı Kahve Makinemiz".

### 8.1. Proje Başlangıcı: Müşteriden Gelen E-posta

Her şey genellikle şöyle bir e-postayla başlar:

{{% callout note %}}
**Konu: Yeni Kahve Makinesi Projesi**

Merhaba Ekip,

Yeni nesil bir kahve makinesi geliştirmek istiyoruz. Temel beklentimiz, makinenin **kullanıcı dostu** olması ve **harika kahveler** yapması. Kullanıcılar telefonlarından makineyi kontrol edebilmeli. Ayrıca, makinenin ne zaman temizlenmesi gerektiğini bilmesi ve kendi kendine temizlik yapabilmesi **güzel olurdu**. Su ve çekirdek bittiğinde de haberimiz olsun lütfen. **Hızlı çalışması** çok önemli.

Teşekkürler,
Ürün Yönetimi
{{% /callout %}}

Gördüğünüz gibi, bu metin harika fikirlerle dolu ama mühendislik için tam bir kabus. "Kullanıcı dostu", "harika kahve", "hızlı" gibi ifadeler tamamen subjektif. "Güzel olurdu" gibi ifadeler ise bir özelliğin zorunlu mu yoksa opsiyonel mi olduğunu belirsiz bırakıyor.

### 8.2. Adım 1: Hammaddeyi Ayrıştırma (Hedefler ve İhtiyaçlar)

İlk işimiz, bu e-postadaki hedefleri ve gizli ihtiyaçları ayrıştırmak:

- **Hedef 1:** Kullanıcılar mobil uygulama üzerinden kahve yapabilmeli.
- **Hedef 2:** Makine, sarf malzemeleri (su, çekirdek) azaldığında haber vermeli.
- **Hedef 3:** Makinenin bir temizlik fonksiyonu olmalı.
- **İhtiyaç (Hedef 1 için):** Mobil uygulama ile makine arasında bir iletişim protokolü.
- **İhtiyaç (Hedef 2 için):** Su ve çekirdek seviyelerini ölçen sensörler.
- **İhtiyaç (Hedef 3 için):** Kendi kendine temizlik yapabilen bir mekanizma ve su devresi.

### 8.3. Adım 2: EARS ile Netleştirme (Gereksinimleri Yazma)

Şimdi bu ihtiyaçları, öğrendiğimiz EARS kalıplarıyla somut gereksinimlere dönüştürelim:

- **Gereksinim (Hedef 1 için):** `Kullanıcı mobil uygulamadaki 'Sert Kahve Demle' düğmesine bastığında, Akıllı Kahve Makinesi, sert kahve tarifine göre demleme işlemini başlatacaktır.` (Olay Odaklı)
- **Gereksinim (Hedef 2 için):** `Eğer su seviyesi %10'un altına düşerse, o zaman Akıllı Kahve Makinesi, mobil uygulamaya 'su seviyesi kritik' bildirimi gönderecektir.` (Negatif Senaryo)
- **Gereksinim (Hedef 3 için):** `'Otomatik Temizlik' modu aktifken, Akıllı Kahve Makinesi, sıcak su ile iç devreleri temizleyecektir.` (Durum Odaklı)

Bu atölye boyunca, e-postadaki her bir belirsiz ifadeyi bu şekilde onlarca net, test edilebilir ve uygulanabilir gereksinime dönüştüreceğiz.

{{% callout note %}}
**Bu Bölümden Akılda Kalanlar**

- Gerçek dünya projeleri, belirsiz ve dağınık fikirlerle başlar.
- İlk adım, bu fikirleri daha somut hedeflere ve ihtiyaçlara ayrıştırmaktır.
- Son adım ise, bu ihtiyaçları EARS kalıplarını kullanarak herkesin aynı şeyi anladığı, atomik gereksinimlere dönüştürmektir.
  {{% /callout %}}

{{% callout note %}}
**Sıra Sizde! (Pratik Alıştırma)**

Yukarıdaki e-postada yer alan **"Hızlı çalışması çok önemli"** hedefini, ölçülebilir ve test edilebilir bir EARS gereksinimine dönüştürmeyi deneyin. (İpucu: Hangi olaydan sonra ne kadar sürede bir tepki vermeli?)
{{% /callout %}}
