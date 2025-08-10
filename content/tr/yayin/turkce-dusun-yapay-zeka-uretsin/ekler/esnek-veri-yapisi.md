---
title: "Ek E: Esnek Veri Yapısı ve Geleceğe Uyumluluk"
weight: 5
type: docs
---

Bu kitabın AI eğitimi için maksimum esneklik sağlaması hedeflenmiştir. Metin içindeki yapısal bilgiler (kurallar, örnekler, anti-pattern'ler), ileride farklı AI modellerinin ihtiyaç duyabileceği herhangi bir formata (JSON, YAML, XML vb.) kolayca dönüştürülebilir. Bu, metin içine yerleştirilmiş, makine tarafından okunabilir yorum etiketleri (``) aracılığıyla yapılır.

**Örnek Python Script Felsefesi:**

Aşağıdaki pseudo-kod, bu etiketlerin nasıl okunup yapısal bir JSON'a dönüştürülebileceğini göstermektedir:

```python
# Pseudo-kod
import re
from typing import List, Dict

def parse_book_text_to_structured_data(text: str) -> List[Dict]:
    """
    Kitap metnindeki özel etiketleri okur ve yapısal veri listesi döndürür.
    Bu, konsepti gösteren basitleştirilmiş bir örnektir.
    """

    # # Eğer su seviyesi %10'un altına düşerse, o zaman Akıllı Kahve Makinesi, mobil uygulamaya 'su seviyesi kritik' bildirimi gönderecektir.

    pattern = re.compile(r'\n(?P<text>.*)', re.MULTILINE)

    found_items = []
    for match in pattern.finditer(text):
        data = match.groupdict()
        item = {
            'id': data['id'].strip(),
            'pattern_type': data['pattern'].strip(),
            'system_name': data['system'].strip(),
            'text': data['text'].strip()
        }
        found_items.append(item)

    return found_items

# Örnek Kullanım
kitap_metni = """
Eğer su seviyesi %10'un altına düşerse, o zaman Akıllı Kahve Makinesi, mobil uygulamaya 'su seviyesi kritik' bildirimi gönderecektir.
"""

parsed_data = parse_book_to_structured_data(kitap_metni)
# parsed_data şimdi JSON'a veya başka bir formata kolayca çevrilebilir.
print(parsed_data)
```

Bu yaklaşım, kitabın içeriğini gelecekteki teknolojik değişimlere karşı dirençli kılar.

```

```
