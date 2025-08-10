# Proje Mimarisi

Bu döküman, `tolgakaratas.com` web sitesinin teknik mimarisini, klasör yapısını ve temel çalışma prensiplerini açıklamaktadır.

## 1. Genel Bakış

Web sitesi, **Hugo** statik site oluşturucusu ve **Hugo Blox** teması kullanılarak geliştirilmiştir. Bu yaklaşım, yüksek performans, güvenlik ve basit bir dağıtım (deployment) süreci sunar. İçerikler Markdown formatında yönetilir ve site, bir CI/CD süreci ile otomatik olarak derlenip yayınlanır.

- **Statik Site Oluşturucu:** Hugo (v0.120.0+)
- **Tema:** Hugo Blox Framework
- **İçerik Formatı:** Markdown
- **Yapılandırma:** YAML
- **Deployment:** Netlify (veya benzeri bir platform) üzerinden Git tabanlı CI/CD

## 2. Klasör Yapısı

Proje, standart bir Hugo yapısını takip eder. Ana klasörler ve görevleri aşağıda açıklanmıştır:

```
tolgakaratas-com/
├── assets/             # SCSS, JS ve Hugo Pipes tarafından işlenecek medya dosyaları
├── config/             # Site yapılandırma dosyaları
│   └── _default/
│       ├── hugo.yaml   # Ana Hugo yapılandırması
│       ├── menus.yaml  # Çok dilli menü tanımları
│       └── params.yaml # Tema'ya özel parametreler (renkler, fontlar vb.)
├── content/            # Web sitesinin tüm içeriği (Markdown dosyaları)
│   ├── authors/        # Yazar profilleri
│   ├── event/          # Konuşmalar ve etkinlikler
│   ├── post/           # Blog yazıları
│   ├── project/        # Proje portfolyosu
│   ├── publication/    # Yayınlar
│   ├── _index.md       # Ana sayfa içeriği ve yapısı
│   └── experience.md   # Deneyim sayfası
├── data/               # Yapılandırılmış veriler (kullanılmıyor)
├── docs/               # Proje dökümantasyonu (PRD, mimari vb.)
│   ├── architecture.md
│   └── prd.md
├── i18n/               # Arayüz çeviri dosyaları (örn: tr.yaml)
├── layouts/            # Tema şablonlarını özelleştirmek için kullanılır (şu an boş)
├── static/             # İşlenmeden doğrudan kopyalanacak statik dosyalar
│   └── uploads/
│       └── resume.pdf  # CV dosyası gibi statik varlıklar
└── go.mod              # Hugo modülleri bağımlılıkları
```

### 2.1. `config`

Sitenin tüm yapılandırması bu klasörde bulunur.

- **`hugo.yaml`**: Hugo'nun temel ayarları, dil yapılandırması, URL yapısı gibi genel ayarları içerir.
- **`menus.yaml`**: İngilizce (`en`) ve Türkçe (`tr`) için ayrı ayrı menü yapılarını tanımlar. Yeni diller eklendiğinde burası güncellenir.
- **`params.yaml`**: Hugo Blox temasının görünümünü (renk teması, fontlar, özelliklerin etkinleştirilmesi/devre dışı bırakılması) kontrol eden parametreleri barındırır.

### 2.2. `content`

Sitenin kalbidir. Tüm metin tabanlı içerikler burada, Markdown formatında saklanır.

- **İçerik Türleri:** `project`, `post`, `event` gibi her bir alt klasör, farklı bir içerik türünü temsil eder.
- **Page Bundles:** Her bir içerik (örneğin bir proje), kendi klasörü içinde (`project/proje-adi/`) bir `index.md` (veya `index.en.md`, `index.tr.md`) dosyası ve bu içeriğe ait görseller gibi diğer varlıklarla birlikte "Page Bundle" olarak yönetilir. Bu, içeriğin taşınabilir ve yönetilebilir olmasını sağlar.
- **Ana Sayfa (`_index.md`):** Ana sayfanın yapısını ve hangi "widget"ların (blokların) gösterileceğini tanımlar.

