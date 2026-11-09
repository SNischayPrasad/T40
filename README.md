# 🔍 SEO Keyword Research & Content Optimization System

> Digital Marketing Internship Project | Sadhanala Nischay Prasad

A complete, repeatable SEO system for a technology services website: keyword research, search-intent analysis, keyword difficulty scoring, competitor gap analysis, keyword-to-page mapping, an on-page SEO audit, and a content and internal-linking plan with a measurement framework.

**Target website:** *NexaByte Solutions*, a sample IT services website (web development, mobile apps, AI solutions, UI/UX design) based in Hyderabad, used as the practice case.

---

## 🎯 Objective

Learn practical SEO fundamentals including keyword research, search intent, on-page optimization, content structure, internal linking and SEO measurement.

## 🛠️ Tools Used

| Tool | Used for |
|---|---|
| Google Search | SERP review, autocomplete, "People also ask", competitor analysis |
| Google Trends | 12-month interest trend (Rising / Stable) for India |
| Google Keyword Planner (concepts) | Search volume ranges and keyword ideas |
| Google Search Console (concepts) | Measurement plan: impressions, clicks, CTR, position |
| Google Sheets / Excel | Keyword dataset, scoring formulas, mapping and plans |
| HTML | Before/after on-page optimized page |
| Google Docs | Project report |

## 📁 Repository Structure

```
seo-keyword-research-system/
├── README.md
├── SEO_Keyword_Research_System.xlsx      # Master workbook (12 sheets, live formulas)
├── data/
│   ├── keyword_research_dataset.csv      # 33 keywords with intent, volume, KD, priority
│   ├── competitor_analysis.csv           # SERP & competitor gap analysis
│   ├── keyword_page_mapping.csv          # Keyword-to-page mapping
│   ├── onpage_seo_audit.csv              # 18 audit findings + fixes
│   ├── title_meta_recommendations.csv    # Optimized titles & meta descriptions
│   ├── heading_structure.csv             # H1/H2/H3 recommendations
│   ├── internal_linking_plan.csv         # Hub-and-spoke linking plan
│   ├── content_plan.csv                  # 12 SEO blog ideas, 6-week calendar
│   └── seo_kpis.csv                      # Measurement framework
├── html/
│   ├── before-web-development.html       # Original unoptimized page
│   └── optimized-web-development.html    # SEO-optimized version
└── report/
    └── SEO_Optimization_Report.pdf       # Full project report
```

## ⚙️ Methodology

1. **Seed keywords** from the site's core services + location (Hyderabad).
2. **Expand** using Google autocomplete, "People also ask" and "Related searches".
3. **Estimate volume** with Keyword Planner ranges (10–100, 100–1K, 1K–10K, India).
4. **Check trends** in Google Trends (last 12 months).
5. **Score difficulty** (0–100) by reviewing page-1 results: big brands, directories, ads, SERP features.
6. **Classify intent**: Informational, Commercial, Transactional, Navigational.
7. **Prioritize** with a formula (in the Excel sheet):

```
Priority Score = LOG10(Volume) × 10 × (100 − KD) / 100 × Intent Weight
Intent weights: Transactional 1.0 · Commercial 0.9 · Informational 0.6 · Navigational 0.4
```

8. **Map** one primary keyword per page, then audit and optimize each page.

> ⚠️ Volumes and difficulty are learning estimates based on tool ranges and manual SERP review. Verify with live tool data before using on a real site.

## 📊 Deliverables

| # | Deliverable | Where |
|---|---|---|
| 1 | Keyword research dataset | `data/keyword_research_dataset.csv`, sheet *Keyword Dataset* |
| 2 | Primary & secondary keywords | sheet *Primary & Secondary* |
| 3 | Search-intent classification | sheet *Search Intent* |
| 4 | Keyword difficulty analysis | *Keyword Dataset* (KD + Easy/Medium/Hard bands) |
| 5 | Competitor keyword analysis | `data/competitor_analysis.csv` |
| 6 | Keyword-to-page mapping | `data/keyword_page_mapping.csv` |
| 7 | On-page SEO audit | `data/onpage_seo_audit.csv` |
| 8 | Title & meta-description recommendations | `data/title_meta_recommendations.csv` (length checks with `LEN()`) |
| 9 | Heading structure recommendations | `data/heading_structure.csv` |
| 10 | Internal-linking plan | `data/internal_linking_plan.csv` |
| 11 | SEO content ideas | `data/content_plan.csv` |
| 12 | SEO optimization report | `report/SEO_Optimization_Report.pdf` |

