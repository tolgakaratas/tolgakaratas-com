# Tolga Karataş Proje ve Yayın Portföyü Ürün Gereksinimleri Belgesi (PRD)

## Goals and Background Context

### Goals

- Tüm projelerimi tek bir platformda etkili bir şekilde sergilemek.
- Profesyonel geçmişimi potansiyel işverenlere ve işbirlikçilere kapsamlı bir şekilde sunmak.
- Projelerimin detayları ve yayınladığım yazılar hakkında detaylı içerikler paylaşmak.
- Etkinlikleri paylaşmak.
- Hazırladığım projeleri paylaşmak.
- Yaptığım sunumları paylaşmak.
- Kanaat önderi, sektör uzmanı, güvenilir danışman, yetkili otorite imajımı geliştirmek.
    - **Metrik:** Web sitesi trafiğinde %20 artış (ilk 6 ay içinde).
    - **Metrik:** Sosyal medya etkileşiminde %15 artış (ilk 6 ay içinde).
    - **İş Değeri:** Potansiyel işverenler ve işbirlikçiler nezdinde güvenilirliği ve uzmanlığı artırmak.

### Background Context

Mevcut özgeçmiş formatlarımın 30 yıllık geniş ve çeşitli deneyimimi tam olarak yansıtmadığını fark ettim. Bu durum, potansiyel işverenlerin ve işbirlikçilerin deneyimimi tam olarak anlamasını zorlaştırıyor ve fırsatları kaçırmama neden olabiliyor. Bu PRD, bu sorunu çözmek ve deneyimimi daha yapılandırılmış, kapsamlı ve etkileşimli bir formatta sunmak için bir yol haritası görevi görecektir.
### Risks and Assumptions

- **Risk 1 (Çeviri Kalitesi):** Çevirilerin dilbilgisi ve anlam bütünlüğü açısından yetersiz olması, kullanıcı deneyimini olumsuz etkileyebilir.
    - **Azaltma Stratejisi:** Profesyonel çevirmenlerle çalışmak ve yerel konuşmacılar tarafından gözden geçirilmesini sağlamak.
- **Risk 2 (İçerik Oluşturma Süresi):** Detaylı proje ve yayın içeriklerinin oluşturulması beklenenden uzun sürebilir.
    - **Azaltma Stratejisi:** İçerik oluşturma sürecini küçük parçalara bölmek ve düzenli ilerleme takibi yapmak.
- **Varsayım 1 (Bütçe ve Kaynak):** Proje için yeterli bütçe ve insan kaynağının mevcut olduğu varsayılmaktadır.
- **Varsayım 2 (Teknik Altyapı):** Hugo ve ilgili teknolojilerin mevcut hosting ortamında sorunsuz çalışacağı varsayılmaktadır.

### Definition of Success

- Web sitesi lansmanından sonraki ilk 6 ay içinde belirlenen trafik ve sosyal medya etkileşim metriklerine ulaşılması.
- Potansiyel işverenlerden ve işbirlikçilerden olumlu geri bildirimler alınması.
- Projelerin ve yayınların detaylı ve güncel bir şekilde sergilenmesi.

### Change Log

| Date | Version | Description | Author |
| :--- | :------ | :---------- | :----- |
| 2025-06-29 | 1.0     | PRD dökümanı analiz edildi ve güncellenmeye başlandı. | BMAD Master Orchestrator |
## Stakeholder Analysis

- **Tolga Karataş (Ürün Sahibi/Konu Uzmanı):** Projenin vizyonunu belirler, içerik sağlar ve nihai kararları verir.
    - **Beklentiler:** Deneyimini en iyi şekilde yansıtan, profesyonel ve etkili bir platform.
- **Potansiyel İşverenler/İşbirlikçiler (Ana Kullanıcılar):** Tolga'nın yetkinliklerini ve projelerini değerlendirir.
    - **Beklentiler:** Kolay erişilebilir, anlaşılır, detaylı ve güvenilir bilgi.
- **Geliştirme Ekibi (Uygulayıcılar):** Teknik gereksinimleri karşılar ve web sitesini geliştirir.
    - **Beklentiler:** Net gereksinimler, teknik varsayımlar ve kısıtlamalar.
- **Çeviri Ekibi (Destekleyici):** Web sitesi içeriğini farklı dillere çevirir.
    - **Beklentiler:** Tutarlı ve doğru çeviri kılavuzları, yeterli bağlam.
- **DevOps Ekibi (Destekleyici):** CI/CD süreçlerini ve deployment'ı yönetir.
    - **Beklentiler:** Otomatikleştirilebilir, güvenli ve ölçeklenebilir altyapı.

## Requirements

### Functional

- **FR1 (Must-have):** Proje portföyü, Tolga Karataş'ın projelerini, yayınlarını, etkinliklerini ve diğer ilgili içeriklerini sergilemelidir.
- **FR2 (Must-have):** Kullanıcılar, projeler arasında kolayca gezinebilmeli ve her bir projenin detaylı açıklamasına erişebilmelidir.
- **FR3 (Must-have):** Web sitesi, farklı cihazlarda (masaüstü, tablet, mobil) uyumlu bir şekilde görüntülenmelidir.

### Non Functional

- **NFR1 (Must-have):** Web sitesi hızlı yüklenmeli ve yüksek performans göstermelidir. (Hedef: Sayfa yükleme süresi 3 saniyenin altında olmalı)
- **NFR2 (Must-have):** Web sitesi güvenli olmalı ve kullanıcı verilerini korumalıdır. (Hedef: OWASP Top 10 güvenlik açıklarına karşı dayanıklı olmalı)
- **NFR3 (Must-have):** Web sitesi SEO (Arama Motoru Optimizasyonu) için optimize edilmelidir. (Hedef: Google PageSpeed Insights skoru mobil için min. 70, masaüstü için min. 90 olmalı)

### Out of Scope

- İleri düzey kullanıcı etkileşimi (yorumlar, forumlar, kullanıcı kayıtları).
- E-ticaret entegrasyonu veya ödeme sistemleri.
- Dinamik içerik yönetimi (CMS entegrasyonu).

### Future Iterations

- Blog veya makale yazma özelliği.
- İletişim formu veya doğrudan mesajlaşma entegrasyonu.
- Gelişmiş arama ve filtreleme özellikleri.
- Farklı dil seçenekleri (örneğin, Almanca, Fransızca).
## User Interface Design Goals

### Overall UX Vision
Kullanıcı dostu, sezgisel ve etkileyici bir deneyim sunmak.

