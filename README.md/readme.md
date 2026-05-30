# Ronny Mwenda — Portfolio Website
**ronnymwenda.netlify.app** · Frontend Developer & Math Teacher · Embu, Kenya

---

## 📁 File Structure

```
ronny-site/
├── index.html          ← Main portfolio page (HOME)
├── about.html          ← Full detailed profile page
├── contact.html        ← Dedicated contact & hire page
├── privacy.html        ← Privacy Policy (required for AdSense)
├── terms.html          ← Terms & Conditions
├── 404.html            ← Custom "Page Not Found" page
├── sitemap.xml         ← SEO sitemap for Google
├── robots.txt          ← Search engine crawling rules
├── netlify.toml        ← Netlify deployment config
├── _redirects          ← URL redirects (Netlify)
├── _headers            ← Security & cache headers (Netlify)
├── profile.jpeg        ← ⚠️ ADD THIS — your profile photo
└── og-image.jpg        ← ⚠️ ADD THIS — social share preview image
```

---

## 🚀 How to Deploy on Netlify

### Option A — Drag & Drop (Easiest)
1. Go to [app.netlify.com](https://app.netlify.com)
2. Log in and click **"Add new site"** → **"Deploy manually"**
3. Drag and drop the entire `ronny-site/` folder onto the page
4. Done — your site is live!

### Option B — GitHub (Recommended for updates)
1. Create a GitHub repo called `ronny-portfolio`
2. Upload all files in this folder to that repo
3. In Netlify: **"Add new site"** → **"Import from Git"** → connect GitHub
4. Select your repo, leave build command empty, publish directory = `.`
5. Click **Deploy** — every time you push to GitHub, site auto-updates

---

## 🖼️ Adding Your Profile Photo

1. Name your photo exactly: **`profile.jpeg`** (lowercase, .jpeg not .jpg)
2. Resize it to at least **400×400 pixels**, square crop preferred
3. Place it in the same folder as `index.html`
4. Re-deploy — it will automatically show on all pages

---

## 🌐 Adding Your OG Image (Social Share Preview)

This is the image that appears when you share your site on WhatsApp, Facebook, etc.

1. Create an image **1200×630 pixels** (landscape)
2. Add your name, role, and a nice background
3. Save as **`og-image.jpg`** in the root folder
4. Re-deploy

---

## 📊 Google Search Console Setup

1. Go to [search.google.com/search-console](https://search.google.com/search-console)
2. Click **"Add property"** → enter `https://ronnymwenda.netlify.app`
3. Choose **"HTML tag"** verification method
4. Copy the meta tag: `<meta name="google-site-verification" content="YOUR_CODE" />`
5. Paste it inside the `<head>` of **index.html** (just before `</head>`)
6. Re-deploy, then click **Verify** in Search Console
7. Submit sitemap: go to **Sitemaps** → add `https://ronnymwenda.netlify.app/sitemap.xml`

---

## 📈 Google Analytics Setup

1. Go to [analytics.google.com](https://analytics.google.com)
2. Create a new property for your website
3. Get your **Measurement ID** (looks like `G-XXXXXXXXXX`)
4. Add this code to every HTML file, just before `</head>`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

Replace `G-XXXXXXXXXX` with your actual Measurement ID.

---

## 💰 Google AdSense Setup

> **Requirements before applying:**
> - ✅ Site has original, useful content (blog posts help)
> - ✅ Privacy Policy page exists → `privacy.html` ✓
> - ✅ Terms & Conditions page exists → `terms.html` ✓
> - ✅ Contact page exists → `contact.html` ✓
> - ✅ About page exists → `about.html` ✓
> - ✅ Site is indexed by Google (check Search Console)
> - ✅ At least 3–5 real blog articles published

**Steps:**
1. Go to [adsense.google.com](https://adsense.google.com)
2. Sign in with your Google account
3. Click **"Get started"** → enter `https://ronnymwenda.netlify.app`
4. Copy the AdSense code snippet they give you
5. Paste it inside `<head>` on **every HTML page**
6. Re-deploy and wait for approval (can take 1–2 weeks)

**AdSense code looks like this:**
```html
<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-XXXXXXXXXXXXXXXX"
  crossorigin="anonymous"></script>
```

---

## 📝 How to Add Blog Posts

1. Create a new file e.g. `blog-quadratic-equations.html`
2. Copy the structure from `about.html` (reuse the nav, footer, styles)
3. Write your article content
4. Add the page to `sitemap.xml` with today's date
5. Link to it from the blog section in `index.html`
6. Re-deploy

---

## ✏️ Common Updates

| What to change | Where |
|---|---|
| Your name / bio | `index.html` → About section |
| Add a new project | `index.html` → Projects section |
| Update contact info | `index.html` + `contact.html` |
| Add social link | `index.html` + `contact.html` + `about.html` |
| Update legal docs | `privacy.html` + `terms.html` (update "Last Updated" date) |
| Add blog post | Create new `.html` file + update `sitemap.xml` |

---

## 📞 Contact

**Ronny Mwenda** ("Ronny Best")  
📧 ronnymwenda89@gmail.com  
📱 WhatsApp: +254 799 188 900  
🌍 Embu County, Kenya  
🌐 [ronnymwenda.netlify.app](https://ronnymwenda.netlify.app)