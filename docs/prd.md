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

### Background Context

Mevcut özgeçmiş formatlarımın 30 yıllık geniş ve çeşitli deneyimimi tam olarak yansıtmadığını fark ettim. Bu PRD, bu sorunu çözmek ve deneyimimi daha yapılandırılmış, kapsamlı ve etkileşimli bir formatta sunmak için bir yol haritası görevi görecektir.

### Change Log

| Date | Version | Description | Author |
| :--- | :------ | :---------- | :----- |
| 2025-06-29 | 1.0     | PRD dökümanı analiz edildi ve güncellenmeye başlandı. | BMAD Master Orchestrator |

## Requirements

### Functional

- **FR1:** Proje portföyü, Tolga Karataş'ın projelerini, yayınlarını, etkinliklerini ve diğer ilgili içeriklerini sergilemelidir.
- **FR2:** Kullanıcılar, projeler arasında kolayca gezinebilmeli ve her bir projenin detaylı açıklamasına erişebilmelidir.
- **FR3:** Web sitesi, farklı cihazlarda (masaüstü, tablet, mobil) uyumlu bir şekilde görüntülenmelidir.

### Non Functional

- **NFR1:** Web sitesi hızlı yüklenmeli ve yüksek performans göstermelidir.
- **NFR2:** Web sitesi güvenli olmalı ve kullanıcı verilerini korumalıdır.
- **NFR3:** Web sitesi SEO (Arama Motoru Optimizasyonu) için optimize edilmelidir.

## User Interface Design Goals

### Overall UX Vision
Kullanıcı dostu, sezgisel ve etkileyici bir deneyim sunmak.

### Key Interaction Paradigms
- Kolay navigasyon
- Hızlı erişim
- Etkileşimli içerik

### Core Screens and Views
- Ana Sayfa
- Projeler Sayfası
- Yayınlar Sayfası
- Etkinlikler Sayfası
- Hakkında Sayfası

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

## Technical Assumptions

### Repository Structure: { Monorepo, Polyrepo, etc...}
Monorepo

### Service Architecture
Statik site (Hugo)

### Testing requirements
- Birim testleri
- Entegrasyon testleri
- Uçtan uca testler

### Additional Technical Assumptions and Requests
- CI/CD pipeline kurulacak.
- Otomatik deployment yapılacak.

## Epics

- Epic1: İçerik zenginleştir
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

### Story 1.2 [Hikaye Başlığı]
#### Acceptance Criteria (ACs)
## Epic 2 Türkçe tercümeleri yap
### Story 2.1 [Hikaye Başlığı]
#### Acceptance Criteria (ACs)
## Epic 3 Rusça tercümeleri yap
### Story 3.1 [Hikaye Başlığı]
#### Acceptance Criteria (ACs)
## Checklist Results Report

## Next Steps

- Projelerin detaylı içeriklerini oluştur.
- Web sitesini Türkçe ve Rusça'ya çevir.
- CI/CD pipeline'ı kur.