### Key Interaction Paradigms
- Kolay navigasyon
- Hızlı erişim
- Etkileşimli içerik

### Core Screens and Views
- Ana Sayfa: Kullanıcıya genel bir bakış sunar, öne çıkan projeleri ve son yayınları gösterir.
- Projeler Sayfası: Tüm projelerin listesini ve detaylı proje sayfalarına bağlantıları içerir.
- Yayınlar Sayfası: Tolga Karataş'ın yayınladığı makaleleri ve yazıları listeler.
- Etkinlikler Sayfası: Katıldığı veya düzenlediği etkinlikleri gösterir.
- Hakkında Sayfası: Tolga Karataş'ın özgeçmişi, becerileri ve iletişim bilgilerini içerir.

### Accessibility: { None, WCAG, etc }
WCAG 2.1 AA

### Branding
- Profesyonel
- Güvenilir
- Yenilikçi

### Target Device and Platforms
- Masaüstü
- Tablet
- Mobil

## Business Workflows / User Flows

### Kullanıcı Akışı: Proje Detayını Görüntüleme

1.  **Başlangıç:** Kullanıcı web sitesine erişir.
2.  **Adım 1:** Kullanıcı ana sayfadaki "Projeler" bölümüne gider veya navigasyon menüsünden "Projeler" sayfasına tıklar.
3.  **Adım 2:** Kullanıcı, öne çıkan projeler listesinden veya tüm projeler listesinden ilgilendiği bir projeyi seçer.
4.  **Adım 3:** Kullanıcı seçilen projenin detay sayfasına yönlendirilir.
5.  **Adım 4:** Kullanıcı, projenin amacını, kullanılan teknolojileri, elde edilen sonuçları ve ilgili bağlantıları inceler.
6.  **Bitiş:** Kullanıcı proje detay sayfasını kapatır veya başka bir sayfaya geçer.

### Kullanıcı Akışı: Yayın Detayını Görüntüleme

1.  **Başlangıç:** Kullanıcı web sitesine erişir.
2.  **Adım 1:** Kullanıcı navigasyon menüsünden "Yayınlar" sayfasına tıklar.
3.  **Adım 2:** Kullanıcı, yayınlar listesinden ilgilendiği bir yayını seçer.
4.  **Adım 3:** Kullanıcı seçilen yayının detay sayfasına yönlendirilir.
5.  **Adım 4:** Kullanıcı, yayının amacını, ana konularını ve ilgili bağlantıları inceler.
6.  **Bitiş:** Kullanıcı yayın detay sayfasını kapatır veya başka bir sayfaya geçer.
### User Personas

- **Persona 1: Potansiyel İşveren Ayşe**
    - **Hedef:** Tolga'nın deneyimini ve yetkinliklerini hızlıca anlamak, ilgili projeleri incelemek.
    - **İhtiyaçlar:** Net, özlü bilgiler; kolay navigasyon; somut başarı örnekleri.
- **Persona 2: Akademisyen Mehmet**
    - **Hedef:** Tolga'nın yayınlarını ve akademik çalışmalarını incelemek, ortak ilgi alanları bulmak.
    - **İhtiyaçlar:** Detaylı yayın bilgileri; ilgili makalelere bağlantılar; araştırma alanları hakkında bilgi.
- **Persona 3: İşbirlikçi Can**
    - **Hedef:** Tolga'nın geçmiş projelerini ve teknik yaklaşımlarını anlamak, potansiyel işbirlikleri için fikir edinmek.
    - **İhtiyaçlar:** Proje detayları; kullanılan teknolojiler; kod depolarına erişim (varsa).
## Technical Assumptions

### Repository Structure: { Monorepo, Polyrepo, etc...}
Monorepo

### Service Architecture
Statik site (Hugo)

### Testing requirements
- Birim testleri (Hedef: Kod kapsamı %80)
- Entegrasyon testleri
- Uçtan uca testler

### Additional Technical Assumptions and Requests
- CI/CD pipeline kurulacak.
- Otomatik deployment yapılacak.

### Technology Stack and Versions
- Hugo: v0.120.0 veya üzeri
- Go: 1.21 veya üzeri (Hugo modülleri için)
- JavaScript: ES6+
- CSS Framework: Bootstrap 5 (veya benzeri)

### Coding Standards and Best Practices
- Temiz Kod prensipleri uygulanacaktır.
- Modüler ve yeniden kullanılabilir bileşenler geliştirilecektir.
- Güvenlik açıkları için OWASP Top 10 prensipleri göz önünde bulundurulacaktır.
- Kod incelemeleri (Code Reviews) zorunlu olacaktır.

### Error Handling and Logging
- Uygulama genelinde merkezi hata yakalama mekanizmaları kurulacaktır.
- Kullanıcıya dostu hata mesajları gösterilecektir.
- Sunucu tarafı hatalar için detaylı loglama (log seviyeleri: INFO, WARN, ERROR) yapılacaktır.
- Loglar merkezi bir sistemde (örneğin, ELK Stack) toplanacaktır.

### Dependencies

- Hugo statik site jeneratörü.
- Netlify veya benzeri bir hosting sağlayıcısı.
- GitHub veya benzeri bir versiyon kontrol sistemi.

### Technical Constraints

- Statik site yapısı nedeniyle dinamik kullanıcı etkileşimleri sınırlıdır.
- İçerik güncellemeleri için manuel dosya düzenlemesi gereklidir (CMS entegrasyonu olmadığı sürece).
- Büyük medya dosyaları için harici depolama çözümleri gerekebilir.
## Data Requirements

- **Projeler:**
    - Başlık (Metin)
    - Kısa Özet (Metin)
    - Detaylı Açıklama (Markdown)
    - Kullanılan Teknolojiler (Etiket Dizisi)
    - Canlı Demo Bağlantısı (URL, isteğe bağlı)
    - Kod Deposu Bağlantısı (URL, isteğe bağlı)
    - Öne Çıkan Proje Durumu (Boolean)
- **Yayınlar:**
    - Başlık (Metin)
    - Özet (Metin)
    - Yayın Tarihi (Tarih)
    - Orijinal Yayın Bağlantısı (URL)
    - Ana Konular (Etiket Dizisi)
- **Etkinlikler:**
    - Başlık (Metin)
    - Tarih (Tarih)
    - Konum (Metin)
    - Açıklama (Markdown)
    - İlgili Bağlantı (URL, isteğe bağlı)

## Business Rules

