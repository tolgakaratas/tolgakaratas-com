---
title: "Bölüm 7: Negatif Senaryolar: Hata Durumlarını Yönetmek"
weight: 3
type: docs
summary: "İşler ters gittiğinde ne olacağını planlamak, sağlam sistemler yaratmanın sırrıdır. Bu 'yağmurlu gün' senaryolarını EARS'ın 'If... Then...' kalıbıyla nasıl yöneteceğinizi öğrenin."
tags: ["EARS", "kalıplar", "negatif senaryo", "hata yönetimi", "if-then"]
---

[Seviye: Orta]

Mühendisliğin en önemli kısımlarından biri, işler ters gittiğinde ne olacağını planlamaktır. Bu "yağmurlu gün" senaryoları, bir sistemi sadece "çalışan" bir sistem olmaktan çıkarıp, "sağlam ve güvenilir" (robust) bir sistem haline getirir.

### 7.1. Hata Yönetiminin Anahtarı: `If... Then...` Kalıbı

- **Açıklama:** EARS, beklenmedik veya istenmeyen durumları ele almak için çok basit ve güçlü bir kalıp sunar. Bu kalıp, bir sorun (eğer) tespit edildiğinde sistemin ne gibi bir düzeltici eylem (o zaman) yapacağını net bir şekilde tanımlar.
- **Kalıp ve Sözdizimi:**
  - **TR:** `Eğer [İstenmeyen Durum], o zaman SİSTEM_ADI, [Sistem Tepkisi]'ni sağlayacaktır.`
  - **EN:** `If [Undesired Condition], then the SYSTEM_NAME shall [System Response].`

### 7.2. Yaygın Hata Türleri ve EARS ile Çözümleri

- **Hatalı Kullanıcı Girdileri:** Kullanıcıların her zaman beklediğimiz gibi davranmayacağını varsaymalıyız.

  - **Örnek (Akıllı Kahve Makinesi):** `Eğer kullanıcı demlemek için gereken miktardan daha az kahve çekirdeği koyarsa, o zaman Akıllı Kahve Makinesi, 'Lütfen çekirdek ekleyin' uyarısını gösterecektir.`
  - **Örnek (Mobil Bankacılık):** `Eğer kullanıcı şifre alanına 8 karakterden daha az bir metin girerse, o zaman Mobil Uygulama, 'Şifreniz en az 8 karakter olmalıdır' mesajını gösterecektir.`

- **Sistem Arızaları veya Kaynak Yetersizlikleri:** Sistemimizin içindeki parçalar da bozulabilir veya kaynakları tükenebilir.

  - **Örnek (Akıllı Kahve Makinesi):** `Eğer su ısıtma ünitesi 5 dakika içinde hedef sıcaklığa ulaşamazsa, o zaman Akıllı Kahve Makinesi, bir arıza kodu gösterecek ve işlemi durduracaktır.`
  - **Örnek (Endüstriyel Su Pompası):** `Eğer pompanın motor sıcaklığı 90 derecenin üzerine çıkarsa, o zaman Pompa Kontrol Sistemi, motoru otomatik olarak durduracak ve bir alarm çalacaktır.`

- **Dış Etkenler ve Bağlantı Sorunları:** Sistemimiz genellikle dış dünyayla iletişim halindedir ve bu iletişim her zaman sorunsuz olmayabilir.
  - **Örnek (Akıllı Kahve Makinesi):** `Eğer Akıllı Kahve Makinesi, hava durumu servisine bağlanamazsa, o zaman makine, 'Hava durumu bilgisi alınamadı' mesajını gösterecektir.`
  - **Örnek (E-ticaret Sitesi):** `Eğer ödeme sistemi bankadan onay alamazsa, o zaman E-ticaret Sitesi, kullanıcıya 'Ödemeniz onaylanmadı, lütfen başka bir kart deneyin' mesajını gösterecektir.`

{{% callout note %}}
**Bu Bölümden Akılda Kalanlar**

- Sağlam sistemler, sadece her şey yolunda gittiğinde ne yapacağını değil, işler ters gittiğinde ne yapacağını da bilir.
- EARS'ın `If... Then...` kalıbı, tüm bu "yağmurlu gün" senaryolarını net bir şekilde tanımlamak için kullanılır.
- Hata durumlarını üç ana kategoride düşünebilirsiniz: Kullanıcı hataları, sistem içi arızalar ve dış dünya sorunları.
  {{% /callout %}}

{{% callout note %}}
**Sıra Sizde! (Pratik Alıştırma)**

Bir online form doldurduğunuzu hayal edin. "Kullanıcı 'zorunlu' olarak işaretlenmiş bir alanı boş bırakıp 'gönder' düğmesine basarsa ne olur?" durumunu `If... Then...` kalıbını kullanarak bir EARS gereksinimi olarak yazın.
{{% /callout %}}
