# 👑 Royal Home Clean Delft - Premium Cleaning Services

A high-converting, SEO-optimized, bilingual (EN/NL) landing page for Tatiana's premium cleaning business in Delft. This site is built for speed, elegance, and lead generation.

## 🚀 Live Features
* **Bilingual Toggle:** Seamless switching between English and Dutch without page reloads.
* **Fully Responsive:** Optimized for desktop, tablet, and mobile (crucial for local service searches).
* **Lead Generation:** Integrated with **EmailJS** for direct-to-inbox quotes and a floating **WhatsApp** button for instant conversion.
* **Modern Aesthetic:** Built with Tailwind CSS, utilizing a "Delft Blue" color palette and premium serif typography.

## 📈 SEO Strategy (Search Engine Optimization)
This site is engineered to rank for high-volume Dutch cleaning keywords:
* **Primary Keywords:** *Schoonmaakdiensten* (45k), *Huishoudelijke hulp* (40k), *Raamreiniging* (35k), *Schoonmaakbedrijf* (32k), *Dieptereiniging* (29k).
* **Local SEO:** Includes specific Delft neighborhood tagging (**Tanthof, Voorhof, Buitenhof, etc.**) to capture "near me" search intent.
* **Schema Markup:** Includes **JSON-LD LocalBusiness data** so Google displays your business info, price range, and location clearly in search results.

## 🛠 Tech Stack
* **HTML5 / CSS3** (Tailwind CSS via CDN)
* **JavaScript** (Vanilla JS for language toggling and UI logic)
* **EmailJS** (Handles the contact form without needing a back-end server)
* **Google Fonts** (Playfair Display & Inter)

## ⚙️ Configuration & Maintenance

### 1. Contact Form (EmailJS)
The form is currently linked to Tatiana's EmailJS account. To update the recipient:
1.  Go to the `<script>` section at the bottom of the HTML.
2.  Update the `emailjs.init("YOUR_PUBLIC_KEY")`.
3.  Update the `service_ID` and `template_ID` in the `emailjs.sendForm` function.

### 2. Updating Prices
Prices are located in the "Our Cleaning Services" section. 
> **Note:** Remember to update the price in **both** the `.lang.en` and `.lang.nl` divs to keep the site consistent.

### 3. Adding New Neighborhoods
To add more service areas, scroll to the "Areas We Serve" section and add a new `<span>` tag following this format:
```html
<span class="bg-white/10 px-4 py-2 rounded-full text-sm font-semibold tracking-wide">📍 Neighborhood Name</span>