- Ana sayfada en fazla 3 öne çıkan proje gösterilmelidir.
- Yayınlar en yeniden en eskiye doğru sıralanmalıdır.
- Tüm harici bağlantılar yeni bir sekmede açılmalıdır.
- Mobil cihazlarda navigasyon menüsü katlanabilir (hamburger menü) olmalıdır.
## Epics

- Epic1: İçerik zenginleştir
#### Estimated Effort
- M (Orta)

#### Dependencies
- İçerik Ekibi'nin proje detaylarını sağlaması.
- Epic2: Türkçe tercümeleri yap
- Epic3: Rusça tercümeleri yap
- Epic4: İçerik Stratejisi ve Üretimi
- Epic5: "Türkçe Düşün, Yapay Zeka Üretsin" Kitabının Yayınlanması
- Epic6: Kapsamlı İçerik Zenginleştirme ve İmaj Geliştirme
- Epic7: Yeni İçerik Türlerinin Entegrasyonu ve Stratejisi
- Epic8: Çok Dilli İçerik ve Menü Tutarlılığı
- Epic9: "Türkçe Düşün, Yapay Zeka Üretsin" Kitabı Formatının İyileştirilmesi

## Epic 6: Kapsamlı İçerik Zenginleştirme ve İmaj Geliştirme

**Goal:** Tolga Karataş'ın web sitesindeki tüm içeriklerin (projeler, yayınlar, blog yazıları, hakkında sayfaları) PDF'teki detaylarla zenginleştirilmesi, görsel öğelerle desteklenmesi ve imajının en üst düzeye çıkarılması.

### Story 6.1: Yazar Profillerinin ve "Hakkımda" Sayfalarının Detaylandırılması

**As a** site ziyaretçisi,
**I want** Tolga Karataş'ın profesyonel geçmişi ve uzmanlık alanları hakkında PDF'teki detaylarla zenginleştirilmiş, kapsamlı ve etkileyici bilgilere erişebilmek,
**so that** onun yetkinliklerini ve somut başarılarını daha iyi anlayabilirim.

#### Acceptance Criteria (ACs)

1.  **AC6.1.1:** PDF'teki "ÇALIŞMA HAYATI" ve "AKADEMİK KARİYERİ" bölümlerindeki detaylar (UNIDO projesi, 5 ülkedeki yazılım geliştirme ekipleri koordinasyonu, ders verdiği üniversiteler, ders konuları) yazar profillerine ve "Hakkımda" sayfalarına (tüm dillerde) entegre edilmelidir.
2.  **AC6.1.2:** "Araştırmacı İş İnsanı" rolünü destekleyen somut başarılar (örn. ASIDEES projesi) vurgulanmalıdır.
3.  **AC6.1.3:** Kariyer yolculuğunu veya uzmanlık alanlarının gelişimini gösteren basit bir zaman çizelgesi (timeline) veya beceri haritası (skill map) Mermaid ile eklenmelidir.

#### Development Tasks

- [ ] Görev 6.1.1: `content/en/authors/tolga/_index.md`, `content/tr/authors/tolga/_index.md` ve `content/ru/authors/tolga/_index.md` dosyalarını PDF'teki bilgilerle güncelle.
- [ ] Görev 6.1.2: İlgili sayfalara Mermaid ile zaman çizelgesi veya beceri haritası ekle.

#### QA Tasks

- [ ] Test 6.1.1: Güncellenen yazar profillerinin ve "Hakkımda" sayfalarının tüm dillerde PDF'teki bilgileri doğru ve eksiksiz içerdiğini doğrula.
- [ ] Test 6.1.2: Mermaid görsellerinin doğru görüntülendiğini ve bilgiyi desteklediğini doğrula.

### Story 6.2: Proje Sayfalarının Detaylandırılması ve Görselleştirilmesi

**As a** site ziyaretçisi,
**I want** Tolga Karataş'ın projeleri hakkında PDF'teki detaylarla zenginleştirilmiş, somut başarıları vurgulayan ve görsel öğelerle desteklenmiş bilgilere erişebilmek,
**so that** projelerin kapsamını, etkisini ve Tolga Karataş'ın katkılarını daha iyi anlayabilirim.

#### Acceptance Criteria (ACs)

1.  **AC6.2.1:** PDF'teki "TİCARİ FAALİYETLERİ" ve "DEVAM EDEN PROJELERİ" bölümlerindeki bilgilerle mevcut proje açıklamaları zenginleştirilmelidir.
2.  **AC6.2.2:** "Denomas Denetim Otomasyon" yazılımının "ithal ikame ürün olarak sanayi bakanlığı, ticaret odası, üniversite ve teknopark heyetleri tarafından onaylanan, tescil edilen yerli malı belgeli sektördeki ilk ve tek yazılım platformu" olduğu bilgisi gibi somut başarı ve tescil detayları ilgili proje sayfalarına eklenmelidir.
3.  **AC6.2.3:** Her projenin iş akışını, mimarisini veya etki alanını gösteren basit akış şemaları (flowchart) veya bileşen diyagramları (component diagram) Mermaid ile eklenmelidir.

#### Development Tasks

- [ ] Görev 6.2.1: İlgili proje sayfalarını PDF'teki bilgilerle güncelle.
- [ ] Görev 6.2.2: Proje sayfalarına Mermaid diyagramları ekle.

#### QA Tasks

- [ ] Test 6.2.1: Güncellenen proje sayfalarının tüm dillerde PDF'teki bilgileri doğru ve eksiksiz içerdiğini doğrula.
- [ ] Test 6.2.2: Mermaid diyagramlarının doğru görüntülendiğini ve bilgiyi desteklediğini doğrula.

### Story 6.3: Yayın Sayfalarının Zenginleştirilmesi ve Ödüllerin Vurgulanması

**As a** site ziyaretçisi,
**I want** Tolga Karataş'ın yayınları hakkında PDF'teki ödül bilgileriyle zenginleştirilmiş ve görsel öğelerle desteklenmiş bilgilere erişebilmek,
**so that** onun akademik ve profesyonel başarılarını daha iyi anlayabilirim.

#### Acceptance Criteria (ACs)

1.  **AC6.3.1:** PDF'teki "ÖDÜLLERİ" bölümünde yer alan "2017 yılında Kiev'de en iyi blockchain hackathon projesi ödülünü ekibiyle almıştır" bilgisinin ilgili yayın veya proje sayfasına eklenmesi.
2.  **AC6.3.2:** "Görev aldığı güvenlik, akıllı şehircilik ve alt yapı yönetimi projeleri onlarca ödül almıştır" ifadesinin, bu projelerin detay sayfalarında veya ilgili yayınlarda somut örneklerle desteklenmesi.
3.  **AC6.3.3:** Yayınların ana argümanlarını veya metodolojilerini özetleyen zihin haritaları (mind map) veya kavram haritaları (concept map) eklenmesi.

