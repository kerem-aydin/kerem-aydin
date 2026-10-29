## Kerem Aydın

Mathematics student at Sakarya University. I design and build **websites,
dashboards, AI agents and automations**, and the checks that prove they still
work tomorrow. I work alone, with agents doing much of the routine work.

**Open for freelance work:** websites · admin panels and dashboards · workflow
automation (n8n, Make, Telegram bots, AI agents).

---

### Selected project

**[Veluxo AI](https://veluxoai.com)** · built alone, July–October 2026

A written-channel receptionist for appointment-based businesses. A message
arrives on Instagram or WhatsApp, the assistant answers it, checks a real free
slot, and writes the booking into the business's own panel.

- Designed and built end to end: marketing site, onboarding, multi-tenant
  business panel (inbox, calendar, conversation history).
- Instagram DM and WhatsApp Cloud API behind one signature-checked webhook.
- A booking engine that writes only after the slot is confirmed free.
- A voice agent prototype that answers the phone and books into the same calendar.
- 340+ automated tests · 670+ commits since July 2026.
- Next.js · React · TypeScript · Supabase (Postgres) · OpenAI · Vercel.

<p>
  <a href="https://veluxoai.com"><img src="assets/veluxo-desktop.jpg" alt="Veluxo AI home page on desktop" width="620"></a>
  <a href="https://veluxoai.com"><img src="assets/veluxo-phone.jpg" alt="Veluxo AI home page on a phone" width="178"></a>
</p>
<sub>Site and panel designed and built by me. The panel shown on the home page uses sample data.</sub>

### Systems I run for myself

Private code, real use. About 1,400 commits across my private repositories in the last year.

| System | What it does |
|---|---|
| **Cockpit** | One dashboard for everything below. Each automation is drawn as a flow diagram that lights up step by step while it runs. |
| **Telegram team** | Bots that send a short morning plan, ask for decisions with buttons and report when something breaks. |
| **Night watch** | Opens the live site every night as a phone and a desktop and reports what broke without an error. Open-sourced as [gece-bekcisi](https://github.com/kerem-aydin/gece-bekcisi). |
| **Research lines** | Coding agents read public sources in five audited stages to find problems people actually pay for. Method open-sourced as [kanitli-arastirma](https://github.com/kerem-aydin/kanitli-arastirma). |
| **Problem radar** | Collects public complaints and reviews, clusters them, counts distinct people. |
| **Job hunter** | Finds small paid automation jobs on public boards and scores them with explicit rules, no model. |
| **Weekly report** | Every Sunday, what was actually built that week, from GitHub and the task list. |
| **Usage guard** | Keeps background agents within limits so the owner always has room to work. Part of [ajan-ofisi](https://github.com/kerem-aydin/ajan-ofisi). |

### Design

I design what I build: the Veluxo site and panel, the cockpit, and a browser
driving game with a procedural, seed-based world and engine sound synthesized
with the Web Audio API (three.js).

### Open source

| Repository | What it does |
|---|---|
| **[gece-bekcisi](https://github.com/kerem-aydin/gece-bekcisi)** | Night watch for websites. A real browser scrolls specified pages as a slow phone and a desktop, reports invisible headings and footers, sideways scroll, broken images, slow pages. Includes a nightly workflow example that checks a deliberately hidden footer first. |
| **[kanitli-arastirma](https://github.com/kerem-aydin/kanitli-arastirma)** | Evidence-first research run by coding agents: separate stages, an adversarial audit by an agent that did not write the work, code-checked rules for what counts as proof that people pay. |
| **[ajan-ofisi](https://github.com/kerem-aydin/ajan-ofisi)** | A one-person office on Telegram: morning plan from a Markdown task list, a decision box with buttons, a usage guard for background agents. |
| **[randevu-widget](https://github.com/kerem-aydin/randevu-widget)** | A booking widget for any site with one script tag. Shadow DOM, slots in the business's own time zone. [Live demo](https://kerem-aydin.github.io/randevu-widget/demo/) |
| **[tr-dogrulama](https://github.com/kerem-aydin/tr-dogrulama)** | Validation for Turkish business data: phone numbers, national ID, tax number, IBAN, role vs. personal email. |
| **[n8n-workflows](https://github.com/kerem-aydin/n8n-workflows)** | Five n8n workflows from my own instance: a demo-clinic booking assistant, WhatsApp messaging, reminders and more, cleaned for reuse. |
| **[sales-collection-dashboard](https://github.com/kerem-aydin/sales-collection-dashboard)** | A Turkish Excel template for monthly sales and bank collections across provinces: bank lines matched to customers, a month selector, summary cards and a native chart. No macros; fictional sample data. |

The five code repositories run their tests on every push, with at most one dependency each. The Excel template is rebuilt from code and checked on every push.

### How I work

- **A model's output is a claim.** "Your appointment is confirmed" is sent only after the calendar has accepted it.
- **Measure what the user sees.** My site's footer was blank on phones with every test green. The night watch exists because of that.
- **Proof before building.** A complaint count is not proof that anyone pays; my research rules say what is.

### Now · October 2026

- Open for freelance work: dashboards and internal tools, websites, workflow automation.
- Building website templates for real-estate offices and dashboards for small businesses.
- Finished six research lines on where AI solves problems people pay for.

TypeScript · JavaScript · Python · Next.js · React · Node.js · Supabase / Postgres ·
Meta Graph API · OpenAI · n8n · Make · GitHub Actions · Vercel · Puppeteer · three.js

[veluxoai.com](https://veluxoai.com) · [LinkedIn](https://www.linkedin.com/in/kerem-aydin-ai)

---

<details>
<summary><b>Türkçe</b></summary>

Sakarya Üniversitesi'nde matematik okuyorum. **Web sitesi, panel, yapay zekâ
ajanları ve otomasyonlar** tasarlayıp kuruyorum; bunların yarın da çalıştığını
kanıtlayan denetimleri de. Tek başıma çalışıyorum; rutin işin çoğunu ajanlar
yapıyor.

**Serbest işlere açığım:** web sitesi · yönetim paneli · iş akışı otomasyonu
(n8n, Make, Telegram botları, yapay zekâ ajanları).

- **Öne çıkan proje:** [Veluxo AI](https://veluxoai.com), randevuyla çalışan işletmeler için
  Instagram ve WhatsApp'tan cevap veren, gerçekten boş saati doğrulayıp randevuyu
  işletmenin paneline yazan resepsiyon. Site, panel ve kanallar dahil uçtan uca tek başıma tasarlayıp
  kurdum (Temmuz–Ekim 2026).
- **Kendim için çalıştırdığım sistemler:** kokpit paneli, Telegram ekibi, gece
  bekçisi, araştırma hatları, problem radarı, iş avcısı, haftalık rapor,
  kullanım bekçisi. Gizli depolarımda son bir yılda yaklaşık 1.400 commit.
- **Açık depolar:** gece-bekcisi, kanitli-arastirma, ajan-ofisi,
  randevu-widget, tr-dogrulama, n8n-workflows, sales-collection-dashboard (Excel satış ve tahsilat paneli).

İş birliklerine ve projelere açığım.

</details>
