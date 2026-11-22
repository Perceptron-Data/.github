<p align="center"><img src="https://perceptron-data.github.io/assets/logo-256.png" width="88" alt="Perceptron Data"></p>
<h2 align="center">Check, don't guess.</h2>
<p align="center">Company checks and data from public sources, as <a href="https://apify.com/perceptr0n">Apify</a> actors. Built in Germany. Focused on DACH and the EU.<br><a href="https://perceptron-data.github.io/">Website</a> · <a href="https://perceptron-data.github.io/de/">Deutsch</a> · <a href="https://perceptron-data.github.io/agents/">For AI agents</a> · <a href="https://perceptron-data.github.io/quality/">Weekly checks</a> · <a href="https://apify.com/perceptr0n">All actors on Apify</a></p>

Merge lead lists into one row per company, see who is legally behind a website, and watch suppliers and customers for insolvency and register notices. Every row says where its data came from. Paid per result, plus a small start fee per run.

**Measured, not promised**

- **8 s** for 15,000 rows deduplicated by two fields, on the default 512 MB of memory (Dataset Merge & Company Dedupe · Apify platform run, 22 Nov 2026)
- **78.5 days** median by which a notice about provisional measures came before the opening of insolvency proceedings – in 54 of 157 measured openings (Insolvency & Handelsregister Monitor · openings of 16–20 Nov 2026)
- **8 of 9** websites that refused automated requests or needed JavaScript came back complete, with a VIES-valid VAT number (Imprint & VAT Check · Apify platform test, 13 Oct 2026)
- **57 of 57** checks with known answers passed in the weekly check, across 13 actors (Weekly check · 22 Nov 2026)

## Start here

Four actors for B2B list work: merge and deduplicate lead lists, watch companies for insolvency and register notices, find the company behind a website, and read the job board of the Bundesagentur für Arbeit.

