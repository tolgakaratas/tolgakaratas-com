---
title: "Bölüm 4: Günlük Dilin Belirsizlikleri ve Makine Mantığı"
weight: 5
type: docs
summary: "İnsanların kolayca anladığı ama makinelerin kafasını karıştıran 'hızlı', 'kolay', 'uygun' gibi kelimelerin tehlikelerini ve bu tuzaklardan nasıl kaçınacağımızı öğrenin."
tags: ["belirsizlik", "doğal dil", "AI mantığı", "anti-pattern"]
---

[Seviye: Temel]

İnsanlar olarak bizler, cümlelerdeki boşlukları tecrübelerimizle ve varsayımlarımızla doldurmakta ustayızdır. Ancak bir makine veya AI agent için her şey siyah ve beyazdır. Bir komut ya nettir ya da değildir. Bu bölümde, gereksinim yazarken kaçınmamız gereken ve makineler için "zehirli" olan belirsizlik türlerini inceleyeceğiz.

### 4.1. Muğlaklık (Ambiguity): "Kullanıcı Dostu" Ne Demek?

Bir kelimenin birden fazla anlama gelebilmesidir.

- **Belirsiz Cümle:** "Sistem, kullanıcı için uygun bir tema sunmalıdır."
- **Problem:** "Uygun" kelimesi tamamen subjektiftir. Bir kullanıcı için "koyu tema" uygunken, diğeri için "yüksek kontrastlı tema" uygun olabilir. Bir AI agent, bu iki seçenekten hangisini seçeceğini bilemez.
- **Net Gereksinim:** "Kullanıcı 'Ayarlar' menüsünden 'Koyu Tema' seçeneğini seçtiğinde, sistem arayüzünü koyu tema renk paletine göre güncelleyecektir."

### 4.2. Belirsizlik (Vagueness): "Hızlı" Ne Kadar Hızlı?

Ölçülemeyen sıfatlar kullanmaktır.

- **Belirsiz Cümle:** "Arama sonuçları hızlı bir şekilde görüntülenmelidir."
- **Problem:** "Hızlı" kelimesi kişiden kişiye değişir. Bir saniye mi, yarım saniye mi? Bir AI, bu hedefi test edemez.
- **Net Gereksinim:** "Kullanıcı arama yaptığında, sistem arama sonuçlarını 500 milisaniyeden daha az bir sürede görüntüleyecektir."

### 4.3. Eksiklik (Incompleteness): "Peki Ya İnternet Giderse?"

Bir senaryonun tüm olasılıklarını kapsamamak, varsayımlarda bulunmaktır.

- **Eksik Cümle:** "Uygulama, kullanıcının yazdığı notu buluta kaydeder."
- **Problem:** Bu cümle, her zaman internet bağlantısı olduğunu varsayar. Peki ya bağlantı yoksa ne olacak? Not kaybolacak mı? AI bu durumu yönetmek için bir kurala ihtiyaç duyar.
- **Net Gereksinim Seti:**
  1.  "Kullanıcı bir notu kaydettiğinde ve internet bağlantısı varken, sistem notu buluta kaydedecektir."
  2.  "Kullanıcı bir notu kaydettiğinde ve internet bağlantısı yokken, sistem notu geçici olarak cihaz hafızasına kaydedecektir."
  3.  "İnternet bağlantısı geri geldiğinde, sistem cihaz hafızasındaki tüm kaydedilmiş notları bulut ile senkronize edecektir."

Bu basit kuralları en başta koyarak, projenin ilerleyen aşamalarında ortaya çıkacak büyük baş ağrılarının ve hataların önüne geçmiş oluruz.

{{% callout note %}}
**Bu Bölümden Akılda Kalanlar**

- AI agent'ler varsayım yapmaz, sadece net komutları uygular.
- "Uygun, kolay, hızlı, etkili" gibi ölçülemeyen sıfatlardan kaçının. Her zaman ölçülebilir hedefler koyun.
- Her senaryo için sadece "olması gerekeni" değil, "ya olmazsa" durumunu da düşünün.
  {{% /callout %}}

{{% callout note %}}
**Sıra Sizde! (Pratik Alıştırma)**

Aşağıdaki belirsiz cümleyi, ölçülebilir ve eksiksiz bir EARS gereksinimine dönüştürmeye çalışın: "Akıllı Kahve Makinesi, kahveyi yeterince sıcak tutmalıdır." (İpucu: "Yeterince sıcak" ne demek? "Ne kadar süreyle?")
{{% /callout %}}