## 🏆 Top Keyword Opportunities

| Keyword | Intent | Est. Volume | KD | Target Page | Score |
|---|---|---|---|---|---|
| website development cost in india | Commercial | 1,300 | 35 | /blog | 18.2 |
| ecommerce website development hyderabad | Transactional | 390 | 40 | /web-development | 15.5 |
| ui ux design company hyderabad | Commercial | 480 | 38 | /ui-ux-design | 15.0 |
| ai chatbot development services | Commercial | 590 | 41 | /ai-solutions | 14.7 |
| website redesign services | Commercial | 320 | 35 | /ui-ux-design | 14.7 |
| custom ai solutions for business | Commercial | 260 | 33 | /ai-solutions | 14.6 |

## 🗺️ Keyword-to-Page Mapping (Summary)

| Page | Primary Keyword |
|---|---|
| `/` | software development company in hyderabad |
| `/web-development` | web development company in hyderabad |
| `/mobile-app-development` | mobile app development company in hyderabad |
| `/ai-solutions` | ai development company in india |
| `/ui-ux-design` | ui ux design company hyderabad |
| `/contact` | software company near me (local) |
| `/blog` | cost guides, comparisons, how-tos (informational) |

## 🧾 On-Page Optimization: Before vs After

| Element | Before | After |
|---|---|---|
| Title | `Services` | `Web Development Company in Hyderabad \| NexaByte` (47 chars) |
| Meta description | Missing | 137-char description with keyword + CTA |
| H1 | Two H1s (`Welcome`, `Our Services`) | One H1 with the primary keyword |
| Headings | H4 before any H2 | Logical H1 → H2 → H3 |
| Images | No alt text, 2.4 MB PNG | Descriptive alt, WebP, lazy-loaded |
| Links | "Click here", `/services?id=5` | Descriptive anchors, clean URLs |
| Technical | No canonical, no schema | Canonical, Open Graph, LocalBusiness JSON-LD |

See `html/before-web-development.html` and `html/optimized-web-development.html`.

## 🔗 Internal Linking Strategy

Hub-and-spoke model: service pages are **hubs**, blog posts are **spokes** that link back with keyword-rich anchor text. The home page passes authority to every service page, and every page has a conversion link to `/contact`.

## ✍️ Content Plan (6 Weeks)

12 blog posts targeting low-difficulty informational and commercial keywords, for example *Website Development Cost in India (2026 Price Guide)*, *Static vs Dynamic Website*, *React vs Next.js*, and *AI Automation for Small Business*. Full calendar in `data/content_plan.csv`.

## 📈 Measurement (Google Search Console)

| KPI | Target (3 months) |
|---|---|
| Impressions | +50% |
| Clicks | +40% |
| CTR | > 3% sitewide |
| Average position | Primary keywords in Top 10 |
| Indexed pages | 100% of key pages |
| Core Web Vitals | All URLs "Good" |

## 💡 Key Learnings

- Search intent matters more than raw volume.
- One primary keyword per page prevents keyword cannibalization.
- Long-tail, low-difficulty keywords are the fastest wins for small sites.
- Titles, metas and headings are small edits with big impact on CTR.
- Internal links connect blog traffic to service (money) pages.
- SEO is measurable: Search Console data shows what to fix next.

## 🚀 How to Use

1. Open `SEO_Keyword_Research_System.xlsx` in Excel or upload it to Google Sheets.
2. Change the intent weights on the **Assumptions** sheet; Priority Scores update automatically.
3. Replace the sample keywords with your own site's data to reuse the system.
4. Open the HTML files in a browser or editor to compare the before/after pages.

## 👤 Author

**Sadhanala Nischay Prasad**
Digital Marketing Intern | B.Tech in Artificial Intelligence
🔗 [LinkedIn](https://www.linkedin.com/in/your-profile) · 📧 nischayprasuna@gmail.com

---

⭐ If you found this useful, consider starring the repo!