#### Development Tasks

- [ ] Görev 6.3.1: İlgili yayın ve proje sayfalarını PDF'teki ödül bilgileriyle güncelle.
- [ ] Görev 6.3.2: Yayın sayfalarına Mermaid zihin haritaları veya kavram haritaları ekle.

#### QA Tasks

- [ ] Test 6.3.1: Güncellenen yayın sayfalarının tüm dillerde PDF'teki bilgileri doğru ve eksiksiz içerdiğini doğrula.
- [ ] Test 6.3.2: Mermaid görsellerinin doğru görüntülendiğini ve bilgiyi desteklediğini doğrula.

### Story 6.4: İçeriklerin Görsel Öğelerle Zenginleştirilmesi

**As a** site ziyaretçisi,
**I want** web sitesindeki karmaşık teknik konuların görsel öğelerle (Mermaid diyagramları, zihin haritaları vb.) desteklenerek daha anlaşılır hale getirilmesini,
**so that** bilgiyi daha kolay kavrayabilir ve Tolga Karataş'ın uzmanlığını daha net görebilirim.

#### Acceptance Criteria (ACs)

1.  **AC6.4.1:** Karmaşık teknik konuları açıklamak için tüm proje ve yayın sayfalarına akış şemaları, mimari diyagramlar veya süreç adımlarını gösteren görsellerin (Mermaid) yaygınlaştırılması.
2.  **AC6.4.2:** "UZMANLIK ALANLARI" ve "DEVAM EDEN PROJELER" gibi bölümlerdeki kavramları açıklamak için akış şemaları, mimari diyagramlar veya süreç adımlarını gösteren görsellerin kullanılması.

#### Development Tasks

- [ ] Görev 6.4.1: Belirlenen sayfalara uygun Mermaid diyagramları ekle.

#### QA Tasks

- [ ] Test 6.4.1: Eklenen tüm görsellerin doğru görüntülendiğini ve içeriği desteklediğini doğrula.

## Epic 7: Yeni İçerik Türlerinin Entegrasyonu ve Stratejisi

**Goal:** Web sitesine kitaplar, rehberler ve yeni blog serileri gibi yeni içerik türlerinin entegre edilmesi ve bu içeriklerin stratejik olarak konumlandırılması.

### Story 7.1: "Uzmanlık Alanları" Rehber Serilerinin Oluşturulması

**As a** site ziyaretçisi,
**I want** Tolga Karataş'ın uzmanlık alanlarına yönelik (Siber güvenlik, stratejik güvenlik, uluslararası uyum standartları vb.) detaylı rehber serilerine erişebilmek,
**so that** bu konularda derinlemesine bilgi edinebilir ve Tolga Karataş'ın düşünce liderliğini takip edebilirim.

#### Acceptance Criteria (ACs)

1.  **AC7.1.1:** PDF'teki "UZMANLIK ALANLARI" bölümündeki her bir uzmanlık alanı için ayrı bir rehber veya blog serisi oluşturulmalıdır.
2.  **AC7.1.2:** Bu rehberlerin "Guide" formatında yeni sayfalar olarak eklenmesi.

#### Development Tasks

- [ ] Görev 7.1.1: Her uzmanlık alanı için yeni içerik dosyaları (Markdown) oluştur.
- [ ] Görev 7.1.2: Bu içerikleri "Guide" formatına uygun şekilde yapılandır.

#### QA Tasks

- [ ] Test 7.1.1: Oluşturulan rehber serilerinin doğru görüntülendiğini ve içeriğin tutarlı olduğunu doğrula.

### Story 7.2: Devam Eden Projeler İçin Yeni Sayfaların Oluşturulması

**As a** site ziyaretçisi,
**I want** Tolga Karataş'ın devam eden projeleri hakkında bilgi edinebilmek,
**so that** onun güncel çalışmalarını takip edebilir ve potansiyel işbirlikleri için fikir edinebilirim.

#### Acceptance Criteria (ACs)

1.  **AC7.2.1:** PDF'te belirtilen "Yönetim Otomasyon Yazılımları", "Güvenlik Otomasyon Yazılımları", "Veri Analiz Yazılımları", "Finansal Risk Analiz Yazılımları" gibi devam eden projeler için ayrı proje sayfaları oluşturulmalıdır.
2.  **AC7.2.2:** Bu sayfaların mevcut projeler gibi detaylandırılması.

#### Development Tasks

- [ ] Görev 7.2.1: Her devam eden proje için yeni içerik dosyaları (Markdown) oluştur.
- [ ] Görev 7.2.2: Bu içerikleri mevcut proje şablonlarına uygun şekilde detaylandır.

#### QA Tasks

- [ ] Test 7.2.1: Oluşturulan devam eden proje sayfalarının doğru görüntülendiğini ve içeriğin tutarlı olduğunu doğrula.

## Epic 8: Çok Dilli İçerik ve Menü Tutarlılığı

**Goal:** Web sitesindeki tüm içeriklerin ve menülerin üç dilde (Türkçe, İngilizce, Rusça) tam ve tutarlı çevirilerinin sağlanması.

### Story 8.1: Tüm İçeriklerin Detaylı ve Tutarlı Çevirilerinin Sağlanması

**As a** site ziyaretçisi,
**I want** web sitesindeki tüm içerikleri (projeler, yayınlar, blog yazıları, hakkında sayfaları) kendi dilimde (Türkçe, İngilizce, Rusça) tam ve detaylı olarak okuyabilmek,
**so that** bilgiyi eksiksiz ve doğru bir şekilde anlayabilirim.

#### Acceptance Criteria (ACs)

1.  **AC8.1.1:** PDF'teki tüm bilgilerin (özellikle "Hakkımda" ve proje/yayın detayları) her üç dilde de tam ve eksiksiz olarak yer aldığından emin olunması.
2.  **AC8.1.2:** Çevirilerin sadece kelime bazında değil, anlam ve bağlam açısından da tutarlı olması.

#### Development Tasks

- [ ] Görev 8.1.1: Tüm mevcut içerik dosyalarını (projeler, yayınlar, blog yazıları, yazar profilleri) üç dildeki çevirilerini kontrol et ve eksik/hatalı kısımları tamamla.

#### QA Tasks

