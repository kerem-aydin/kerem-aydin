## Kerem Aydın

İşletmelerin kaçırdığı talebi karşılayan randevu asistanları yazıyorum:
web sitesine ve telefona gelen isteği alan, müsait saati **işletmenin kendi
takviminden doğrulayan** ve randevuyu oraya yazan sistemler.

Şu an **[Veluxo AI](https://veluxoai.com)** üzerinde çalışıyorum. Yazılı kanal
ve telefon resepsiyonu, tek takvim.

---

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

---

### Açık depolar

| Depo | Ne işe yarar |
|---|---|
| **[randevu-widget](https://github.com/BruceWayne2122/randevu-widget)** | Herhangi bir siteye tek script etiketiyle eklenen randevu kutusu. Bağımlılık yok, Shadow DOM içinde çalışır, saat dilimini işletmenin saatiyle hesaplar. |
| **[tr-dogrulama](https://github.com/BruceWayne2122/tr-dogrulama)** | Türk işletme verisiyle çalışırken defalarca yeniden yazılan küçük şeyler: Türkçe duyarlı küçültme, telefon (444'lü hatlar dahil), kurumsal rol e-postası ayrımı, TCKN, VKN, IBAN. |

İkisi de bağımlılıksız, ikisi de testli.

---

### Kullandıklarım

TypeScript · Next.js · React · Node.js · Python · n8n · Google Calendar API ·
OpenAI · ElevenLabs

---

Matematik okuyorum. Freelance iş alıyorum: randevu widget'ı kurulumu, tek
sayfa tanıtım sitesi, kurumsal site.
