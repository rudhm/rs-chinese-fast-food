# RS Chinese Fast Food & Dudh Dairy 🍔🍜🥛

> **Official Website & Digital Food Menu with WhatsApp Ordering & Free Home Delivery**  
> **Live Site:** [https://rsfastfood.in](https://rsfastfood.in) (or [GitHub Pages Mirror](https://rudhm.github.io/rs-chinese-fast-food/))

---

## 📱 Primary Core Directive: Mobile-First Users

> [!IMPORTANT]
> **95%+ of customers browse and order through mobile phones** via WhatsApp links, table QR code scans, Google Maps, and social media.
> 
> When contributing to or modifying this codebase:
> - **Always design, test, and optimize for mobile viewports (360px – 430px) first.**
> - Keep touch targets at least **44px × 44px**.
> - Ensure all form inputs have a minimum font size of **16px** to prevent iOS Safari auto-zooming.
> - Ensure bottom-sheet cart drawers and bottom checkout bars are ergonomic for one-thumb operation.
> - Verify zero horizontal overflow on mobile screens.
> - Keep asset weights minimal for fast cellular 3G/4G loading.

Refer to [`GEMINI.md`](./GEMINI.md) and [`AGENTS.md`](./AGENTS.md) for full architectural guidelines.

---

## 🌟 Key Features

- **🍔 67 Pure Vegetarian Dishes:** Curated categories including Noodles, Manchurian, Rice, Momos, Pizza, Burgers, Sandwiches, Fries, Pav Bhaji, Chaat, Maggi, Parathas, Shakes, and Hot/Cold Beverages.
- **🔍 Instant Live Search & Filter Chips:** Fast real-time filtering across dish names (English & Hindi) and descriptions, plus one-tap tags (`Must Try`, `Paneer`, `Spicy`, `Under ₹50`).
- **🛒 Dynamic Cart & WhatsApp Ordering:** Pre-fills customer name, delivery address, special cooking instructions, itemized bill, and payment preference into WhatsApp.
- **📱 Progressive Web App (PWA):** Offline asset caching via service worker (`sw.js`) and install-to-homescreen prompt (`manifest.json`).
- **🌓 Dark / Light Theme:** Automatic system theme detection with manual toggle and persistence.
- **🗺️ Directions & Social Sharing:** One-tap Google Maps directions and Web Share API integration.

---

## 🛠️ Local Development

To run the site locally:

```bash
# Python built-in server
python3 -m http.server 8000

# Or using Node
npx serve .
```

Open [http://localhost:8000](http://localhost:8000) in your mobile browser or desktop browser with Mobile Device Emulation turned on (iPhone / Pixel / Galaxy).