### 2.3. `i18n`

Uluslararasılaştırma (Internationalization) dosyalarını içerir. `tr.yaml`, `en.yaml` gibi dosyalar, temada yer alan "Read More", "Recent Posts" gibi sabit metinlerin çevirilerini barındırır.

### 2.4. `static`

Hugo tarafından herhangi bir işleme tabi tutulmadan doğrudan sitenin kök dizinine kopyalanacak dosyalar burada yer alır. PDF'ler, `favicon.ico` gibi dosyalar için idealdir.

### 2.5. `docs`

Projenin kendisiyle ilgili dökümantasyonu içerir. Bu, projenin zaman içinde bakımını ve geliştirilmesini kolaylaştırır.

## 3. Çoklu Dil Mimarisi (Multilingual)

Site, İngilizce (varsayılan) ve Türkçe dillerini destekleyecek şekilde yapılandırılmıştır. Gelecekte Rusça gibi yeni dillerin eklenmesi de bu mimari ile kolaydır.

- **URL Yapısı:** Türkçe içerikler `/tr/` alt dizininde sunulur. İngilizce içerikler ise kök dizinde (`/`) yer alır. Bu, `config/_default/hugo.yaml` dosyasındaki `defaultContentLanguageInSubdir: false` ayarı ile kontrol edilir.
- **İçerik Dosyaları:** Bir içeriğin farklı dillerdeki versiyonları, aynı page bundle klasörü içinde dosya adı son ekleri ile yönetilir.
  - `content/project/proje-adi/index.en.md` (İngilizce içerik)
  - `content/project/proje-adi/index.tr.md` (Türkçe içerik)
- **Arayüz Çevirileri:** `i18n/tr.yaml` dosyası, tema arayüzünün Türkçeleştirilmesini sağlar.
- **Menüler:** `config/_default/menus.yaml` içinde her dil için ayrı bir menü tanımı bulunur.

## 4. Veri Akışı ve İçerik Yönetimi

1.  **İçerik Oluşturma:** Yeni bir proje, blog yazısı veya etkinlik eklemek için ilgili `content` alt klasöründe yeni bir page bundle (klasör ve `index.xx.md` dosyası) oluşturulur.
2.  **Metadata (Front Matter):** Her Markdown dosyasının başındaki YAML bloğu (`--- ... ---`), o içeriğin başlık, tarih, etiketler, özet gibi meta verilerini tanımlar.
3.  **Derleme:** `hugo` komutu çalıştırıldığında, Hugo `content` klasöründeki tüm dosyaları okur, `layouts` klasöründeki şablonlarla birleştirir ve `public` adında bir klasörün içine tamamen statik HTML, CSS ve JS dosyalarından oluşan siteyi oluşturur.
4.  **Dağıtım (Deployment):** Proje, bir Git deposuna (örn. GitHub) gönderildiğinde, Netlify gibi bir servis bu değişikliği algılar, `hugo` komutunu çalıştırarak siteyi derler ve dünya çapındaki CDN'lerine dağıtarak yayına alır.

## 5. Özelleştirme ve Genişletme

- **Görsel Özelleştirme:** Renkler, fontlar ve diğer stil ayarları `config/_default/params.yaml` üzerinden kod yazmadan değiştirilebilir.
- **HTML Yapısını Değiştirme:** Bir sayfanın HTML yapısını değiştirmek gerekirse, Hugo Blox temasının ilgili şablon dosyası `layouts/` klasörüne kopyalanır ve burada düzenlenir. Bu, temanın orijinal dosyalarını bozmadan özelleştirme yapmayı sağlar.
- **Yeni İçerik Türleri:** Yeni bir içerik türü (örneğin "Kurslar") eklemek için `content/courses/` adında bir klasör ve `layouts/courses/` altında `single.html` ve `list.html` şablonları oluşturmak yeterlidir.
