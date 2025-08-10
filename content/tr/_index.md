---
title: "DENEME"
date: 2025-08-10
type: landing
translationKey: homepage

design:
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      username: tolga
      text: ""
      button:
        text: CV İndir
        url: uploads/tolga-karatas-hakkinda.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: '📚 Araştırmalarım'
      subtitle: ''
      text: |-
        İstanbul Yıldız Teknik Üniversitesi Teknopark'ta bir araştırma bilimcisiyim. Bilgi güvenliği, veri analizi, makine öğrenmesi, derin öğrenme, yapay zeka ve algo-ticaret üzerine blog yazıyorum.

        Bilim ve teknolojinin ekonomideki rolünü kapsamlı bir şekilde araştırmak için bir dizi nitel ve nicel yöntem uyguluyorum.
        
        İşbirliği için lütfen ulaşın 😃
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Öne Çıkan Yayınlar
      filters:
        folders:
          - yayin
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Son Yayınlar
      text: ""
      filters:
        folders:
          - yayin
        exclude_featured: true
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Son ve Gelecek Konuşmalar
      filters:
        folders:
          - etkinlik
    design:
      view: article-grid
      columns: 1
  - block: collection
    id: news
    content:
      title: Son Haberler
      subtitle: ''
      text: ''
      page_type: yazi
      count: 5
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      offset: 0
      order: desc
    design:
      view: date-title-summary
      spacing:
        padding: [0, 0, 0, 0]
---