- [ ] Test 8.1.1: Tüm dillerdeki içeriklerin detay ve kapsam açısından tutarlı olduğunu doğrula.
- [ ] Test 8.1.2: Çevirilerin dilbilgisi ve anlam bütünlüğü açısından kalitesini doğrula.

### Story 8.2: Çok Dilli Menü Çevirilerinin Kontrolü ve Düzeltilmesi

**As a** site ziyaretçisi,
**I want** web sitesindeki menülerin kendi dilimde (Türkçe, İngilizce, Rusça) doğru ve tutarlı bir şekilde görüntülenmesini,
**so that** sitede kolayca gezinebilirim.

#### Acceptance Criteria (ACs)

1.  **AC8.2.1:** `config/_default/menus.yaml` ve diğer dil-spesifik menü yapılandırmalarının kontrol edilmesi.
2.  **AC8.2.2:** Türkçe ve Rusça menü çevirilerinin düzgün olduğunun doğrulanması ve gerekli düzeltmelerin yapılması.

#### Development Tasks

- [ ] Görev 8.2.1: `config/_default/menus.yaml` ve ilgili dil dosyalarını incele.
- [ ] Görev 8.2.2: Menü çevirilerindeki hataları düzelt.

#### QA Tasks

- [ ] Test 8.2.1: Tüm dillerdeki menülerin doğru görüntülendiğini ve navigasyonun sorunsuz çalıştığını doğrula.

## Epic 9: "Türkçe Düşün, Yapay Zeka Üretsin" Kitabı Formatının İyileştirilmesi

**Goal:** `content/en/publication/turkce-kodlama` altındaki sayfaların Hugo Blox'un "docs" (kitap) formatına uygun hale getirilerek okunaklılığının ve yerleşimlerinin iyileştirilmesi.

### Story 9.1: `turkce-kodlama` Sayfalarının `type: docs` Formatına Dönüştürülmesi

**As a** site ziyaretçisi,
**I want** "Türkçe Düşün, Yapay Zeka Üretsin" kitabını web sitesinde kitap formatında (sol menüde bölümler, sayfa içi navigasyon vb.) kolayca okuyabilmek,
**so that** içeriği daha düzenli ve kullanıcı dostu bir şekilde takip edebilirim.

#### Acceptance Criteria (ACs)

1.  **AC9.1.1:** `content/en/publication/turkce-kodlama` altındaki tüm `index.md` dosyalarının `frontmatter`'ına `type: docs` eklenmesi.
2.  **AC9.1.2:** Gerekirse sayfaların yeniden düzenlenmesi veya taşınması (örneğin, `_index.md` ve bölüm klasörleri).
3.  **AC9.1.3:** Hugo Blox'un "docs" özelliğinin tüm yeteneklerinin (sol menüde bölüm navigasyonu, önceki/sonraki sayfa düğmeleri vb.) kullanılması.

#### Development Tasks

- [ ] Görev 9.1.1: `content/en/publication/turkce-kodlama` altındaki `index.md` dosyalarını `type: docs` ile güncelle.
- [ ] Görev 9.1.2: Kitap yapısına uygun olarak dosya ve klasör yapısını düzenle.

#### QA Tasks

- [ ] Test 9.1.1: Kitap sayfalarının "docs" formatında doğru görüntülendiğini ve navigasyonun çalıştığını doğrula.
- [ ] Test 9.1.2: Sol menüde bölüm navigasyonunun ve önceki/sonraki sayfa düğmelerinin çalıştığını doğrula.

## Epic 1 İçerik Zenginleştir

Web sitesindeki mevcut içerikleri zenginleştirerek ziyaretçilere daha kapsamlı ve değerli bilgiler sunmak.

### Story 1.1 Projelerin detaylı gösterimi

As a site ziyaretçisi,
I want Tolga Karataş tarafından yapılan, geliştirilen veya katkıda bulunulan **öne çıkan projelerine** kolayca erişmek ve onları detaylı olarak incelemek, ayrıca diğer projeler hakkında genel bir bakışa sahip olmak,
so that Tolga Karataş'ın uzmanlığını ve somut başarılarını anlayarak, potansiyel işbirlikleri ve fırsatlar hakkında bilgi edinebilirim.

#### Acceptance Criteria (ACs)

1.  **FR1.1.1:** Web sitesi ana sayfasından veya "Projeler" bölümünden **belirlenmiş öne çıkan projelere** (maksimum 3 adet) tam erişim sağlanmalıdır ve **diğer projeler özet olarak listelenmelidir**.
2.  **FR1.1.2:** **Öne çıkan her bir proje sayfası**, projenin amacını, kullanılan temel teknolojileri, elde edilen sonuçları ve varsa canlı demo veya kod deposu bağlantılarını içeren **kapsamlı ve zengin detayda** bilgi sunmalıdır. Diğer projeler için ise sadece başlık, kısa özet ve ilgili dış bağlantılar (varsa) gösterilmelidir.
3.  **NFR1.1.3 (Test Edilebilirlik):** Proje detay sayfalarında yer alan tüm harici bağlantılar (GitHub, canlı demo linkleri vb.) tıklanabilir olmalı ve ilgili hedefe başarıyla yönlendirmelidir (HTTP 200 OK).
4.  **NFR1.1.4 (Kullanılabilirlik):** Kullanıcılar, proje sayfaları arasında sorunsuz gezinebilmelidir (Öne çıkan projelerin detay sayfaları ile proje listesi arasında ve genel proje listesi içinde). Geri ve ileri navigasyon tutarlı çalışmalıdır.
5.  **NFR1.1.5 (Uyumluluk):** Proje detay sayfaları ve proje listeleri, yaygın kullanılan tüm modern tarayıcılarda (Chrome, Firefox, Safari, Edge) ve mobil/masaüstü cihazlarda (iOS, Android, Windows, macOS) tutarlı ve okunabilir bir şekilde görüntülenebilmelidir.
6.  **NFR1.1.6 (Performans):** Proje detay sayfaları, ilk yüklemede 3 saniyenin altında yüklenmelidir (Lighthouse veya WebPageTest ile ölçülecektir).
7.  **NFR1.1.7 (Negatif Senaryo):** Geçersiz bir proje ID'si ile erişim denendiğinde, kullanıcıya "Proje bulunamadı" gibi bilgilendirici bir hata mesajı gösterilmeli ve ana sayfa veya projeler listesine yönlendirilmelidir.

#### Development Tasks

