# Proje Yayınlama Planı

Bu döküman, `tolgakaratas.com` web sitesinin "Projects" bölümünde yer alacak tüm projelerin sistematik bir şekilde nasıl ekleneceğini ve yönetileceğini tanımlar.

## 1. Amaç

Sitede profesyonel, kişisel ve akademik tüm projeleri tutarlı ve kapsamlı bir formatta sergileyerek portfolyoyu zenginleştirmek.

## 2. Projelerin Tespiti ve Listelenmesi

Yayınlanacak tüm projelerin bir listesini çıkararak işe başlayacağız. Bu liste, aşağıdaki adımlarla oluşturulacaktır:

- **Mevcut Projeler:** `content/project/` altında zaten var olan projeler gözden geçirilecek.
- **Özgeçmişten Gelen Projeler:** CV'de belirtilen şirketlerde (DigiTuccar, Forceye, İlim Teknoloji vb.) yapılan önemli çalışmalar proje olarak eklenecek.
- **Diğer Projeler:** Kişisel, hobi amaçlı, akademik veya açık kaynak kodlu katkılar listeye dahil edilecek.

### Proje Listesi (Takip için)

- [ ] **Denomas Audit Information Management Automation Software (52819)** - *Mevcut, içerik zenginleştirilecek.*
- [ ] **Denomas Management Automation Platform (65780)** - *Mevcut, içerik zenginleştirilecek.*
- [ ] **Denomas Security Automation Software (73271)** - *Mevcut, içerik zenginleştirilecek.*
- [x] **DigiTuccar - Algoritmik Ticaret Backtesting Çerçevesi** - *İçerik güncellendi, sayfa oluşturuldu.*
- [ ] **İlim Teknoloji A.Ş. - Monitoring Otomasyon Yazılımı**
- [ ] **Ilim Technology LLC - Yenilikçi Güvenlik Çözümleri**
- [ ] **İlim Teknoloji A.Ş. - Monitoring Otomasyon Yazılımı**
- [ ] **Ilim Technology LLC - Yenilikçi Güvenlik Çözümleri**
- [ ] *Eklenecek diğer projeler için bu liste güncellenecektir...*

## 3. Her Proje İçin İçerik Standardı

Her projenin tutarlı bir yapıda olması için aşağıdaki şablon kullanılacaktır. Her proje `content/project/proje-adi/` klasörü altında `index.md` dosyası olarak oluşturulacaktır.

### `index.md` Front Matter Şablonu

```yaml
---
title: "Proje Başlığı"
date: YYYY-MM-DD
summary: "Projenin 1-2 cümlelik kısa ve dikkat çekici özeti. Liste sayfalarında görünecek."
tags:
  - "Teknoloji 1"
  - "Teknoloji 2"
  - "Alan Adı (örn: Güvenlik)"
# Projeyi temsil eden bir görseli bu sayfanın klasörüne ekleyin.
image:
  filename: "featured.jpg"
  caption: "Görsel açıklaması (isteğe bağlı)"
# Projenin canlı linki varsa
external_link: ""
# Projenin kaynak kod linki varsa
url_code: "https://github.com/kullanici/proje"
---
```

### `index.md` İçerik (Body) Şablonu

Projenin `---` ile ayrılan gövde kısmında aşağıdaki başlıklar kullanılmalıdır:

```markdown
### Projenin Amacı
Bu bölümde projenin hangi sorunu çözdüğü, hangi ihtiyaca yönelik geliştirildiği anlatılacaktır.

### Kullanılan Teknolojiler
Projede kullanılan programlama dilleri, framework'ler, veritabanları ve diğer önemli araçlar listelenecektir.

### Benim Rolüm ve Katkılarım
Projedeki görev tanımı, sorumluluklar ve kişisel olarak sağlanan katkılar detaylandırılacaktır.

### Öne Çıkan Özellikler
Projenin en dikkat çekici veya yenilikçi 2-3 özelliği maddeler halinde açıklanacaktır.
```

## 4. Yayınlama Süreci

1.  **Bilgi Toplama:** Yukarıdaki "Proje Listesi"ndeki her bir proje için "İçerik Standardı"na uygun şekilde bilgiler toplanır.
2.  **Klasör Oluşturma:** Her proje için `content/project/` altında `proje-adi` formatında yeni bir klasör oluşturulur.
3.  **`index.md` ve Görsel Ekleme:** Proje klasörünün içine `index.md` dosyası oluşturulur ve şablona göre doldurulur. `featured.jpg` (veya `.png`) görseli de bu klasöre eklenir.
4.  **Gözden Geçirme ve Yayınlama:** Değişiklikler yerel sunucuda kontrol edildikten sonra siteye yüklenir.