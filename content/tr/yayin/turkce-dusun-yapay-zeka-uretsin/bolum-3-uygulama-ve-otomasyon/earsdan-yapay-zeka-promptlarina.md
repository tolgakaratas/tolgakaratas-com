---
title: "Bölüm 11: EARS'dan Yapay Zeka Prompt'larına: Otomasyon Köprüsü"
weight: 4
type: docs
summary: "Kitabımızın en sihirli anı. İnsan dilindeki net bir gereksinimi, bir yapay zekanın anlayacağı ve üzerine kod yazabileceği yapılandırılmış bir komuta (prompt'a) nasıl dönüştürürüz?"
tags: ["prompt engineering", "otomasyon", "AI", "json", "yapısal veri"]
---

[Seviye: İleri]

{{% callout warning %}}
**Anlatıcıdan Bir Not: Mühendis Şapkalarımızı Takalım**

Harika, şimdiye kadar konunun felsefesini ve insani yönünü konuştuk. Artık bir anlığına mühendis şapkalarımızı takma ve bu anlattıklarımızın bir makine için nasıl somut, matematiksel bir komuta dönüştüğünü görme zamanı. Burası, fikrin koda dönüştüğü sihirli atölye!
{{% /callout %}}

Şimdi kitabımızın en sihirli anına geldik. Şu ana kadar, insan olarak bizlerin anlayacağı, net ve temiz gereksinimler yazmayı öğrendik. Peki, bu insan dilindeki netliği, bir yapay zeka agent'inin anlayacağı ve üzerine kod yazabileceği somut bir komuta (prompt'a) nasıl dönüştürürüz?

### 11.1. Yapısal Dönüşüm: Neden Gerekli?

Bir AI agent, bir EARS cümlesini okuyup anlayabilse de, en verimli şekilde çalışması için "yapılandırılmış veriye" ihtiyaç duyar. Tıpkı bir aşçının, bir tarifin "bir tutam tuz" gibi belirsiz bir ifadesi yerine, "5 gram tuz" gibi net bir ölçüye ihtiyaç duyması gibi. EARS cümlesini, AI için bir JSON veya YAML dosyasına dönüştürmek, tüm belirsizlikleri ortadan kaldırır ve otomasyonun kapısını açar.

### 11.2. EARS Cümleciklerini Yapısal Veriye Dönüştürme Kuralları (Dönüşüm Mantığı)

EARS'ın güzelliği, kalıplarının bu dönüşüme mükemmel şekilde izin vermesidir. İşte temel haritalama:

| EARS Anahtar Kelimesi | Anlamı      | JSON Prompt Alanı                             | Açıklama                                                                    |
| :-------------------- | :---------- | :-------------------------------------------- | :-------------------------------------------------------------------------- |
| **`When`**            | Olay        | `trigger: { "type": "event", ... }`           | Sistemin tepki vermesine neden olan anlık olay.                             |
| **`While`**           | Durum       | `precondition: { "state": "...", ... }`       | Gereksinimin geçerli olması için sistemin içinde bulunması gereken durum.   |
| **`If... Then...`**   | Hata Durumu | `error_handling: { "condition": "...", ... }` | Normal akışın dışında, istenmeyen bir durum gerçekleştiğinde ne yapılacağı. |
| **Sistem Adı**        | Sorumlu     | `system_under_test: "..."`                    | Bu komutu yerine getirecek olan sistem veya bileşen.                        |
| **Sistem Tepkisi**    | Eylem       | `response: { "action": "...", ... }`          | Sistemin gerçekleştirmesi beklenen somut eylem.                             |

### 11.3. Tam Bir AI Prompt Örneği

Şimdi, basit bir EARS gereksinimini alıp tam teşekküllü bir AI prompt'una dönüştürelim.

- **EARS Gereksinimi:** `Eğer su seviyesi %10'un altına düşerse, o zaman Akıllı Kahve Makinesi, mobil uygulamaya 'su seviyesi kritik' bildirimi gönderecektir.`

- **AI Developer Agent için Zenginleştirilmiş Prompt (JSON):**

```json
{
  "taskId": "REQ-CM-042",
  "description": "Su seviyesi kritik olduğunda kullanıcıya bildirim gönderilmesi.",
  "requirement_source": "Eğer su seviyesi %10'un altına düşerse, o zaman Akıllı Kahve Makinesi, mobil uygulamaya 'su seviyesi kritik' bildirimi gönderecektir.",
  "handler": {
    "type": "error_handling",
    "condition": {
      "source": "su_seviyesi_sensoru",
      "metric": "su_yuzdesi",
      "operator": "<",
      "value": 10
    }
  },
  "system_under_test": "Akilli_Kahve_Makinesi",
  "response": {
    "action": "send_push_notification",
    "target_service": "Mobil_Uygulama_Api",
    "payload": {
      "user_id": "{aktif_kullanici_id}",
      "title": "Akıllı Kahve Makinesi",
      "message": "Su seviyesi kritik! Lütfen su haznesini doldurun.",
      "notification_type": "uyari"
    }
  },
  "technical_context": {
    "relevant_files": [
      "/services/SensorManager.js",
      "/services/NotificationService.js"
    ],
    "target_function_to_implement": "NotificationService.sendLowWaterAlert(userId)"
  },
  "acceptance_criteria_test": {
    "scenario": "Su seviyesi %9'a düştüğünde",
    "expected_result": "Mobil_Uygulama_Api'ye yukarıdaki payload ile bir POST isteği gönderildiğini doğrula."
  }
}
```

{{% callout note %}}
Bu yapısal prompt, AI agent'e sadece ne yapacağını değil, aynı zamanda bunu hangi dosyada, hangi fonksiyon içinde, hangi veriyle yapacağını ve sonucun nasıl test edileceğini de söyler. İşte bu, gerçek otomasyondur!
{{% /callout %}}

{{% callout note %}}
**Bu Bölümden Akılda Kalanlar**

- EARS gereksinimleri, AI agent'ler için yapılandırılmış prompt'lara dönüştürülmenin ilk adımıdır.
- Bu dönüşüm, EARS'ın anahtar kelimelerini (`When`, `While`, `If`) JSON gibi bir formatın alanlarına haritalayarak yapılır.
- En iyi prompt'lar, gereksinimin kendisine ek olarak, AI'ın işini kolaylaştıracak teknik bağlam (dosya adları, fonksiyonlar) ve test kriterleri de içerir.
  {{% /callout %}}

{{% callout note %}}
**Sıra Sizde! (Pratik Alıştırma)**

`"Kullanıcı 'temizle' düğmesine bastığında, Akıllı Kahve Makinesi, temizlik işlemini başlatacaktır."` EARS gereksinimini, yukarıdaki JSON formatına benzer şekilde basit bir yapıya dönüştürmeye çalışın. `trigger` alanını nasıl doldururdunuz? `response` alanı ne olurdu?
{{% /callout %}}
