---
title: "Bölüm 13: İnsan ve Makine İşbirliği: Testte Sınırları Belirlemek"
weight: 6
type: docs
summary: "Yapay zeka her şeyi yapabilir mi? Cevap: Hayır. Bu bölümde, hangi görevlerin mutlaka insanda kalması gerektiğini ve bir yöneticinin asla yapay zekaya devretmemesi gereken kritik onay noktalarını öğrenin."
tags: ["işbirliği", "insan-AI", "strateji", "onay süreci", "UX"]
---

[Seviye: İleri]

Yapay zeka ne kadar gelişirse gelişsin, bazı şeyler hala (ve belki de her zaman) insana özgü kalacaktır. Harika bir mühendislik süreci, makinenin hızını ve titizliğini, insanın bilgeliği ve sezgisiyle birleştirmektir. Peki, test sürecinde hangi görevleri AI'a devretmeli, hangilerini mutlaka kendimiz yapmalıyız?

### 13.1. Mutlaka İnsana Bırakılması Gereken Testler

{{% callout warning %}}
**Anlatıcıdan Bir Not**

Kariyerim boyunca yüzlerce projede görev aldım; siber güvenlikten akıllı şehirlere, finanstan savunma sanayine kadar. Gördüğüm en büyük hata, teknolojiye körü körüne güvenmektir. Unutmayın, en akıllı yapay zeka bile bir makinedir. Empati kuramaz, estetikten anlamaz ve etik bir pusulası yoktur. Bu görevler her zaman biz insanlara aittir.
{{% /callout %}}

- **Kullanıcı Deneyimi (UX) ve Estetik:** Bir AI, bir düğmenin çalıştığını test edebilir, ama o düğmenin renginin kullanıcıyı rahatsız edip etmediğini, animasyonunun "tatmin edici" bir his verip vermediğini veya uygulamanın genel akışının "sezgisel" olup olmadığını anlayamaz. Bu, empati ve estetik algısı gerektirir.
- **Keşifsel Test (Exploratory Testing):** AI, kendisine verilen senaryoları mükemmel bir şekilde uygular. Ama bir insan, bir "yaramaz çocuk" gibi davranarak, "Acaba şuraya 1 milyon kere tıklasam ne olur?" veya "Formu gönderirken interneti çeksem ne patlar?" gibi, hiçbir senaryoda yazmayan ama gerçek hayatta olabilecek tuhaf hataları bulabilir.
- **Stratejik ve Etik Uygunluk:** Bir AI, bir özelliğin para kazandırıp kazandırmadığını ölçebilir, ama o özelliğin kullanıcıları kandırıp kandırmadığını veya markanın imajına zarar verip vermediğini değerlendiremez. Bu, insani değerler ve iş stratejisi gerektiren bir karardır.

### 13.2. Yöneticinin "Onay" Vermesi Gereken Kritik Aşamalar

Bir AI yüzlerce testi otomatik yapabilir, ancak sorumluluk her zaman insandadır. İşte bir yöneticinin asla AI'a devretmemesi gereken onay noktaları:

1.  **Test Stratejisinin Onayı:** Projenin başında, "Hangi riskler bizim için daha önemli? 144 login senaryosunun hepsini mi test edelim, yoksa en kritik 25 tanesi yeterli mi?" Bu, kaynak ve risk yönetimi kararıdır.
2.  **Kullanıcı Kabul Testi (UAT) Onayı:** Tüm otomatik testler yeşil yansa bile, en sonunda bir insan (genellikle ürün sahibi veya müşteri), "Evet, bu özellik tam olarak benim istediğim şeyi yapıyor ve işime değer katıyor" demelidir.
3.  **Kritik Hata Değerlendirmesi (Triage):** AI kritik bir hata bulduğunda, bu hatanın ne kadar acil olduğu ("hemen şimdi mi düzeltilmeli, yoksa bir sonraki sürümde mi?") kararını bir insan vermelidir.
4.  **Sürüm Onayı (Release):** Tüm testler bittiğinde, ürünün müşteriye sunulmaya hazır olduğuna dair nihai "EVET" veya "HAYIR" kararını vermek. Bu, tüm risklerin tartıldığı bir iş kararıdır.

{{% callout note %}}
**Bu Bölümden Akılda Kalanlar**

- AI, hız ve tekrar gerektiren, mantıksal ve sistematik testlerde mükemmeldir.
- İnsan, empati, yaratıcılık, strateji ve etik gerektiren testlerde vazgeçilmezdir.
- Başarılı bir proje, AI'ı bir "süper güçlü stajyer" gibi kullanır, ancak nihai kararları ve sorumluluğu her zaman tecrübeli insanlara bırakır.
  {{% /callout %}}

{{% callout note %}}
**Sıra Sizde! (Düşünce Egzersizi)**

Geliştirdiğiniz bir mobil oyunu düşünün. Hangi testleri (örneğin, "karakterin zıplama mesafesi") bir AI'a yaptırırdınız? Hangi testleri (örneğin, "oyunun eğlenceli olup olmadığı") mutlaka bir insana yaptırırdınız?
{{% /callout %}}
