---
title: ""
date: 2022-10-24
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
        text: Скачать резюме
        url: uploads/resume.pdf
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
      title: '📚 Мои исследования'
      subtitle: ''
      text: |-
        Я научный сотрудник в Технопарке Стамбульского технического университета Йылдыз. Я веду блог об информационной безопасности, анализе данных, машинном обучении, глубоком обучении и алгоритмической торговле.

        Я применяю ряд качественных и количественных методов для всестороннего исследования роли науки и технологий в экономике.
        
        Пожалуйста, свяжитесь со мной для сотрудничества 😃
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Избранные публикации
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Последние публикации
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Недавние и предстоящие выступления
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1
  - block: collection
    id: news
    content:
      title: Последние новости
      subtitle: ''
      text: ''
      page_type: post
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
