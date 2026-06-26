# How to publish this site & make it appear in Google search

Your site is built and ready. But to be searchable on Google, it must be **hosted on a public domain**. Here is exactly what to do.

---

## What's in this folder

```
index.html                  ← the main website page
conference-proceedings.pdf  ← your 16 MB PDF (renamed for SEO)
robots.txt                  ← tells Google to crawl everything
sitemap.xml                 ← lists pages for Google to find
README.md                   ← this file
```

---

## Step 1 — Host the website (pick ONE option)

### Option A: GitHub Pages (free, easiest, recommended)
1. Make a GitHub account at https://github.com
2. Create a new public repository (e.g. `termiz-conference-2025`)
3. Upload all 4 files (`index.html`, `conference-proceedings.pdf`, `robots.txt`, `sitemap.xml`) to the repo
4. Go to **Settings → Pages**, set source to `main` branch, root folder
5. Your site is live at: `https://YOUR_USERNAME.github.io/termiz-conference-2025/`

### Option B: Netlify (free, drag-and-drop)
1. Go to https://app.netlify.com/drop
2. Drag the entire `website` folder onto the page
3. You get a URL like `https://random-name.netlify.app` immediately
4. You can change the URL name in site settings

### Option C: Vercel (free)
1. Go to https://vercel.com → "Add New Project"
2. Drag in the folder or connect a GitHub repo
3. Deploy.

### Option D: Your own domain (best for SEO long-term)
Buy a domain (e.g. `termiz-conference.uz`, `tdpi-anjuman.uz`) for ~$10/year from Namecheap, GoDaddy, or any registrar, then point it to GitHub Pages / Netlify / Vercel.

---

## Step 2 — Update the URLs in your files

After you know your final URL (e.g. `https://termiz-conference.netlify.app`), open these three files and **replace every `https://example.com/`** with your real URL:

- `index.html` — search for `example.com` (appears in `<link rel="canonical">`, Open Graph tags, and JSON-LD)
- `robots.txt` — update the `Sitemap:` line
- `sitemap.xml` — update both `<loc>` lines

You can do this with Find & Replace in any text editor (Notepad, VS Code, etc.).

---

## Step 3 — Submit to Google Search Console (this is what gets you indexed)

This is the **most important step**. Google won't find your site automatically.

1. Go to https://search.google.com/search-console
2. Click **Add property → URL prefix**, paste your site URL
3. Verify you own the site (Google will give you a small HTML file to upload, or a DNS record)
4. Once verified:
   - Go to **Sitemaps** (left sidebar) → submit `sitemap.xml`
   - Go to **URL Inspection** → paste your homepage URL → click **Request Indexing**
   - Repeat URL Inspection for the PDF URL: `https://YOUR-SITE/conference-proceedings.pdf` → Request Indexing

5. Also submit to **Bing**: https://www.bing.com/webmasters (covers Bing, DuckDuckGo, Yahoo)

---

## Step 4 — Wait and verify

- **Indexing typically takes 3–14 days.** Sometimes faster, sometimes a month.
- Check progress in Search Console under **Coverage / Pages**.
- Once indexed, you can find your site by searching:
  - `site:YOUR-DOMAIN.com` — shows everything Google has indexed from you
  - `"Xorijiy tillarni mutaxassislik fanlarida o'qitishning yangi pedagogik yondashuvlari"` (with quotes) — exact title match
  - `"978-9910-786-25-0"` — by ISBN
  - `"Termiz davlat pedagogika instituti" anjuman 2025`

---

## Step 5 — Help it rank higher (optional but powerful)

Search rankings improve when other sites link to yours. Some easy wins:

- **Google Scholar**: submit the PDF via https://scholar.google.com/intl/en/scholar/inclusion.html (academic citations rank very highly)
- **Academia.edu** or **ResearchGate**: upload the PDF and link back to your site
- **Wikipedia**: if the conference is notable, add a citation
- **Termiz DPI's own website**: ask them to link to your page
- **Social media**: share the URL on LinkedIn, Telegram, Facebook — every share helps

---

## SEO features already built in

Your site already includes everything Google looks for:

- ✅ Descriptive `<title>` with the full Uzbek title + ISBN
- ✅ Meta description in Uzbek with all key terms
- ✅ Keyword meta tag covering the topic
- ✅ Schema.org `Book` structured data (Google reads this and shows it as a rich result)
- ✅ Open Graph tags (for sharing on Facebook/Telegram)
- ✅ Twitter Card tags
- ✅ Semantic HTML structure (`<header>`, `<section>`, `<footer>`, `<dl>`)
- ✅ Mobile-responsive design (Google's mobile-first index loves this)
- ✅ `robots.txt` allowing all crawlers
- ✅ `sitemap.xml` listing both the page and the PDF
- ✅ Canonical link tag
- ✅ Multilingual signals (Uzbek primary, English alternate)
- ✅ The PDF filename `conference-proceedings.pdf` is SEO-friendly
- ✅ Fast load (no heavy frameworks, just HTML + CSS)

---

## A realistic note

Even with perfect SEO, ranking #1 on Google for competitive terms is hard. But ranking well for **specific, long-tail queries** about THIS book is very achievable. People searching for:
- the exact title
- the ISBN `978-9910-786-25-0`
- editor names like "Kabilova Sayyora"
- "Termiz DPI 2025 anjuman"

…will almost certainly find your site once it's indexed, because there is little competition for these specific terms.

Good luck!
