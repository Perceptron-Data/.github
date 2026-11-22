<p align="center"><img src="https://perceptron-data.github.io/assets/logo-256.png" width="88" alt="Perceptron Data"></p>
<h2 align="center">Check, don't guess.</h2>
<p align="center">Company checks and data from public sources, as <a href="https://apify.com/perceptr0n">Apify</a> actors. Built in Germany. Focused on DACH and the EU.<br><a href="https://perceptron-data.github.io/">Website</a> · <a href="https://perceptron-data.github.io/de/">Deutsch</a> · <a href="https://perceptron-data.github.io/quality/">Weekly checks</a> · <a href="https://apify.com/perceptr0n">All actors on Apify</a></p>

Paste website domains and get the company behind each one: legal name, register number and VAT number, checked live against the EU's VIES register. Ask a question and get cited passages with an evidence level for your LLM. Every row says where its data came from. Paid per result, plus a small start fee per run.

**Measured, not promised:** 8 of 9 websites that refused automated requests or needed JavaScript came back complete, with a VIES-valid VAT number (Imprint & VAT Check · Apify platform test, 13 Oct 2026) · 10 of 10 published research questions gave the known answer in the weekly check (Research Agent · 12 Oct 2026) · 164 field values compared one by one with the original source: 136 matched (82.9%) (Imprint & VAT Check · sample, 12 Oct 2026)

**For AI agents:** every actor is a tool on Apify's MCP server — `https://mcp.apify.com?tools=perceptr0n/imprint-impressum-website-contact-scraper,perceptr0n/research-agent` · [setup for Claude Code, Cursor and the API](https://perceptron-data.github.io/agents/)

## Company checks

Two checks for lists of companies, with a traceable answer per company.

