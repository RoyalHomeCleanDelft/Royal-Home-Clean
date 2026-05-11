# 👑 Royal Home Clean Delft - Premium Multi-Page Cleaning Website

A high-converting, SEO-optimized, bilingual (EN/NL) platform for a premium professional cleaning business in Delft. This site utilizes a modern multi-page structure and advanced indexing rules to maximize local search visibility.

## 🚀 Live Features

* **Specialized Service Pages:** Dedicated landing pages for **Carpet Cleaning** and **Move-Out Cleaning** to capture specific search intent.
* **Bilingual Toggle:** Seamless switching between English and Dutch across all pages via URL parameters (`?lang=en` / `?lang=nl`).
* **Fully Responsive:** Mobile-first design optimized for local service searches on the go.
* **Lead Generation:** Integrated with **EmailJS** for direct-to-inbox quotes and a floating **WhatsApp** button for instant bookings.
* **Advanced Drying Tech:** Highlights professional HeatWave & DualBrush technology for 1-hour carpet drying.

## 📈 SEO & Indexing Strategy

This site is engineered to rank for high-volume Dutch and Expat cleaning keywords while maintaining a "clean" index in Google Search Console:

* **Primary Keywords:** *Tapijtreiniging Delft*, *Schoonmaakbedrijf*, *Move-out cleaning Delft*, *Bank reinigen*.
* **Clean URL Indexing:** Uses a simplified `sitemap.xml` that only lists primary URLs to prevent "Alternative page" indexing errors.
* **Parameter Management:** A custom `robots.txt` file is configured to prevent search engines from indexing language-variant duplicates, focusing 100% of "ranking power" on the main pages.
* **Local SEO:** Specific neighborhood targeting for Delft (Tanthof, Voorhof, Buitenhof, etc.) and JSON-LD LocalBusiness schema.

## 🛠 Tech Stack

* **HTML5 / CSS3** (Tailwind CSS via CDN)
* **JavaScript** (Vanilla JS for language toggling and UI logic)
* **EmailJS** (Serverless contact form handling)
* **Robots.txt & Sitemap.xml** (Configured for optimal Google Search Console health)

## ⚙️ Configuration & Maintenance

### 1. Managing Pages

To edit the content of your service pages:

* **Carpet Cleaning (Home):** Edit `index.html`.
* **Move-Out Cleaning:** Edit `move-out-cleaning.html`.
* **General Assets:** Favicons and shared images are located in the root directory.

### 2. Indexing & Google Search Console

If you add a new page to the site:

1. **Sitemap:** Add the new clean URL to `sitemap.xml`. Do **not** include URLs with `?lang=` parameters.
2. **Robots.txt:** Ensure the `Disallow: /*?lang=` rule remains in place to prevent duplicate content flags.
3. **Validation:** After making changes, re-submit the sitemap in Google Search Console to trigger a fresh crawl.

### 3. Contact Form (EmailJS)

The form is linked to an EmailJS account. To update the recipient or credentials:

1. Locate the `<script>` section at the bottom of the HTML files.
2. Update the `emailjs.init("YOUR_PUBLIC_KEY")`.
3. Ensure the `service_ID` and `template_ID` match your EmailJS dashboard.

### 4. Updating Content

Because the site is bilingual, always ensure that updates are made in **both** the English and Dutch content blocks:

* `<div class="lang-en">...</div>`
* `<div class="lang-nl">...</div>`
