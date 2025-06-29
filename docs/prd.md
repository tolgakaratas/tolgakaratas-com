# Tolga Karataş Proje Portföyü Ürün Gereksinimleri Belgesi (PRD)

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
- Kullanılacak Teknolojiler: Hugo, Go (Hugo için), Markdown, HTML, CSS, JavaScript.

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

## Epic 1 İçerik Zenginleştir

Web sitesindeki mevcut içerikleri zenginleştirerek ziyaretçilere daha kapsamlı ve değerli bilgiler sunmak.

### Story 1.1 Projelerin detaylı gösterimi

As a site ziyaretçisi,
I want Tolga Karataş tarafından yapılan, geliştirilen veya katkıda bulunulan **öne çıkan projelerine** kolayca erişmek ve onları detaylı olarak incelemek, ayrıca diğer projeler hakkında genel bir bakışa sahip olmak,
so that Tolga Karataş'ın uzmanlığını ve somut başarılarını anlayarak, potansiyel işbirlikleri ve fırsatlar hakkında bilgi edinebilirim.

#### Acceptance Criteria (ACs)

1.  **FR1.1.1:** Web sitesi ana sayfasından veya "Projeler" bölümünden **belirlenmiş öne çıkan projelere** tam erişim sağlanmalıdır ve **diğer projeler özet olarak listelenmelidir**.
2.  **FR1.1.2:** **Öne çıkan her bir proje sayfası**, projenin amacını, kullanılan temel teknolojileri, elde edilen sonuçları ve varsa canlı demo veya kod deposu bağlantılarını içeren **kapsamlı ve zengin detayda** bilgi sunmalıdır. Diğer projeler için ise sadece başlık, kısa özet ve ilgili dış bağlantılar (varsa) gösterilmelidir.
3.  **NFR1.1.3:** Proje detay sayfalarında yer alan tüm harici bağlantılar (örneğin GitHub, canlı demo linkleri) çalışır durumda olmalıdır.
4.  **NFR1.1.4:** Kullanıcılar, proje sayfaları arasında sorunsuz gezinebilmelidir (Öne çıkan projelerin detay sayfaları ile proje listesi arasında ve genel proje listesi içinde).
5.  **NFR1.1.5:** Proje detay sayfaları ve proje listeleri, mobil ve masaüstü cihazlarda tutarlı ve okunabilir bir şekilde görüntülenebilmelidir.

#### Tasks / Subtasks

- [ ] Görev 1.1.1: Öne çıkan projeler için içerik dosyalarını (index.md) oluştur.
- [ ] Görev 1.1.2: Diğer projeler için kısa özet içeriklerini oluştur.
- [ ] Görev 1.1.3: Hugo projesindeki 'projects' koleksiyonunun öne çıkan ve özet listeleme kurallarına uygun olduğundan emin ol.
- [ ] Görev 1.1.4: Tüm harici bağlantıları test et.

### Story 1.2 Yayınların detaylı gösterimi

As a site ziyaretçisi,
I want Tolga Karataş'ın yayınladığı makalelere ve yazılara kolayca erişmek ve onları detaylı olarak incelemek,
so that Tolga Karataş'ın bilgi birikimini ve düşüncelerini anlayarak, ilgili konularda bilgi edinebilirim.

#### Acceptance Criteria (ACs)

1.  **FR1.2.1:** Web sitesi ana sayfasından veya "Yayınlar" bölümünden tüm yayınlara tam erişim sağlanmalıdır.
2.  **FR1.2.2:** Her bir yayın sayfası, yayının amacını, ana konularını, ilgili bağlantıları (örneğin, orijinal yayın linki) ve varsa özetini içeren kapsamlı bilgi sunmalıdır.
3.  **NFR1.2.3:** Yayın detay sayfalarında yer alan tüm harici bağlantılar çalışır durumda olmalıdır.
4.  **NFR1.2.4:** Kullanıcılar, yayın sayfaları arasında sorunsuz gezinebilmelidir.
5.  **NFR1.2.5:** Yayın detay sayfaları ve yayın listeleri, mobil ve masaüstü cihazlarda tutarlı ve okunabilir bir şekilde görüntülenebilmelidir.

#### Tasks / Subtasks
#### Estimated Effort
- S (Küçük)

#### Dependencies
- İçerik Ekibi'nin yayın detaylarını sağlaması.

