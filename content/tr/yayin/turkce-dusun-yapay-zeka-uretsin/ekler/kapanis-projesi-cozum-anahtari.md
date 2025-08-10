---
title: "Ek F: Kapanış Projesi Çözüm Anahtarı"
weight: 6
type: docs
---

Bölüm 15'teki "Akıllı Sera" projesi için hazırladığımız örnek çözümler aşağıdadır. Unutmayın, bu tek doğru cevap değildir, sadece iyi bir yaklaşımdır. Sizin cevaplarınız farklı ama hala geçerli olabilir!

**Örnek EARS Gereksinimleri:**

1.  `Toprak nem sensörü, nem seviyesini %30'un altında ölçtüğünde, Akıllı Sera Sistemi, sulama vanasını 10 saniye süreyle açacaktır.`
2.  `Sıcaklık sensörü, sıcaklığı 5°C'nin altında ölçtüğünde, Akıllı Sera Sistemi, ısıtma lambasını yakacaktır.`
3.  `Isıtma lambası yanarken, sıcaklık sensörü sıcaklığı 10°C'nin üzerinde ölçtüğünde, Akıllı Sera Sistemi, ısıtma lambasını söndürecektir.`
4.  `Eğer su tankındaki seviye 'boş' ise, o zaman Akıllı Sera Sistemi, sulama vanasını açmayacaktır.`
5.  `Eğer su tankındaki seviye 'boş' ise, o zaman Akıllı Sera Sistemi, kullanıcıya 'su tankı boş' bildirimi gönderecektir.`

**Örnek Permütatif Test Senaryosu:**

- **Adı:** `TEST_SULAMA_P_004: Toprak Kuru, Bitki Domates, Su Tankı Dolu`
- **Değişkenler:** Toprak Nemi (`Çok Islak`, `Nemli`, `Kuru`), Bitki Türü (`Domates`, `Salatalık`, `Biber`), Su Tankı Seviyesi (`Dolu`, `Az`, `Boş`).

**Örnek AI Prompt (JSON):**

```json
{
  "taskId": "REQ-SERA-001",
  "requirement_source": "Toprak nem sensörü, nem seviyesini %30'un altında ölçtüğünde, Akıllı Sera Sistemi, sulama vanasını 10 saniye süreyle açacaktır.",
  "trigger": {
    "type": "event",
    "source": "toprak_nem_sensoru",
    "condition": {
      "metric": "nem_yuzdesi",
      "operator": "<",
      "value": 30
    }
  },
  "system_under_test": "Akilli_Sera_Sistemi",
  "response": {
    "action": "open_valve",
    "target": "sulama_vanasi",
    "parameters": {
      "duration_seconds": 10
    }
  },
  "acceptance_criteria_test": {
    "scenario": "Toprak nemi %29 olarak ölçüldüğünde",
    "expected_result": "Sulama vanasına 10 saniye boyunca 'açık' sinyali gönderildiğini doğrula."
  }
}
```
