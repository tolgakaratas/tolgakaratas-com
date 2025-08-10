---
title: "Bölüm 14: İleri Seviye Konular ve Sınırları Zorlamak"
weight: 1
type: docs
summary: "EARS'ı temel fonksiyonların ötesine taşıyın. Performans ve güvenlik gibi kritik ama soyut konuları EARS ile nasıl somut ve test edilebilir kurallara dönüştüreceğinizi öğrenin."
tags: ["NFR", "güvenlik", "performans", "sürüm kontrolü"]
---

[Seviye: İleri]

Tebrikler! Buraya kadar geldiyseniz, artık EARS'ın temel mantığını ve uygulama alanlarını çok iyi biliyorsunuz demektir. Şimdi, bu bilgiyi biraz daha zorlayıcı ve özel alanlarda nasıl kullanabileceğimize bakalım.

### 14.1. Fonksiyonel Olmayan Gereksinimler (NFRs) ve EARS

Bazen bir sistemin ne yaptığı kadar, o işi "nasıl" yaptığı da önemlidir. Hız, güvenlik, kapasite gibi konulara Fonksiyonel Olmayan Gereksinimler (Non-Functional Requirements) deriz. EARS, normalde fonksiyonel gereksinimler için tasarlanmış olsa da, küçük bir yaratıcılıkla NFR'leri de netleştirebiliriz.

- **Belirsiz NFR:** "Sistem güvenli olmalıdır."
- **EARS ile Netleştirilmiş NFR:** `Eğer bir kullanıcı 15 dakika boyunca hiçbir işlem yapmazsa, o zaman Kullanıcı Yönetim Sistemi, kullanıcının oturumunu otomatik olarak sonlandıracaktır.` (Güvenlik)

- **Belirsiz NFR:** "Arama fonksiyonu hızlı çalışmalıdır."
- **EARS ile Netleştirilmiş NFR:** `Kullanıcı bir arama yaptığında ve veritabanında 1 milyondan az kayıt varken, Arama Motoru, sonuçları 2 saniyeden az sürede listeleyecektir.` (Performans)

### 14.2. Değişen Gereksinimleri Yönetmek

Projeler yaşayan organizmalardır ve gereksinimler zamanla değişebilir. Önemli olan bu değişimi kontrolsüz bir kaosa değil, yönetilen bir sürece dönüştürmektir.

- **Sürümleme (Versioning):** Her gereksinime bir kimlik (ID) ve sürüm numarası verin. Örneğin `REQ-CM-042-v1.0`. Eğer bir değişiklik gerekirse, `REQ-CM-042-v1.1` olarak güncelleyin ve değişikliğin ne olduğunu not edin.
- **Geçersiz Kılma (Deprecation):** Bir gereksinim artık geçerli değilse onu silmek yerine, durumunu `GEÇERSİZ` olarak işaretleyin. Bu, projenin tarihçesini ve alınan kararların nedenlerini anlamak için önemlidir.
- **Yerine Geçme (Superseding):** Eğer yeni bir gereksinim, eskisinin yerini alıyorsa, bunu belirtin. Örneğin: `REQ-CM-042-v1.1 (Durum: GEÇERSİZ, Yerine Geçen: REQ-CM-095-v1.0)`.

Bu basit kurallar, projeniz büyüdükçe ve değiştikçe, herkesin aynı ve en güncel bilgiyle çalışmasını sağlar.

{{% callout note %}}
**Bu Bölümden Akılda Kalanlar**

- EARS, Fonksiyonel Olmayan Gereksinimleri (NFR) ölçülebilir ve test edilebilir hale getirmek için de kullanılabilir.
- Gereksinimleri bir kimlik ve sürüm numarasıyla yönetmek, proje büyüdükçe yaşanacak kaosu engeller.
  {{% /callout %}}

{{% callout note %}}
**Sıra Sizde! (Düşünce Egzersizi)**

"Uygulama, çok sayıda kullanıcıyı desteklemelidir" şeklindeki belirsiz bir "ölçeklenebilirlik" NFR'sini, EARS formatında ölçülebilir bir gereksinime dönüştürmeyi deneyin.
{{% /callout %}}