- [ ] Görev 1.2.1: Yayınlar için içerik dosyalarını (index.md) oluştur.
- [ ] Görev 1.2.2: Hugo projesindeki 'publication' koleksiyonunun listeleme kurallarına uygun olduğundan emin ol.
- [ ] Görev 1.2.3: Tüm harici bağlantıları test et.

## Epic 2 Türkçe tercümeleri yap

Web sitesinin tüm içeriğini Türkçe'ye çevirerek daha geniş bir kitleye ulaşmak.

### Story 2.1 Web sitesi içeriğinin Türkçe'ye çevrilmesi

As a Türkçe konuşan ziyaretçi,
I want web sitesindeki tüm içeriği (projeler, yayınlar, etkinlikler, hakkında vb.) Türkçe olarak okuyabilmek,
so that içeriği kendi dilimde anlayabilir ve Tolga Karataş'ın çalışmalarını daha iyi değerlendirebilirim.

#### Acceptance Criteria (ACs)

1.  **FR2.1.1:** Web sitesinin tüm metin içerikleri (başlıklar, açıklamalar, menüler vb.) Türkçe'ye çevrilmelidir.
2.  **FR2.1.2:** Türkçe ve İngilizce dil seçenekleri arasında kolayca geçiş yapılabilmelidir.
3.  **NFR2.1.3:** Çeviriler dilbilgisi ve anlam bütünlüğü açısından doğru olmalıdır.
4.  **NFR2.1.4:** Türkçe karakterler (ç, ğ, ı, ö, ş, ü) doğru bir şekilde görüntülenmelidir.

#### Tasks / Subtasks
#### Estimated Effort
- L (Büyük)

#### Dependencies
- İçerik Ekibi'nin tüm içeriği tamamlaması.

- [ ] Görev 2.1.1: Tüm içerik dosyalarının Türkçe versiyonlarını oluştur.
- [ ] Görev 2.1.2: Hugo çoklu dil yapılandırmasını ayarla.
- [ ] Görev 2.1.3: Çevirileri gözden geçir ve düzelt.

## Epic 3 Rusça tercümeleri yap

Web sitesinin tüm içeriğini Rusça'ya çevirerek Rusça konuşan kitleye ulaşmak.

### Story 3.1 Web sitesi içeriğinin Rusça'ya çevrilmesi

As a Rusça konuşan ziyaretçi,
I want web sitesindeki tüm içeriği (projeler, yayınlar, etkinlikler, hakkında vb.) Rusça olarak okuyabilmek,
so that içeriği kendi dilimde anlayabilir ve Tolga Karataş'ın çalışmalarını daha iyi değerlendirebilirim.

#### Acceptance Criteria (ACs)

1.  **FR3.1.1:** Web sitesinin tüm metin içerikleri (başlıklar, açıklamalar, menüler vb.) Rusça'ya çevrilmelidir.
2.  **FR3.1.2:** Türkçe, İngilizce ve Rusça dil seçenekleri arasında kolayca geçiş yapılabilmelidir.
3.  **NFR3.1.3:** Çeviriler dilbilgisi ve anlam bütünlüğü açısından doğru olmalıdır.
4.  **NFR3.1.4:** Rusça karakterler doğru bir şekilde görüntülenmelidir.

#### Tasks / Subtasks
#### Estimated Effort
- L (Büyük)

#### Dependencies
- İçerik Ekibi'nin tüm içeriği tamamlaması.
- Türkçe çevirinin tamamlanması.

- [ ] Görev 3.1.1: Tüm içerik dosyalarının Rusça versiyonlarını oluştur.
- [ ] Görev 3.1.2: Hugo çoklu dil yapılandırmasını Rusça için ayarla.
- [ ] Görev 3.1.3: Çevirileri gözden geçir ve düzelt.
## Checklist Results Report

## Next Steps

- Projelerin detaylı içeriklerini oluştur. (Sorumlu: İçerik Ekibi, Tahmini Bitiş: 2025-07-15)
- Web sitesini Türkçe ve Rusça'ya çevir. (Sorumlu: Çeviri Ekibi, Tahmini Bitiş: 2025-08-30)
- CI/CD pipeline'ı kur. (Sorumlu: DevOps Ekibi, Tahmini Bitiş: 2025-07-30)