| | Actor | What you get | Price (Apify free plan) |
|---|---|---|---|
| <img src="https://perceptron-data.github.io/assets/icons/ads-transparency-256.png" width="32" alt=""> | [Advertiser Check (Google & Bing)](https://perceptron-data.github.io/actors/google-ads-transparency-scraper/) | Company list in, one row per company out: Google ads, Bing ads, ad counts, accounts – for domains, Bing matches proven by landing pages. | $4.00 per 1,000 companies checked (from $2.50) + $0.01 start fee per run |
| <img src="https://perceptron-data.github.io/assets/icons/impressum-256.png" width="32" alt=""> | [Imprint & VAT Check](https://perceptron-data.github.io/actors/imprint-impressum-website-contact-scraper/) | Domains in, company rows out: legal name, address, register number and EU VAT ID checked against VIES – from the Impressum. | $5.00 per 1,000 websites (from $2.50) + $0.01 start fee per run |
| <img src="https://perceptron-data.github.io/assets/icons/impressum-256.png" width="32" alt=""> | [Free Imprint & Contact Check](https://perceptron-data.github.io/actors/free-website-contact-imprint-scraper/) | Free: the same company row as the paid check – EU VAT ID checked against VIES, email, phone – for up to 10 websites per run. | Free |

## More data from public sources

Each actor reads public sources – or your own documents – and returns one row per record.

### Ads & Apps

App ratings, versions and App Store reviews from both stores in one table.

| | Actor | What you get | Price (Apify free plan) |
|---|---|---|---|
| <img src="https://perceptron-data.github.io/assets/icons/appstores-256.png" width="32" alt=""> | [App Store & Google Play Data](https://perceptron-data.github.io/actors/appstore-google-play-intelligence/) | App IDs or App Store keywords in, one row per app out – shared fields for App Store and Google Play, plus App Store reviews. | $1.00 per 1,000 apps (from $0.50) + $0.01 start fee per run |

### Hiring & Trade Fairs

Who is hiring in Germany, how employees rate employers, who exhibits in Munich and Cologne.

| | Actor | What you get | Price (Apify free plan) |
|---|---|---|---|
| <img src="https://perceptron-data.github.io/assets/icons/arbeitsagentur-256.png" width="32" alt=""> | [Arbeitsagentur Jobs](https://perceptron-data.github.io/actors/arbeitsagentur-jobs-scraper/) | Keyword and place in, one row per job out: employer, salary range, home office, location – who is hiring in Germany. | $1.00 per 1,000 jobs (from $0.50) + $0.01 start fee per run |
| <img src="https://perceptron-data.github.io/assets/icons/logo-256.png" width="32" alt=""> | [XING Jobs](https://perceptron-data.github.io/actors/xing-jobs-scraper/) | Keyword and place in, one row per job out: company, salary with its source, career level, full text – DACH jobs from XING. | $1.00 per 1,000 jobs (from $0.50) + $0.00005 start fee per run |
| <img src="https://perceptron-data.github.io/assets/icons/kununu-256.png" width="32" alt=""> | [kununu Employer Data](https://perceptron-data.github.io/actors/kununu-employer-data-scraper/) | kununu profiles in, one row per employer out: score vs. industry, salary ranges of top job titles, benefits and reviews. | $1.00 per 1,000 records (from $0.50) + $0.04 start fee per run |
| <img src="https://perceptron-data.github.io/assets/icons/messe-muenchen-256.png" width="32" alt=""> | [Messe München Exhibitors](https://perceptron-data.github.io/actors/messe-muenchen-exhibitor-list-scraper/) | Exhibitor directory in, one row per exhibitor out: stand, address, phone, website, product groups – who exhibits in Munich. | $5.00 per 1,000 exhibitors (from $2.50) + $0.01 start fee per run |
| <img src="https://perceptron-data.github.io/assets/icons/koelnmesse-256.png" width="32" alt=""> | [Koelnmesse Exhibitors](https://perceptron-data.github.io/actors/anuga-ism-koelnmesse-exhibitor-scraper/) | Exhibitor list in, one row per exhibitor out: hall and stand, contacts, brands and product categories – who exhibits in Cologne. | $5.00 per 1,000 exhibitors (from $2.50) + $0.01 start fee per run |

### Registers

Insolvency and register notices for German companies, EU tenders and German power plants – from public registers.

| | Actor | What you get | Price (Apify free plan) |
|---|---|---|---|
| <img src="https://perceptron-data.github.io/assets/icons/insolvency-monitor-256.png" width="32" alt=""> | [Insolvency & Handelsregister Monitor](https://perceptron-data.github.io/actors/german-insolvency-handelsregister-monitor/) | Company list in, one row per German company out: insolvency and register notices, EU VAT ID check, open positions – or only what changed. | $20.00 per 1,000 company rows (from $10.00) + $0.00005 start fee per run |
| <img src="https://perceptron-data.github.io/assets/icons/ted-256.png" width="32" alt=""> | [TED Tenders](https://perceptron-data.github.io/actors/eu-tenders-ted-scraper/) | Countries and CPV codes in, one row per notice out: buyer, value, deadline and award winner – who wins public contracts. | $2.00 per 1,000 tenders (from $1.00) + $0.01 start fee per run |
| <img src="https://perceptron-data.github.io/assets/icons/mastr-256.png" width="32" alt=""> | [MaStR Energy Assets](https://perceptron-data.github.io/actors/german-energy-assets-mastr/) | Filters in, one row per plant out: operator, capacity, commissioning date, grid operator – who operates energy assets in Germany. | $4.00 per 1,000 units (from $2.00) + $0.04 start fee per run |
| <img src="https://perceptron-data.github.io/assets/icons/eudamed-256.png" width="32" alt=""> | [EUDAMED Medical Devices](https://perceptron-data.github.io/actors/eudamed-medical-device-scraper/) | Filters in, one row per device, manufacturer or certificate out – who makes which medical devices in the EU. | $30.00 per 1,000 records (from $15.00) + $0.02 start fee per run |

### Documents

PDF, Word, Excel and PowerPoint to Markdown – tables as Markdown and JSON rows, OCR for scans.

| | Actor | What you get | Price (Apify free plan) |
|---|---|---|---|
| <img src="https://perceptron-data.github.io/assets/icons/doc-markdown-256.png" width="32" alt=""> | [PDF to Markdown](https://perceptron-data.github.io/actors/pdf-to-markdown-converter/) | Files in, Markdown out – tables as Markdown and JSON rows, OCR for scans, RAG chunks with page numbers. No LLM involved. | $0.50 per 1,000 pages (from $0.35) + $0.005 start fee per run |

### Research for AI

Cited passages from the web, EU and German legal texts and open research for AI agents and RAG, with an evidence level for every source.

| | Actor | What you get | Price (Apify free plan) |
|---|---|---|---|
| <img src="https://perceptron-data.github.io/assets/icons/research-agent-256.png" width="32" alt=""> | [Research Agent](https://perceptron-data.github.io/actors/research-agent/) | A question in, ranked passages out – each with its source and an evidence level; EU and German law texts included. | $15.00 per 1,000 questions + $0.00005 start fee per run |

### Tools

Merge datasets and remove duplicates – or let the free finder name the actor that fits, with fields and run cost.

| | Actor | What you get | Price (Apify free plan) |
|---|---|---|---|
| <img src="https://perceptron-data.github.io/assets/icons/dataset-merge-dedupe-256.png" width="32" alt=""> | [Dataset Merge & Company Dedupe](https://perceptron-data.github.io/actors/merge-dedupe-datasets-company-leads/) | Datasets, files or rows in, one merged dataset without duplicates out – for lead lists one row per company, with the reason for every merge. | $0.30 per 1,000 rows in merge or dedupe mode (from $0.20) + $0.00005 start fee per run |
| <img src="https://perceptron-data.github.io/assets/icons/finder-256.png" width="32" alt=""> | [Data Source Finder](https://perceptron-data.github.io/actors/dach-eu-data-source-finder/) | A source in, the matching actor out – with fields, record count and run cost. Free. | Free |

## Custom Actors

Need a source that is not in the catalogue, extra fields or a different delivery? Perceptron Data also builds actors to order. Write to thom.ehr@gmail.com with the source and the data you need, or open an issue on the Apify page of one of our actors. Prices are quoted per project.

### Auf Deutsch

**Prüfen statt raten.** Firmen-Checks und Daten aus öffentlichen Quellen: Wer wirbt bei Google und Bing, wer steht hinter einer Website (USt-IdNr. über die EU-Prüfung VIES), dazu Register, Stellen, Messen, Dokumente und Recherche für KI — [zur deutschen Übersicht](https://perceptron-data.github.io/de/).

**Actors nach Maß:** Schreiben Sie an thom.ehr@gmail.com, welche Quelle und welche Daten Sie brauchen, oder eröffnen Sie ein Issue auf der Apify-Seite eines unserer Actors. Preise je Projekt nach Angebot.

<sub>[Impressum](https://perceptron-data.github.io/impressum/) · [Datenschutz](https://perceptron-data.github.io/datenschutz/) · Independent provider, not affiliated with Apify or the data sources named. Bug reports are welcome.</sub>
