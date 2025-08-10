---
title: "Bölüm 6: Pozitif Senaryolar: İstenen Davranışları Kodlamak"
weight: 2
type: docs
summary: "Her şeyin yolunda gittiği 'güneşli gün' senaryoları. Bir sistemin normal çalışma koşulları altında ne yapması gerektiğini tanımlayan temel EARS kalıplarını öğrenin."
tags: ["EARS", "kalıplar", "pozitif senaryo", "when", "while"]
---
[Seviye: Orta]

Her şeyin yolunda gittiği "güneşli gün" senaryolarına hoş geldiniz! Bu bölümde, bir sistemin normal çalışma koşulları altında ne yapması gerektiğini tanımlayan EARS kalıplarını öğreneceğiz.

### 6.1. Sürekli Gereksinimler (Ubiquitous)
* **Açıklama:** Bunlar, sistemin bir koşula veya olaya bağlı olmaksızın, her zaman, adeta nefes almak gibi yapması gereken şeylerdir. Genellikle sistemin temel durumunu veya sürekli bir görevini tanımlarlar.
* **Kalıp ve Sözdizimi (Pattern & Syntax):**
    * **TR:** `SİSTEM_ADI, [Sistem Tepkisi]'ni sağlayacaktır.`
    * **EN:** `The SYSTEM_NAME shall [System Response].`
* **Örnekler:**
    * **Akıllı Kahve Makinesi:** `Akıllı Kahve Makinesi, Wi-Fi ağına bağlı kalacaktır.`
    * **Endüstriyel Su Pompası:** `Endüstriyel Su Pompası, mevcut su basıncını her saniye ölçecektir.`

### 6.2. Durum Odaklı Gereksinimler (State-Driven)
* **Açıklama:** Sistemin belirli bir "modda" veya "durumda" olduğu sürece geçerli olan kurallardır. Durum sona erdiğinde, bu kural da geçerliliğini yitirir.
* **Kalıp ve Sözdizimi:**
    * **TR:** `[Durum] boyunca, SİSTEM_ADI, [Sistem Tepkisi]'ni sağlayacaktır.`
    * **EN:** `While [State], the SYSTEM_NAME shall [System Response].`
* **Örnekler:**
    * **Akıllı Kahve Makinesi:** `'Temizlik modu' aktifken, Akıllı Kahve Makinesi, demleme fonksiyonunu devre dışı bırakacaktır.`
    * **Endüstriyel Su Pompası:** `Motor çalıştığı sürece, Endüstriyel Su Pompası, soğutma fanını aktif tutacaktır.`

### 6.3. Olay Odaklı Gereksinimler (Event-Driven)
* **Açıklama:** Belirli bir olay meydana geldiği anda sistemin vermesi gereken anlık tepkilerdir. "Biri kapıyı çaldığında kapıyı açmak" gibi düşünebilirsiniz.
* **Kalıp ve Sözdizimi:**
    * **TR:** `[Olay] olduğunda, SİSTEM_ADI, [Sistem Tepkisi]'ni sağlayacaktır.`
    * **EN:** `When [Event], the SYSTEM_NAME shall [System Response].`
* **Örnekler:**
    * **Akıllı Kahve Makinesi:** `Kullanıcı 'favorilerime ekle' düğmesine bastığında, Akıllı Kahve Makinesi, mevcut kahve ayarlarını kullanıcının profiline kaydedecektir.`
    * **Endüstriyel Su Pompası:** `Acil durdurma düğmesine basıldığında, Endüstriyel Su Pompası, motor gücünü derhal kesecektir.`

{{% callout note %}}
**Bu Bölümden Akılda Kalanlar**

* "Güneşli gün" senaryoları, sistemin normal ve beklenen davranışlarını tanımlar.
* `Ubiquitous` kalıbı "her zaman" olan şeyler içindir.
* `While` kalıbı, belirli bir "durum boyunca" olan şeyler içindir.
* `When` kalıbı, tek bir "olay olduğunda" verilen tepkiler içindir.
{{% /callout %}}

{{% callout note "Sıra Sizde! (Pratik Alıştırma)" %}}
Bir müzik çalar uygulamasını düşünün. "Kullanıcı bir şarkıyı beğenmek için 'kalp' ikonuna bastığında ne olur?" durumunu Olay Odaklı (Event-Driven) bir EARS gereksinimi olarak yazın.
{{% /callout %}}