- [ ] Görev 1.1.1: Öne çıkan projeler için Hugo içerik dosyalarını (index.md) oluştur ve gerekli meta verileri ekle.
- [ ] Görev 1.1.2: Diğer projeler için kısa özet içeriklerini oluştur.
- [ ] Görev 1.1.3: Hugo şablonlarında (layouts) 'projects' koleksiyonunun öne çıkan ve özet listeleme kurallarına uygun filtreleme ve sıralama mantığını uygula.
- [ ] Görev 1.1.4: Proje detay sayfalarında canlı demo ve kod deposu bağlantılarını dinamik olarak render et.
- [ ] Görev 1.1.5: Geçersiz proje ID'si durumunda hata sayfasına yönlendirme veya hata mesajı gösterme mekanizmasını geliştir.

#### QA Tasks

- [ ] Test 1.1.1: Tüm öne çıkan projelerin ve diğer projelerin listeleme kurallarına uygunluğunu doğrula.
- [ ] Test 1.1.2: Her bir proje detay sayfasının tüm cihazlarda ve tarayıcılarda doğru görüntülendiğini test et.
- [ ] Test 1.1.3: Tüm harici bağlantıların (GitHub, canlı demo) çalışır durumda olduğunu ve doğru hedefe yönlendirdiğini doğrula (HTTP 200 OK).
- [ ] Test 1.1.4: Proje detay sayfaları arasında ve proje listesi ile detay sayfaları arasında navigasyonun sorunsuz çalıştığını test et.
- [ ] Test 1.1.5: Geçersiz proje ID'si ile erişim denendiğinde beklenen hata mesajının gösterildiğini ve yönlendirmenin doğru yapıldığını test et.
- [ ] Test 1.1.6: Proje detay sayfalarının performans metriklerini (yükleme süresi) Lighthouse/WebPageTest ile ölç ve hedeflere uygunluğunu doğrula.

### Story 1.2 Yayınların detaylı gösterimi

As a site ziyaretçisi,
I want Tolga Karataş'ın yayınladığı makalelere ve yazılara kolayca erişmek ve onları detaylı olarak incelemek,
so that Tolga Karataş'ın bilgi birikimini ve düşüncelerini anlayarak, ilgili konularda bilgi edinebilirim.

#### Acceptance Criteria (ACs)

1.  **FR1.2.1:** Web sitesi ana sayfasından veya "Yayınlar" bölümünden tüm yayınlara tam erişim sağlanmalıdır.
2.  **FR1.2.2:** Her bir yayın sayfası, yayının amacını, ana konularını, ilgili bağlantıları (örneğin, orijinal yayın linki) ve varsa özetini içeren kapsamlı bilgi sunmalıdır.
3.  **NFR1.2.3 (Test Edilebilirlik):** Yayın detay sayfalarında yer alan tüm harici bağlantılar (orijinal yayın linki vb.) tıklanabilir olmalı ve ilgili hedefe başarıyla yönlendirmelidir (HTTP 200 OK).
4.  **NFR1.2.4 (Kullanılabilirlik):** Kullanıcılar, yayın sayfaları arasında sorunsuz gezinebilmelidir. Geri ve ileri navigasyon tutarlı çalışmalıdır.
5.  **NFR1.2.5 (Uyumluluk):** Yayın detay sayfaları ve yayın listeleri, yaygın kullanılan tüm modern tarayıcılarda (Chrome, Firefox, Safari, Edge) ve mobil/masaüstü cihazlarda (iOS, Android, Windows, macOS) tutarlı ve okunabilir bir şekilde görüntülenebilmelidir.
6.  **NFR1.2.6 (Performans):** Yayın detay sayfaları, ilk yüklemede 3 saniyenin altında yüklenmelidir (Lighthouse veya WebPageTest ile ölçülecektir).
7.  **NFR1.2.7 (Negatif Senaryo):** Geçersiz bir yayın ID'si ile erişim denendiğinde, kullanıcıya "Yayın bulunamadı" gibi bilgilendirici bir hata mesajı gösterilmeli ve ana sayfa veya yayınlar listesine yönlendirilmelidir.

#### Development Tasks

- [ ] Görev 1.2.1: Yayınlar için Hugo içerik dosyalarını (index.md) oluştur ve gerekli meta verileri ekle.
- [ ] Görev 1.2.2: Hugo şablonlarında (layouts) 'publication' koleksiyonunun listeleme kurallarına uygun filtreleme ve sıralama mantığını uygula.
- [ ] Görev 1.2.3: Yayın detay sayfalarında orijinal yayın bağlantılarını dinamik olarak render et.
- [ ] Görev 1.2.4: Geçersiz yayın ID'si durumunda hata sayfasına yönlendirme veya hata mesajı gösterme mekanizmasını geliştir.

#### QA Tasks

- [ ] Test 1.2.1: Tüm yayınların listeleme kurallarına uygunluğunu doğrula.
- [ ] Test 1.2.2: Her bir yayın detay sayfasının tüm cihazlarda ve tarayıcılarda doğru görüntülendiğini test et.
- [ ] Test 1.2.3: Tüm harici bağlantıların (orijinal yayın linki) çalışır durumda olduğunu ve doğru hedefe yönlendirdiğini doğrula (HTTP 200 OK).
- [ ] Test 1.2.4: Yayın detay sayfaları arasında ve yayın listesi ile detay sayfaları arasında navigasyonun sorunsuz çalıştığını test et.
- [ ] Test 1.2.5: Geçersiz yayın ID'si ile erişim denendiğinde beklenen hata mesajının gösterildiğini ve yönlendirmenin doğru yapıldığını test et.
- [ ] Test 1.2.6: Yayın detay sayfalarının performans metriklerini (yükleme süresi) Lighthouse/WebPageTest ile ölç ve hedeflere uygunluğunu doğrula.

## Epic 2 Türkçe tercümeleri yap

Web sitesinin tüm içeriğini Türkçe'ye çevirerek daha geniş bir kitleye ulaşmak.

### Story 2.1 Web sitesi içeriğinin Türkçe'ye çevrilmesi

As a Türkçe konuşan ziyaretçi,
I want web sitesindeki tüm içeriği (projeler, yayınlar, etkinlikler, hakkında vb.) Türkçe olarak okuyabilmek,
so that içeriği kendi dilimde anlayabilir ve Tolga Karataş'ın çalışmalarını daha iyi değerlendirebilirim.

#### Acceptance Criteria (ACs)

