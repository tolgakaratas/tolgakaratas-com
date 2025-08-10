---
title: "Bölüm 10: EARS ve Agile: User Story'leri Güçlendirmek"
weight: 3
type: docs
summary: "EARS, Agile ve Scrum süreçlerinin yerine geçmez, onları daha da güçlendirir. Belirsiz 'Kabul Kriterlerini' nasıl çelik gibi sağlam ve test edilebilir kurallara dönüştüreceğinizi öğrenin."
tags: ["agile", "scrum", "user story", "acceptance criteria"]
---

[Seviye: Orta]

"Scrum", "User Story", "Acceptance Criteria"... Eğer yazılım dünyasındaysanız, bu kelimeleri her gün duyarsınız. Peki, EARS bu çevik (Agile) dünyanın neresinde duruyor? Cevap: Tam kalbinde! EARS, belirsiz User Story'leri ve zayıf Kabul Kriterlerini (Acceptance Criteria), adeta bir süper güce dönüştürür.

### 10.1. User Story Nedir?

Bir User Story, bir özelliğin kimin için, ne amaçla ve neden istendiğini anlatan kısa bir ifadedir:

> **"Bir [Kullanıcı Tipi] olarak, [bir eylem yapmak] istiyorum, böylece [bir fayda elde edebilirim]."**

### 10.2. Zayıf Kabul Kriterleri Problemi

Problem, bu hikayenin "ne zaman tamamlanmış sayılacağını" belirleyen kabul kriterlerinde başlar.

- **User Story:** `"Bir e-ticaret sitesi müşterisi olarak, arama sonuçlarını fiyata göre sıralayabilmek istiyorum, böylece bütçeme en uygun ürünleri bulabilirim."`
- **Zayıf Kabul Kriterleri:**
  - Fiyata göre sıralama çalışmalı.
  - Artan ve azalan sıralama olmalı.

Bu kriterler belirsizdir. "Çalışmalı" ne demek? AI agent bu işi nasıl test edecek?

### 10.3. EARS ile Güçlendirilmiş Kabul Kriterleri

Şimdi aynı kabul kriterlerini EARS ile yazalım:

- **EARS ile Güçlendirilmiş Kabul Kriterleri:**
  - **AC1:** `Kullanıcı 'fiyata göre sırala: artan' seçeneğini seçtiğinde, Arama Sonuçları Sistemi, ürünleri en düşük fiyattan en yükseğe doğru listeleyecektir.`
  - **AC2:** `Kullanıcı 'fiyata göre sırala: azalan' seçeneğini seçtiğinde, Arama Sonuçları Sistemi, ürünleri en yüksek fiyattan en düşüğe doğru listeleyecektir.`
  - **AC3 (Negatif Senaryo):** `Eğer arama sonuçlarında fiyat bilgisi olmayan bir ürün varsa, o zaman Arama Sonuçları Sistemi, bu ürünü sıralamanın en sonunda gösterecektir.`

{{% callout note %}}
**Farkı Gördünüz mü?**

Artık elimizde bir AI agent'in (veya bir test mühendisinin) alıp, adım adım test edebileceği, atomik ve sorgulanamaz kurallar var. Belirsizlik ortadan kalktı.
{{% /callout %}}

{{% callout note %}}
**Bu Bölümden Akılda Kalanlar**

- EARS, Agile ve Scrum süreçlerini ortadan kaldırmaz, tam aksine onları daha verimli hale getirir.
- User Story'lerinizin Kabul Kriterlerini EARS formatında yazmak, belirsizliği ortadan kaldırır ve test edilebilirliği en üst düzeye çıkarır.
- Her kabul kriteri, net bir tetikleyici, sistem ve tepkiden oluşmalıdır.
  {{% /callout %}}

{{% callout note %}}
**Sıra Sizde! (Pratik Alıştırma)**

- **User Story:** `"Bir blog yazarı olarak, yazdığım bir taslağı daha sonra yayınlamak üzere kaydedebilmek istiyorum, böylece yazımı hemen yayınlamak zorunda kalmam."`
- Bu User Story için en az iki tane, EARS formatında yazılmış Kabul Kriteri yazın.
  {{% /callout %}}
