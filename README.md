# 👑 Royal Home Clean Delft - Premium Multi-Page Cleaning Website

A high-converting, SEO-optimized, bilingual (EN/NL) platform for a premium house cleaning business in Delft. This site utilizes a professional multi-page structure to maximize local SEO and lead generation.

## 🚀 Live Features
* **Multi-Page Architecture:** Uses a clean folder-based URL structure (e.g., `/move-out-cleaning/`) for better user experience and professional appearance.
* **Bilingual Toggle:** Seamless switching between English and Dutch across all pages without reloads.
* **Fully Responsive:** Optimized for desktop, tablet, and mobile (crucial for local service searches).
* **Lead Generation:** Integrated with **EmailJS** for direct-to-inbox quotes and a floating **WhatsApp** button for instant conversion.
* **Modern Aesthetic:** Built with Tailwind CSS, utilizing a "Delft Blue" color palette and premium serif typography.

## 📈 SEO Strategy (Search Engine Optimization)
This site is engineered to rank for high-volume Dutch and Expat cleaning keywords:
* **Dedicated Service Pages:** Targeted landing pages for high-intent keywords like "End of tenancy cleaning" and "Move out cleaning Delft."
* **Primary Keywords:** *Schoonmaakdiensten* (45k), *Huishoudelijke hulp* (40k), *Opleveringsschoonmaak*, *Schoonmaakbedrijf*.
* **Local SEO:** Specific Delft neighborhood tagging (**Tanthof, Voorhof, Buitenhof, etc.**) and **XML Sitemap** integration for rapid Google indexing.
* **Schema Markup:** Includes **JSON-LD LocalBusiness data** for rich search results.

## 🛠 Tech Stack
* **HTML5 / CSS3** (Tailwind CSS via CDN)
* **JavaScript** (Vanilla JS for language toggling and UI logic)
* **EmailJS** (Serverless contact form handling)
* **Google Search Console** (Integrated via Sitemap.xml)

## ⚙️ Configuration & Maintenance

### 1. Managing Pages & Folders
The site uses a "Clean URL" structure. To edit specific pages:
* **Home Page:** Edit `index.html` in the root folder.
* **Move-Out Page:** Edit `move-out-cleaning/index.html`.
* **Images:** Store page-specific images inside their respective service folders to keep the repository organized.

### 2. Contact Form (EmailJS)
The form is linked to an EmailJS account. To update the recipient:
1. Go to the `<script>` section at the bottom of the HTML.
2. Update the `emailjs.init("YOUR_PUBLIC_KEY")`.
3. Update the `service_ID` and `template_ID`.

### 3. Sitemap Updates
When adding a new page, ensure the `sitemap.xml` in the root directory is updated and re-submitted to Google Search Console to ensure the new content is crawled immediately.

### 4. Updating Prices & Content
> **Note:** Because the site is bilingual, remember to update content in **both** the `.lang.en` and `.lang.nl` divs to maintain consistency.