1.  **FR2.1.1:** Web sitesinin tüm metin içerikleri (başlıklar, açıklamalar, menüler, proje/yayın/etkinlik detayları vb.) Türkçe'ye doğru ve eksiksiz bir şekilde çevrilmelidir.
2.  **FR2.1.2:** Kullanıcılar, web sitesinin herhangi bir sayfasından Türkçe ve İngilizce dil seçenekleri arasında kolayca ve hızlı bir şekilde geçiş yapabilmelidir. Dil seçimi kalıcı olmalıdır (örneğin, çerezler aracılığıyla).
3.  **NFR2.1.3 (Çeviri Kalitesi):** Türkçe çeviriler, dilbilgisi, yazım ve anlam bütünlüğü açısından yüksek kalitede olmalı, yerel kültüre uygun ve doğal bir akıcılık sunmalıdır. (Hedef: %95 doğruluk oranı, profesyonel çevirmen/yerel konuşmacı onayı).
4.  **NFR2.1.4 (Karakter Desteği):** Türkçe'ye özgü karakterler (ç, ğ, ı, ö, ş, ü) tüm sayfalarda ve cihazlarda doğru bir şekilde görüntülenmelidir.
5.  **NFR2.1.5 (Negatif Senaryo):** Desteklenmeyen bir dil seçeneği ile erişim denendiğinde, varsayılan dile (Türkçe veya İngilizce) yönlendirme yapılmalı veya uygun bir hata mesajı gösterilmelidir.

#### Development Tasks

- [ ] Görev 2.1.1: Tüm içerik dosyalarının (projeler, yayınlar, etkinlikler, hakkında vb.) Türkçe versiyonlarını oluştur.
- [ ] Görev 2.1.2: Hugo çoklu dil yapılandırmasını (config.toml veya hugo.yaml) Türkçe için ayarla.
- [ ] Görev 2.1.3: Dil seçimi için kullanıcı arayüzü bileşenini (örneğin, dil değiştirici) geliştir.

#### QA Tasks

- [ ] Test 2.1.1: Web sitesinin tüm metin içeriklerinin Türkçe'ye doğru ve eksiksiz çevrildiğini doğrula.
- [ ] Test 2.1.2: Türkçe ve İngilizce dil seçenekleri arasında sorunsuz ve hızlı geçiş yapıldığını test et. Dil seçiminin kalıcı olduğunu doğrula.
- [ ] Test 2.1.3: Türkçe çevirilerin dilbilgisi, yazım ve anlam bütünlüğü açısından kalitesini doğrula.
- [ ] Test 2.1.4: Türkçe'ye özgü karakterlerin tüm sayfalarda ve cihazlarda doğru görüntülendiğini test et.
- [ ] Test 2.1.5: Desteklenmeyen bir dil seçeneği ile erişim denendiğinde beklenen hata mesajının/yönlendirmenin doğru yapıldığını test et.

## Epic 3 Rusça tercümeleri yap

Web sitesinin tüm içeriğini Rusça'ya çevirerek Rusça konuşan kitleye ulaşmak.

### Story 3.1 Web sitesi içeriğinin Rusça'ya çevrilmesi

As a Rusça konuşan ziyaretçi,
I want web sitesindeki tüm içeriği (projeler, yayınlar, etkinlikler, hakkında vb.) Rusça olarak okuyabilmek,
so that içeriği kendi dilimde anlayabilir ve Tolga Karataş'ın çalışmalarını daha iyi değerlendirebilirim.

#### Acceptance Criteria (ACs)

1.  **FR3.1.1:** Web sitesinin tüm metin içerikleri (başlıklar, açıklamalar, menüler, proje/yayın/etkinlik detayları vb.) Rusça'ya doğru ve eksiksiz bir şekilde çevrilmelidir.
2.  **FR3.1.2:** Kullanıcılar, web sitesinin herhangi bir sayfasından Türkçe, İngilizce ve Rusça dil seçenekleri arasında kolayca ve hızlı bir şekilde geçiş yapabilmelidir. Dil seçimi kalıcı olmalıdır (örneğin, çerezler aracılığıyla).
3.  **NFR3.1.3 (Çeviri Kalitesi):** Rusça çeviriler, dilbilgisi, yazım ve anlam bütünlüğü açısından yüksek kalitede olmalı, yerel kültüre uygun ve doğal bir akıcılık sunmalıdır. (Hedef: %95 doğruluk oranı, profesyonel çevirmen/yerel konuşmacı onayı).
4.  **NFR3.1.4 (Karakter Desteği):** Rusça karakterler tüm sayfalarda ve cihazlarda doğru bir şekilde görüntülenmelidir.
5.  **NFR3.1.5 (Negatif Senaryo):** Desteklenmeyen bir dil seçeneği ile erişim denendiğinde, varsayılan dile (Türkçe veya İngilizce) yönlendirme yapılmalı veya uygun bir hata mesajı gösterilmelidir.

#### Development Tasks

- [ ] Görev 3.1.1: Tüm içerik dosyalarının (projeler, yayınlar, etkinlikler, hakkında vb.) Rusça versiyonlarını oluştur.
- [ ] Görev 3.1.2: Hugo çoklu dil yapılandırmasını (config.toml veya hugo.yaml) Rusça için ayarla.
- [ ] Görev 3.1.3: Dil seçimi için kullanıcı arayüzü bileşenini (örneğin, dil değiştirici) Rusça seçeneğini içerecek şekilde güncelle.

#### QA Tasks

- [ ] Test 3.1.1: Web sitesinin tüm metin içeriklerinin Rusça'ya doğru ve eksiksiz çevrildiğini doğrula.
- [ ] Test 3.1.2: Türkçe, İngilizce ve Rusça dil seçenekleri arasında sorunsuz ve hızlı geçiş yapıldığını test et. Dil seçiminin kalıcı olduğunu doğrula.
- [ ] Test 3.1.3: Rusça çevirilerin dilbilgisi, yazım ve anlam bütünlüğü açısından kalitesini doğrula.
- [ ] Test 3.1.4: Rusça karakterlerin tüm sayfalarda ve cihazlarda doğru görüntülendiğini test et.
- [ ] Test 3.1.5: Desteklenmeyen bir dil seçeneği ile erişim denendiğinde beklenen hata mesajının/yönlendirmenin doğru yapıldığını test et.

## Epic 4: İçerik Stratejisi ve Üretimi

Web sitesini bir düşünce liderliği platformuna dönüştürmek için mevcut içeriği zenginleştirmek ve stratejik yeni içerikler üretmek.

### Story 4.1 Uzmanlık Alanlarına Yönelik Blog Yazıları Oluşturma

