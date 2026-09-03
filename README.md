## Kerem Aydın

I build appointment assistants that catch the demand a business misses:
systems that take the request coming from a website or a phone call, check a
free slot **against the business's own calendar**, and write the booking into
it.

Currently working on **[Veluxo AI](https://veluxoai.com)** — written channels
and phone reception, one calendar.

---

### Most of my work comes down to three questions

**Whatever the model says, what is actually in the book?**
A language model's output is a claim. The sentence "your appointment is
confirmed" can only be written after the calendar has actually accepted it.
Any system that leaves that gap open ends with somebody showing up for
nothing.

**Whose clock is this?**
`new Date("2026-09-10T14:00")` reads as Berlin in a visitor's browser and as
UTC on the server. Both are wrong, and the bug surfaces as "the appointment
moved by an hour" on the first complaint.

**Is this measurement measuring anything?**
A green test suite may be testing the wrong layer. Once, an end-to-end exam I
trusted was never calling my own endpoint at all.

---

### Open repositories

| Repository | What it does |
|---|---|
| **[randevu-widget](https://github.com/BruceWayne2122/randevu-widget)** | A booking box you add to any site with one script tag. No dependencies, runs inside a Shadow DOM, computes slots in the business's own time zone. [Live demo](https://brucewayne2122.github.io/randevu-widget/demo/) |
| **[tr-dogrulama](https://github.com/BruceWayne2122/tr-dogrulama)** | The small things you rewrite every time you work with Turkish business data: Turkish-aware lowercasing, phone numbers (including 444 lines), corporate vs. personal email, national ID, tax number, IBAN. |

Both dependency-free, both tested.

### Tools

TypeScript · Next.js · React · Node.js · Python · n8n · Google Calendar API ·
OpenAI · ElevenLabs

I study mathematics. Available for freelance work: booking widget setup,
one page sites, corporate websites.

---
---

## Türkçe

İşletmelerin kaçırdığı talebi karşılayan randevu asistanları yazıyorum:
web sitesine ve telefona gelen isteği alan, müsait saati **işletmenin kendi
takviminden doğrulayan** ve randevuyu oraya yazan sistemler.

Şu an **[Veluxo AI](https://veluxoai.com)** üzerinde çalışıyorum. Yazılı kanal
ve telefon resepsiyonu, tek takvim.

### Yaptığım işin çoğu şu üç soruya iniyor

**Model ne söylerse söylesin, defterde ne var?**
Bir dil modelinin çıktısı bir iddiadır. "Randevunuz oluşturuldu" cümlesi ancak
takvim gerçekten yazdıktan sonra kurulabilir. Aradaki farkı kapatmayan her
sistem, birinin boşuna gelmesiyle biter.

**Saat kimin saati?**
`new Date("2026-09-10T14:00")` ziyaretçinin tarayıcısında Berlin, sunucuda UTC
okunur. İkisi de yanlıştır ve hata "randevu bir saat kaymış" diye, ilk
şikayette ortaya çıkar.

**Bu ölçüm gerçekten ölçüyor mu?**
Yeşil bir test suiti yanlış katmanı ölçüyor olabilir. Bir defa, uçtan uca
geçtiğini sandığım bir sınav aslında kendi uç noktamı hiç çağırmıyordu.

### Açık depolar

| Depo | Ne işe yarar |
|---|---|
| **[randevu-widget](https://github.com/BruceWayne2122/randevu-widget)** | Herhangi bir siteye tek script etiketiyle eklenen randevu kutusu. Bağımlılık yok, Shadow DOM içinde çalışır, saat dilimini işletmenin saatiyle hesaplar. [Canlı demo](https://brucewayne2122.github.io/randevu-widget/demo/) |
| **[tr-dogrulama](https://github.com/BruceWayne2122/tr-dogrulama)** | Türk işletme verisiyle çalışırken defalarca yeniden yazılan küçük şeyler: Türkçe duyarlı küçültme, telefon (444'lü hatlar dahil), kurumsal rol e-postası ayrımı, TCKN, VKN, IBAN. |

İkisi de bağımlılıksız, ikisi de testli.

Matematik okuyorum. Freelance iş alıyorum: randevu widget'ı kurulumu, tek
sayfa tanıtım sitesi, kurumsal site.
