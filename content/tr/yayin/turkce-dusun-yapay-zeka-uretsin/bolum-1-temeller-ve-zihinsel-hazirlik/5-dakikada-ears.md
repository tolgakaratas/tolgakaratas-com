---
title: "Bölüm 2: 5 Dakikada EARS - İlk Gereksinimimizi Yazalım"
weight: 3
summary: "Teoriye boğulmadan önce EARS'ın gücünü anında görün. Belirsiz bir fikrin sadece 3 basit adımla nasıl test edilebilir bir gereksinime dönüştüğünü öğrenin."
type: docs
tags: ["hızlı başlangıç", "EARS", "pratik"]
---

[Seviye: Temel]

Teorinin derinliklerine dalmadan önce, EARS'ın pratikte ne kadar basit ve güçlü olduğunu görelim. Amacımız, belirsiz bir fikri, herkesin aynı şeyi anladığı, test edilebilir bir gereksinime dönüştürmektir.

### 2.1. Hızlı Başlangıç: "Akıllı Lamba" Fikri

Elimizdeki dağınık fikir şu olsun: **"Yeni bir akıllı lamba tasarlıyoruz ve lamba sesle kontrol edilebilmeli."**

Bu bir hedeftir, gereksinim değil. Gelin bunu EARS ile netleştirelim.

1.  **Sistemi Tanımla:** Üzerinde çalıştığımız şey ne? -> "Akıllı Lamba".
2.  **Tetikleyiciyi (Olayı) Bul:** Sistemin tepki vermesini ne sağlar? -> "Kullanıcının bir komut vermesi". Hangi komut? -> "'Aç' komutu".
3.  **Beklenen Tepkiyi Belirle:** Tetikleyici gerçekleştiğinde sistem ne yapmalı? -> "Işığı yakmalı".

Şimdi bu üç parçayı EARS'ın en yaygın kalıplarından biri olan **Olay Odaklı (Event-Driven)** kalıba yerleştirelim:

- **İngilizce Kalıp:** `When [Event], the SYSTEM_NAME shall [System Response].`
- **Türkçe Kalıp:** `[Olay] olduğunda, SİSTEM_ADI, [Sistem Tepkisi]'ni sağlayacaktır.`

Bu kalıbı doldurduğumuzda ortaya çıkan sonuç:

> **"Kullanıcı 'aç' komutunu verdiğinde, Akıllı Lamba, ışığı yakacaktır."**

### 2.2. Anında Başarı: Ne Kazandık?

Sadece birkaç dakikada, belirsiz bir fikirden son derece net bir gereksinime ulaştık:

- **Net:** Ne olunca ne olacağı kesin olarak belli.
- **Test Edilebilir:** Bir test mühendisi (veya bir AI agent), kullanıcıya "aç" dedirtip lambanın yanıp yanmadığını kolayca kontrol edebilir.
- **Kapsamı Belli:** Sorumluluk "Akıllı Lamba" sistemine aittir.
- **Anlaşılır:** Hem müşteri hem de mühendis bu cümleden aynı şeyi anlar.

İşte EARS'ın gücü budur. Şimdi, bu basit yapının arkasındaki derinliği ve diğer kalıpları keşfetmeye hazırsınız.

{{% callout note %}}
**Bu Bölümden Akılda Kalanlar**

- EARS, belirsiz hedefleri; net, test edilebilir ve anlaşılır gereksinimlere dönüştürür.
- Bir gereksinimin üç temel unsuru vardır: Tetikleyici (ne olunca?), Sistem (kim yapacak?) ve Tepki (ne yapacak?).
- Basit bir kalıp kullanmak, karmaşık fikirleri herkes için açık hale getirebilir.
  {{% /callout %}}

{{% callout note %}}
**Sıra Sizde! (Pratik Alıştırma)**

Yukarıdaki "Akıllı Lamba" örneğinden yola çıkarak, lambayı kapatmak için gereken EARS gereksinimini siz yazın. Hangi kelimelerin değişmesi gerektiğini fark ettiniz mi?
{{% /callout %}}