As a site ziyaretçisi,
I want Tolga Karataş'ın bilgi güvenliği, yapay zeka ve otomasyon gibi konulardaki uzmanlığını yansıtan derinlemesine blog yazılarını okumak,
so that onun bilgi birikiminden faydalanabilir ve sektördeki yetkinliğini daha iyi anlayabilirim.

#### Acceptance Criteria (ACs)
1.  `docs/blog-yayinlama-plani.md`'de tanımlanan ana temalara uygun en az 5 yeni blog yazısı oluşturulmalıdır.
2.  Her yazı, tanımlanan içerik standardına (front matter, body yapısı) uygun olmalıdır.
3.  Yazılarda kullanılan görseller ve diyagramlar konuyu desteklemeli ve yüksek kalitede olmalıdır.

### Story 4.2 Mevcut Proje ve Yayın Sayfalarını Zenginleştirme

As a potansiyel işveren veya işbirlikçi,
I want mevcut proje ve yayın sayfalarındaki "Lorem Ipsum" gibi yer tutucu metinler yerine, projenin amacını, kapsamını ve sonuçlarını detaylı anlatan zengin içerikler görmek,
so that Tolga Karataş'ın geçmiş çalışmalarının somut etkisini ve değerini tam olarak değerlendirebilirim.

#### Acceptance Criteria (ACs)
1.  `content/project` ve `content/publication` altındaki tüm sayfalarda yer alan yer tutucu metinler kaldırılmalı ve özgün açıklamalarla değiştirilmelidir.
2.  Her proje sayfası, projedeki rolü ve kişisel katkıları net bir şekilde açıklamalıdır.

### Story 4.3 İçerikler Arası Bağlantı Ağı Kurma

As a site kullanıcısı,
I want bir blog yazısını okurken, o konuyla ilgili bir projeye veya akademik yayına kolayca geçiş yapabilmek,
so that konular arasındaki bağlantıları keşfederek bütüncül bir anlayış geliştirebilirim.

#### Acceptance Criteria (ACs)
1.  Yeni oluşturulan her blog yazısında, ilgili en az bir proje veya yayına link verilmelidir.
2.  Proje sayfalarından, o projeyle ilgili yazılmış blog yazılarına veya yayınlara linkler eklenmelidir.

## Checklist Results Report

Bu bölüm, her bir hikaye veya epik için tamamlanan testlerin, kalite kontrollerinin ve kabul kriteri doğrulamalarının özetini içerecektir. Test senaryolarının durumu (geçti/kaldı), bulunan hatalar ve çözümleri burada takip edilecektir.

## Next Steps

- Projelerin detaylı içeriklerini oluştur. (Sorumlu: İçerik Ekibi, Tahmini Bitiş: 2025-07-15)
- Web sitesini Türkçe ve Rusça'ya çevir. (Sorumlu: Çeviri Ekibi, Tahmini Bitiş: 2025-08-30)
- CI/CD pipeline'ı kur. (Sorumlu: DevOps Ekibi, Tahmini Bitiş: 2025-07-30)

### Epic 5: "Türkçe Düşün, Yapay Zeka Üretsin" Kitabının Yayınlanması

"Türkçe Düşün, Yapay Zeka Üretsin" adlı kitabın, web sitesinde bölümler halinde yayınlanarak okuyuculara sunulması.

#### Story 5.1 Kitabın Bölümlere Ayrılıp Yayınlanması

**As a** site ziyaretçisi,
**I want** "Türkçe Düşün, Yapay Zeka Üretsin" kitabını web sitesi üzerinden online olarak, bölümler halinde okuyabilmek,
**so that** gereksinim mühendisliği ve yapay zeka ile prompt üretimi konularındaki bu değerli kaynağa kolayca erişebilir ve kendi projelerimde bu bilgileri kullanabilirim.

##### Acceptance Criteria (ACs)

1.  **FR5.1.1:** `tum-kitap.md` dosyasındaki içerik, `content/tr/publication/turkce-dusun-yapay-zeka-uretsin` dizini altına, her bölüm için ayrı bir alt dizin oluşturularak bölünmelidir.
2.  **FR5.1.2:** Her bölüm dizininin içinde, bölüm içeriğini barındıran bir `index.md` dosyası bulunmalıdır.
3.  **FR5.1.3:** Kitabın ana giriş sayfası (`content/tr/publication/turkce-dusun-yapay-zeka-uretsin/_index.md`) oluşturulmalı ve tüm bölümlere buradan link verilmelidir.
4.  **FR5.1.4:** Bölümler, menüde veya sayfada doğru sıralama ile (`weight` parametresi kullanılarak) gösterilmelidir.
5.  **NFR5.1.5 (Uyumluluk):** Tüm kitap bölümleri, yaygın kullanılan tüm modern tarayıcılarda ve mobil/masaüstü cihazlarda tutarlı ve okunabilir bir şekilde görüntülenebilmelidir.
6.  **NFR5.1.6 (Navigasyon):** Kullanıcılar, kitap bölümleri arasında (önceki/sonraki bölüm) kolayca gezinebilmelidir.

##### Development Tasks

- [ ] Görev 5.1.1: `tum-kitap.md` dosyasını oku ve içeriği manuel olarak bölümlere ayır.
- [ ] Görev 5.1.2: Her bölüm için `content/tr/publication/turkce-dusun-yapay-zeka-uretsin/bolum-X` formatında dizinler oluştur.
- [ ] Görev 5.1.3: Her bölüm içeriğini ilgili dizindeki `index.md` dosyasına yaz.
- [ ] Görev 5.1.4: Hugo `front matter`'larının (title, weight vb.) her bölüm için doğru şekilde oluşturulduğundan emin ol.
- [ ] Görev 5.1.5: Kitabın ana giriş sayfasını (`_index.md`) oluştur ve bölümlere linkleri ekle.

##### QA Tasks

- [ ] Test 5.1.1: Tüm bölümlerin doğru dizinlere ve dosyalara ayrıldığını doğrula.
- [ ] Test 5.1.2: Her bölüm sayfasının içeriğinin eksiksiz ve doğru olduğunu kontrol et.
- [ ] Test 5.1.3: Bölüm sıralamasının doğru olduğunu doğrula.
- [ ] Test 5.1.4: Bölümler arası ve ana sayfaya geri navigasyonun çalıştığını test et.
- [ ] Test 5.1.5: Tüm kitap sayfalarının farklı cihaz ve tarayıcılarda düzgün görüntülendiğini kontrol et.
