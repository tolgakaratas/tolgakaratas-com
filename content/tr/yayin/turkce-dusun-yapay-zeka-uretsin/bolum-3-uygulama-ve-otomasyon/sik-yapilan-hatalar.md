---
title: "Bölüm 9: Sık Yapılan Hatalar (Negatif Örnek Kütüphanesi)"
weight: 2
type: docs
summary: "En iyi öğrenme yollarından biri de hataları incelemektir. Bu bölümde, bir yapay zekayı eğitirken ona ne yapmaması gerektiğini de öğreten bir 'anti-pattern' kütüphanesi oluşturuyoruz."
tags: ["anti-pattern", "hatalar", "kalite", "doğrulama"]
---

[Seviye: Orta]

En iyi öğrenme yollarından biri de başkalarının (ve kendimizin) yaptığı hataları incelemektir. Bu bölüm, bir yapay zeka agent'ini eğitirken ona sadece ne yapacağını değil, aynı zamanda ne yapmaması gerektiğini de öğreten bir "anti-pattern" kütüphanesi gibidir.

### Anti-Pattern 1: Belirsiz Fiil Kullanımı

- **Açıklama:** Sistemin ne yapacağını net olarak belirtmeyen, genel geçer fiiller kullanmak. Bu, AI için en yaygın kafa karışıklığı kaynağıdır.
- **Hatalı Örnek (Negatif):** `Sistem, kullanıcı bilgilerini **yönetecektir**.`
- **Doğru Örnek (Pozitif):** `Sistem, yeni kullanıcı bilgilerini veritabanına **kaydedecektir**.`
- **Neden Hatalı?:** "Yönetmek" fiili; kaydetmek, silmek, güncellemek, okumak gibi onlarca farklı anlama gelebilir. AI, bunlardan hangisini yapacağını bilemez.

### Anti-Pattern 2: Tasarımı Gereksinim Olarak Yazmak

- **Açıklama:** Sistemin ne yapması gerektiğini ("WHAT") söylemek yerine, bunu nasıl yapacağını ("HOW") anlatmaktır. Bu, gereksiz kısıtlamalara ve daha iyi çözümlerin gözden kaçmasına neden olur.
- **Hatalı Örnek (Negatif):** `Kullanıcı bir kategori seçtiğinde, ekranda bir **açılır menü (dropdown menu)** belirecektir.`
- **Doğru Örnek (Pozitif):** `Kullanıcı bir ana kategori seçtiğinde, sistem ilgili alt kategorileri **listeleyecektir**.`
- **Neden Hatalı?:** Belki de açılır menü, o arayüz için en iyi çözüm değildir. Belki de yan tarafta açılan bir panel veya tıklanabilir kutucuklar daha kullanışlı olacaktır. İkinci gereksinim, çözüme ("nasıl") değil, probleme ("ne") odaklanarak mühendise (veya AI'a) en iyi çözümü bulma esnekliği tanır.

### Anti-Pattern 3: Birden Fazla İşi Birleştirmek (Atomik Olmamak)

- **Açıklama:** Altın Kural'ın ihlalidir. Tek bir gereksinim cümlesine birden fazla sistemin veya birden fazla eylemin sığdırılmasıdır. Bu, test etmeyi ve hata ayıklamayı imkansız hale getirir.
- **Hatalı Örnek (Negatif):** `Sipariş onaylandığında, Envanter Sistemi stoğu düşecek ve E-posta Servisi müşteriye onay e-postası gönderecektir.`
- **Doğru Örnek (Pozitif):**
  1.  `Sipariş onaylandığında, Sipariş Yönetim Sistemi, Envanter Sistemine 'stoğu düşür' komutu gönderecektir.`
  2.  `'Stoğu düşür' komutu alındığında, Envanter Sistemi, ilgili ürünün stoğunu bir adet azaltacaktır.`
  3.  `Sipariş onaylandığında, Sipariş Yönetim Sistemi, E-posta Servisine 'onay e-postası gönder' komutu gönderecektir.`
- **Neden Hatalı?:** Eğer e-posta gönderilemez ama stok düşülürse ne olur? Hatalı örnekte bu durum belirsizdir. Doğru örnekte ise her bir adım ayrı bir gereksinim olduğu için her birinin başarı ve hata durumu ayrıca yönetilebilir.

{{% callout note %}}
**Bu Bölümden Akılda Kalanlar**

- Her zaman net, tek bir anlama gelen, eyleme dönük fiiller kullanın.
- "Ne" yapılması gerektiğine odaklanın, "nasıl" yapılacağına değil. Çözümü mühendislere bırakın.
- Bir gereksinim, sadece tek bir iş yapmalıdır. Atomik ve test edilebilir olmalıdır.
  {{% /callout %}}

{{% callout note %}}
**Sıra Sizde! (Pratik Alıştırma)**

Aşağıdaki hatalı gereksinimi, öğrendiğiniz anti-pattern'leri kullanarak düzeltin: `"Sistem, kullanıcının profilini güncellemek için bir form göstermeli ve değişiklikleri hızlıca kaydetmelidir."`
{{% /callout %}}
