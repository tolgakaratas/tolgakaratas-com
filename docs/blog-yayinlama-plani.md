# Blog ve Yayın Planı

Bu doküman, `tolgakaratas.com` sitesinin "Blog" (Post) ve "Yayınlar" (Publication) bölümlerinde yer alacak içeriklerin stratejisini ve yayınlanma sürecini tanımlar.

## 1. Amaç

Uzmanlık alanlarında düzenli ve yüksek kaliteli içerikler üreterek siteyi canlı tutmak, organik trafiği artırmak ve Tolga Karataş'ı bir düşünce lideri olarak konumlandırmak.

## 2. Konu Fikirleri (İçerik Havuzu)

Aşağıdaki konulardan yola çıkarak bir içerik takvimi oluşturulabilir:

- [ ] **Vaka Çalışması:** Denomas Güvenlik Otomasyonu projesinde SCAP ve OVAL entegrasyonu nasıl yapıldı?
- [ ] **Teknik İnceleme:** Freqtrade için dağıtık backtest mimarisi kurmanın avantajları ve zorlukları.
- [ ] **Görüş Yazısı:** Bağımsız, düşmanca araştırmaların (adversarial research) devlet regülasyonlarını nasıl şekillendirdiği üzerine bir analiz.
- [ ] **Rehber:** ISO 27001 uyumlu bir altyapı için otomasyonun rolü.
- [ ] **Kişisel Deneyim:** Bir teknoloji girişimini sıfırdan kurarken öğrenilen 5 kritik ders.
- [ ] ... (Bu liste sürekli güncellenecektir)

## 3. Her Yazı İçin İçerik Standardı

Her yazı `content/post/yazi-basligi/` altında `index.md` olarak oluşturulacaktır.

### `index.md` Front Matter Şablonu

```yaml
---
title: "Yazı Başlığı"
date: YYYY-MM-DD
summary: "Yazının 1-2 cümlelik, sosyal medyada ve liste sayfalarında dikkat çekecek özeti."
authors:
  - tolga
tags:
  - "Anahtar Kelime 1"
  - "Teknoloji"
  - "Sektör"
image:
  caption: 'Görsel açıklaması'
  # Yazıyı temsil eden bir görseli bu sayfanın klasörüne featured.jpg/png olarak ekleyin.
---
```

### `index.md` İçerik (Body) Şablonu

```markdown
### Giriş: Sorunu veya Konuyu Tanımla
Okuyucunun dikkatini çekecek, yazının neden önemli olduğunu anlatan bir başlangıç yap.

### Ana Bölüm: Detaylı Açıklama ve Analiz
Konuyu alt başlıklarla detaylandır. Teknik yazılarda kod blokları (` ```python ... ``` `), diyagramlar (`mermaid`) ve formüller kullanarak içeriği zenginleştir.

### Sonuç: Özet ve Geleceğe Bakış
Yazının ana fikirlerini özetle ve okuyucuya bir sonraki adımı (call-to-action) belirt (örn: "Bu konu hakkındaki düşüncelerinizi X'te paylaşın", "İlgili projem olan Y'yi inceleyin").
```

## 4. Yayınlama Süreci

1.  **Fikir Seçimi:** İçerik havuzundan bir konu seçilir.
2.  **Taslak Hazırlama:** İçerik standardına uygun olarak `index.md` dosyası oluşturulur.
3.  **Görsel ve Medya Ekleme:** Yazıya uygun, telif hakkı sorunu olmayan bir görsel bulunur ve eklenir.
4.  **İç Bağlantılar:** Yazı içinde ilgili diğer projelere, yayınlara veya blog yazılarına linkler eklenir.
5.  **Gözden Geçirme ve Yayınlama:** Değişiklikler yerel sunucuda kontrol edildikten sonra siteye yüklenir.