| | Actor | What you get | Price (Apify free plan) |
|---|---|---|---|
| <img src="https://perceptron-data.github.io/assets/icons/dataset-merge-dedupe-256.png" width="32" alt=""> | [Dataset Merge & Company Dedupe](https://perceptron-data.github.io/actors/merge-dedupe-datasets-company-leads/) | Datasets, files or rows in, one merged dataset without duplicates out – for lead lists one row per company, with the reason for every merge. | $0.30 per 1,000 rows in merge or dedupe mode (from $0.20) + $0.00005 start fee per run |
| <img src="https://perceptron-data.github.io/assets/icons/insolvency-monitor-256.png" width="32" alt=""> | [Insolvency & Handelsregister Monitor](https://perceptron-data.github.io/actors/german-insolvency-handelsregister-monitor/) | Company list in, one row per German company out: insolvency and register notices, EU VAT ID check, open positions – or only what changed. | $20.00 per 1,000 company rows (from $10.00) + $0.00005 start fee per run |
| <img src="https://perceptron-data.github.io/assets/icons/impressum-256.png" width="32" alt=""> | [Imprint & VAT Check](https://perceptron-data.github.io/actors/imprint-impressum-website-contact-scraper/) | Domains in, company rows out: legal name, address, register number and EU VAT ID checked against VIES – from the Impressum. | $5.00 per 1,000 websites (from $2.50) + $0.01 start fee per run |
| <img src="https://perceptron-data.github.io/assets/icons/arbeitsagentur-256.png" width="32" alt=""> | [Arbeitsagentur Jobs](https://perceptron-data.github.io/actors/arbeitsagentur-jobs-scraper/) | Keyword and place in, one row per job out: employer, salary range, home office, location – who is hiring in Germany. | $1.00 per 1,000 jobs (from $0.50) + $0.01 start fee per run |

## How the actors work together

A lead pipeline in four runs – each run works on the rows of the one before:

1. **Fetch jobs and sources** – Job ads, companies that are hiring, trade-fair exhibitors – or your own export. One row per record, with the company's name. (Arbeitsagentur Jobs, Hiring Companies Germany, Messe München Exhibitors)
2. **Merge company duplicates** – Several lists become one row per company. Every merged row names the reason. (Dataset Merge & Company Dedupe)
3. **Check imprint and VAT ID** – For rows that carry a website: legal name, register number and EU VAT ID from its legal notice, the VAT ID checked against VIES. (Imprint & VAT Check)
4. **Insolvency watchlist** – The register numbers go onto a watchlist. After the first run, a scheduled run returns a row only for companies where something changed. (Insolvency & Handelsregister Monitor)

Each step is one run on Apify – started by hand, on a schedule, through the API or by an AI agent.

## For AI agents

Every actor is a tool on Apify's MCP server. Name the tools in the address and your agent has them at hand: it sees the input fields and the price per result before it calls (plus a small start fee per run).

```
https://mcp.apify.com?tools=perceptr0n/merge-dedupe-datasets-company-leads,perceptr0n/german-insolvency-handelsregister-monitor,perceptr0n/imprint-impressum-website-contact-scraper,perceptr0n/arbeitsagentur-jobs-scraper
```

[Set it up in Claude Code, Cursor or n8n](https://perceptron-data.github.io/agents/)

## All actors

### Company checks

Two checks for lists of companies, with a traceable answer per company.

| | Actor | What you get | Price (Apify free plan) |
|---|---|---|---|
| <img src="https://perceptron-data.github.io/assets/icons/ads-transparency-256.png" width="32" alt=""> | [Advertiser Check (Google & Bing)](https://perceptron-data.github.io/actors/google-ads-transparency-scraper/) | Company list in, one row per company out: Google ads, Bing ads, ad counts, accounts – for domains, Bing matches proven by landing pages. | $4.00 per 1,000 companies checked (from $2.50) + $0.01 start fee per run |
| <img src="https://perceptron-data.github.io/assets/icons/impressum-256.png" width="32" alt=""> | [Imprint & VAT Check](https://perceptron-data.github.io/actors/imprint-impressum-website-contact-scraper/) | Domains in, company rows out: legal name, address, register number and EU VAT ID checked against VIES – from the Impressum. | $5.00 per 1,000 websites (from $2.50) + $0.01 start fee per run |
| <img src="https://perceptron-data.github.io/assets/icons/website-contact-256.png" width="32" alt=""> | [Free Imprint & Contact Check](https://perceptron-data.github.io/actors/free-website-contact-imprint-scraper/) | Free: the same company row as the paid check – EU VAT ID checked against VIES, email, phone – for up to 10 websites per run. | Free |

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
| <img src="https://perceptron-data.github.io/assets/icons/xing-jobs-256.png" width="32" alt=""> | [XING Jobs](https://perceptron-data.github.io/actors/xing-jobs-scraper/) | Keyword and place in, one row per job out: company, salary with its source, career level, full text – DACH jobs from XING. | $1.00 per 1,000 jobs (from $0.50) + $0.00005 start fee per run |
| <img src="https://perceptron-data.github.io/assets/icons/hiring-companies-256.png" width="32" alt=""> | [Hiring Companies Germany](https://perceptron-data.github.io/actors/hiring-companies-germany/) | Job and place in, one row per hiring company out: open positions, own website confirmed by its Impressum, contact data. | $10.00 per 1,000 companies (from $5.00) + $0.01 start fee per run |
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

### Documents

PDF, Word, Excel and PowerPoint to Markdown – tables as Markdown and JSON rows, OCR for scans.

| | Actor | What you get | Price (Apify free plan) |
|---|---|---|---|
| <img src="https://perceptron-data.github.io/assets/icons/doc-markdown-256.png" width="32" alt=""> | [PDF to Markdown](https://perceptron-data.github.io/actors/pdf-to-markdown-converter/) | Files in, Markdown out – tables as Markdown and JSON rows, OCR for scans, RAG chunks with page numbers. No LLM involved. | $0.50 per 1,000 pages (from $0.35) + $0.005 start fee per run |

### Tools

Merge datasets and remove duplicates – or let the free finder name the actor that fits, with fields and run cost.

| | Actor | What you get | Price (Apify free plan) |
|---|---|---|---|
| <img src="https://perceptron-data.github.io/assets/icons/dataset-merge-dedupe-256.png" width="32" alt=""> | [Dataset Merge & Company Dedupe](https://perceptron-data.github.io/actors/merge-dedupe-datasets-company-leads/) | Datasets, files or rows in, one merged dataset without duplicates out – for lead lists one row per company, with the reason for every merge. | $0.30 per 1,000 rows in merge or dedupe mode (from $0.20) + $0.00005 start fee per run |
| <img src="https://perceptron-data.github.io/assets/icons/finder-256.png" width="32" alt=""> | [Data Source Finder](https://perceptron-data.github.io/actors/dach-eu-data-source-finder/) | A source in, the matching actor out – with fields, record count and run cost. Free. | Free |

## Built by Thomas Ehrler · Engineering & Custom Actors

One developer builds and runs every actor in this catalogue. The rules below hold for each of them – and for every actor built to order.

- **Direct interfaces, plain HTTP** – 15 of the 16 actors start no browser: they read their sources over direct interfaces and plain HTTP, on 256 MB to 1 GB of default memory. kununu Employer Data starts one; the imprint checks and Hiring Companies Germany can hand a page that needs JavaScript to Apify's Web Fetch.
- **Fixed rules, nothing guessed** – When rows are put together or a website is assigned to a company, the row names the reason. What cannot be shown stays apart or is reported as not found. In the Imprint & VAT Check and the Insolvency & Handelsregister Monitor an outage of a source is a status of its own – not “nothing found”.
- **Tested against outages and restarts** – Before an upload every actor goes through a test bench: a run like Apify's daily test, simulated blocks and outages of the source, and – where a run is long enough – a restart in the middle. Every Sunday a watchdog repeats the published checks.
- **Based in Germany** – Thomas Ehrler builds and runs the actors from Germany; the legal notice names him. The focus is on company data from Germany, Austria, Switzerland and the EU, and every actor is described in English and German.

### Custom Apify actors and B2B pipelines

Need a source that is not in the catalogue, extra fields or a different delivery? Perceptron Data also builds actors to order. Actors for public sources in Germany, Austria, Switzerland and the EU: job boards, registers, company websites, trade-fair directories and documents.

#### How it works

1. You describe the source and the data you need – in an e-mail or in an issue on the Apify page of one of our actors.
2. You get a quote for that description; there is no price list.
3. We build the actor.
4. Before delivery it passes the same test bench as our published actors: a run like Apify's daily test, a restart in the middle of a run, and simulated blocks and outages of the source.
5. You get it as an actor in your own Apify account.

#### What we do not do

- No data behind a login.
- No bypassing of bot protection.

Write to thom.ehr@gmail.com with the source and the data you need, or open an issue on the Apify page of one of our actors. Prices are quoted per project.

## Auf Deutsch

**Prüfen statt raten.** Firmen-Checks und Daten aus öffentlichen Quellen: Lead-Listen zu einer Zeile je Firma zusammenführen, sehen, wer hinter einer Website steht (USt-IdNr. über die EU-Prüfung VIES), Firmen auf Insolvenz- und Registerbekanntmachungen beobachten – dazu Stellen, Messen, Register und Dokumente. [Zur deutschen Übersicht](https://perceptron-data.github.io/de/)

**Actors nach Maß:** Schreiben Sie an thom.ehr@gmail.com, welche Quelle und welche Daten Sie brauchen, oder eröffnen Sie ein Issue auf der Apify-Seite eines unserer Actors. Preise je Projekt nach Angebot.

<sub>[Impressum](https://perceptron-data.github.io/impressum/) · [Datenschutz](https://perceptron-data.github.io/datenschutz/) · Independent provider, not affiliated with Apify or the data sources named. Bug reports are welcome.</sub>
