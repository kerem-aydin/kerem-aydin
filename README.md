## Kerem Aydın

I build automation systems for small businesses, and the checks that prove
they still work tomorrow.

Right now that is **[Veluxo AI](https://veluxoai.com)**: a written-channel
receptionist for appointment-based businesses. A message arrives on Instagram
or WhatsApp, the assistant answers it, checks a real free slot, and writes the
booking into the business's own panel. I designed, built and shipped it alone.

---

### What I have shipped

**Veluxo AI** · live product, solo
- Instagram DM and WhatsApp Cloud API channels behind one signature-checked
  webhook.
- A booking engine that writes only after the slot is confirmed free, so two
  conversations cannot take the same hour.
- A multi-tenant business panel: inbox, calendar, conversation history,
  onboarding.
- About 470 automated tests across the channel, booking and panel code.
- Next.js 16 · React 19 · TypeScript · Supabase (Postgres) · OpenAI · Vercel.
- 770+ commits since July 2026.

**An automation fleet that watches itself**
- **Night watch:** every night a real browser opens the live site as a phone
  and as a desktop, scrolls every page to the bottom, and reports anything that
  broke without an error: an invisible section, horizontal overflow, a broken
  image, a slow page. Before each run it puts a known bug back on purpose and
  fails if it cannot catch it.
- **Problem radar:** every Monday it reads public complaints (Hacker News,
  1-2 star App Store reviews), clusters them, counts distinct people, and sends
  the five problems people pay for but are unhappy with.
- **Cockpit:** one screen for all of the above. Each automation is drawn as a
  flow diagram and lights up step by step while it runs.

---

### How I work

**Whatever the model says, what is actually in the book?**
A language model's output is a claim. "Your appointment is confirmed" can only
be sent after the calendar has accepted it.

**Whose clock is this?**
`new Date("2026-09-10T14:00")` reads as Berlin in a visitor's browser and as
UTC on the server. Both are wrong, and the bug shows up as "my appointment
moved by an hour".

**Is this measurement measuring anything?**
A green test suite can be testing the wrong layer. The footer of my own site
was blank on phones: no error, no failing test. A layout change after
load had pushed the scroll triggers below the end of the page. I found it by
measuring what a phone actually shows, and the night watch now checks for
that class of bug every night.

---

### Open repositories

| Repository | What it does |
|---|---|
| **[randevu-widget](https://github.com/kerem-aydin/randevu-widget)** | A booking box you add to any site with one script tag. No dependencies, runs inside a Shadow DOM, computes slots in the business's own time zone. [Live demo](https://kerem-aydin.github.io/randevu-widget/demo/) |
| **[tr-dogrulama](https://github.com/kerem-aydin/tr-dogrulama)** | The small things you rewrite every time you work with Turkish business data: Turkish-aware lowercasing, phone numbers (including 444 lines), corporate vs. personal email, national ID, tax number, IBAN. |

Both dependency-free, both tested.

### Tools

TypeScript · Next.js · React · Node.js · Python · Supabase / Postgres ·
Meta Graph API (Instagram, WhatsApp) · OpenAI · GitHub Actions · Vercel ·
Puppeteer

I study mathematics in Türkiye. Open to collaborations and projects:
[veluxoai.com](https://veluxoai.com) · [LinkedIn](https://www.linkedin.com/in/kerem-aydin-a124a0420)

---
---

## Türkçe

Küçük işletmeler için otomasyon sistemleri kuruyorum ve bu sistemlerin yarın
da çalıştığını kanıtlayan denetimleri.

Şu an bu **[Veluxo AI](https://veluxoai.com)**: randevuyla çalışan işletmeler
için yazılı kanal resepsiyonu. Instagram'a ya da WhatsApp'a bir mesaj gelir,
asistan cevaplar, gerçekten boş bir saati doğrular ve randevuyu işletmenin
kendi paneline yazar. Tek başıma tasarladım, yazdım ve yayına aldım.

### Yayına aldıklarım

**Veluxo AI** · canlı ürün, tek kişi
- Resmî Meta API'leri üzerinde Instagram DM ve WhatsApp kanalları; imza
  denetimli tek bir webhook.
- Saat gerçekten boş olduğu doğrulanmadan yazmayan bir randevu motoru; iki
  konuşma aynı saati alamaz.
- Çok kiracılı işletme paneli: gelen kutusu, takvim, konuşma geçmişi, kurulum.
- Kanal, randevu ve panel kodunda yaklaşık 470 otomatik test.
- Temmuz 2026'dan beri 770'ten fazla commit.

**Kendi kendini denetleyen otomasyonlar**
- **Gece bekçisi:** her gece gerçek bir tarayıcı canlı siteyi telefon ve
  bilgisayar gibi açar, her sayfayı dibine kadar kaydırır; hata vermeden bozulan
  şeyleri bildirir: görünmeyen bölüm, yana taşma, kırık resim, yavaş sayfa. Her
  koşudan önce bilinen bir hatayı bilerek geri koyar; yakalayamazsa kendini
  bozuk sayar.
- **Problem radarı:** her pazartesi herkese açık şikâyetleri okur (Hacker News,
  App Store'da 1-2 yıldızlı yorumlar), kümeler, ayrı kişileri sayar ve insanların
  para ödediği ama memnun olmadığı beş sorunu getirir.
- **Kokpit:** hepsi tek ekranda. Her otomasyon bir akış şeması olarak çizilir,
  çalışırken adım adım yanar.

### Nasıl çalışıyorum

**Model ne söylerse söylesin, defterde ne var?**
Bir dil modelinin çıktısı bir iddiadır. "Randevunuz oluşturuldu" ancak takvim
kabul ettikten sonra söylenebilir.

**Saat kimin saati?**
`new Date("2026-09-10T14:00")` ziyaretçinin tarayıcısında Berlin, sunucuda UTC
okunur. İkisi de yanlıştır ve hata "randevum bir saat kaymış" diye ortaya çıkar.

**Bu ölçüm gerçekten ölçüyor mu?**
Yeşil bir test suiti yanlış katmanı ölçüyor olabilir. Kendi sitemin footer'ı
telefonda boş kalıyordu: hata yok, düşen test yok. Açılıştan sonraki bir
yerleşim değişikliği, kaydırma tetiklerini sayfanın sonunun altına itmişti.
Telefonun gerçekte ne gösterdiğini ölçerek buldum; gece bekçisi artık bu hata
sınıfını her gece arıyor.

### Açık depolar

| Depo | Ne işe yarar |
|---|---|
| **[randevu-widget](https://github.com/kerem-aydin/randevu-widget)** | Herhangi bir siteye tek script etiketiyle eklenen randevu kutusu. Bağımlılık yok, Shadow DOM içinde çalışır, saat dilimini işletmenin saatiyle hesaplar. [Canlı demo](https://kerem-aydin.github.io/randevu-widget/demo/) |
| **[tr-dogrulama](https://github.com/kerem-aydin/tr-dogrulama)** | Türk işletme verisiyle çalışırken defalarca yeniden yazılan küçük şeyler: Türkçe duyarlı küçültme, telefon (444'lü hatlar dahil), kurumsal rol e-postası ayrımı, TCKN, VKN, IBAN. |

İkisi de bağımlılıksız, ikisi de testli.

Türkiye'de matematik okuyorum. İş birliklerine ve projelere açığım.
