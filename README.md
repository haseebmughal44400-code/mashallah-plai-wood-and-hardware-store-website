# Mashallah Plywood & Hardware Store — Official Website

A modern, high-performance, and responsive commercial business website for **Mashallah Plywood & Hardware Store**, Lahore, Pakistan. Built with React, TypeScript, Vite, and Tailwind CSS.

---

## 📁 Complete Folder Structure

```text
mashallah-plywood-hardware-store/
├── index.html                   # HTML entry point, SEO meta tags, Google Fonts, Schema.org
├── package.json                 # Project dependencies and build scripts
├── tsconfig.json                # TypeScript compiler configuration
├── vite.config.ts               # Vite bundler & Tailwind configuration
├── vercel.json                  # Vercel deployment & routing configuration
├── .gitignore                   # Git ignore file for node_modules, dist, logs
├── README.md                    # Project documentation & deployment guide
├── metadata.json                # Applet configuration metadata
└── src/
    ├── main.tsx                 # React entry point
    ├── App.tsx                  # Main application layout & section coordinator
    ├── index.css                # Global Tailwind CSS & typography setup
    ├── config/
    │   └── storeConfig.ts       # ⭐ CENTRAL CONFIG: WhatsApp, phone, address, timings
    ├── data/
    │   └── products.ts          # ⭐ PRODUCT DATABASE: 12 categories, 20+ products, specs
    └── components/
        ├── Navbar.tsx           # Sticky header, top contact bar, WhatsApp CTA, mobile drawer
        ├── Hero.tsx             # Hero section with value proposition & trust points
        ├── CategorySection.tsx  # 12 hardware & plywood category cards with active filters
        ├── ProductCatalog.tsx   # Live search, category filters, product grid, WhatsApp buttons
        ├── ProductModal.tsx     # Deep-dive product specification & inquiry dialog
        ├── WhyChooseUsSection.tsx # 6 value proposition cards (quality, wholesale rates, delivery)
        ├── HowToOrderSection.tsx # 3-step order workflow + BOQ WhatsApp trigger
        ├── AboutSection.tsx     # Grounded company history, mission, & craftsmanship values
        ├── QuoteRequestSection.tsx # Contractor & bulk inquiry form + WhatsApp dispatch
        ├── ContactSection.tsx   # Complete address, hours, Google Maps, direct phone call
        ├── StickyMobileBar.tsx  # Sticky bottom bar with touch-friendly Call & WhatsApp
        └── Footer.tsx           # Rich footer with links, categories, and copyright
```

---

## 🚀 Quick Start (Local Development)

### 1. Install dependencies
```bash
npm install
```

### 2. Start the development server
```bash
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser.

### 3. Build for production
```bash
npm run build
```
The optimized production bundle will be generated in the `dist/` directory.

---

## 📤 How to Push to GitHub

1. Open your terminal in the project directory:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Mashallah Plywood & Hardware Store website"
   ```

2. Create a new repository on [GitHub](https://github.com/new) named `mashallah-plywood-hardware-store`.

3. Link your local repo and push:
   ```bash
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/mashallah-plywood-hardware-store.git
   git push -u origin main
   ```

---

## ⚡ How to Deploy on Vercel

### Method 1: Via Vercel Web Dashboard (Recommended)
1. Go to [vercel.com](https://vercel.com) and sign in.
2. Click **"Add New..."** -> **"Project"**.
3. Import the `mashallah-plywood-hardware-store` repository from your GitHub account.
4. Framework Preset will automatically detect **Vite**.
5. Build Command: `npm run build`
6. Output Directory: `dist`
7. Click **"Deploy"**. Your website will be live in under 1 minute with free SSL and global CDN!

### Method 2: Via Vercel CLI
```bash
npm install -g vercel
vercel
```

---

## 🛠️ Where to Customize Your Store

### 1. Change WhatsApp, Phone, Address & Timings
Open `src/config/storeConfig.ts`:
- Change `whatsappNumber`: `"923001234567"` (Use international format without `+` or spaces).
- Change `phone`: `"+92 300 1234567"` (Shown in navbar and contact cards).
- Change `address`: Update your exact shop address in Lahore.
- Change `businessHours`: Update weekday, Friday, or Sunday timings.
- Change `delivery`: Toggle `enabled: true/false` or edit Lahore delivery areas.

### 2. Add or Edit Products
Open `src/data/products.ts` and add items to the `PRODUCTS` array:
```typescript
{
  id: "prod-my-item",
  name: "Premium Teak Ply",
  category: "Plywood & Boards",
  description: "Natural decorative veneer sheet for doors and cabinets.",
  image: "https://images.unsplash.com/...",
  featured: true,
  specifications: ["Thickness: 4mm", "Size: 8x4 ft"],
  unitLabel: "Per Sheet"
}
```

### 3. Replace Images
- Use any image URL or place local image files inside a `public/images/` folder and reference them as `/images/your-photo.jpg`.

---

## 📄 License
MIT License. Created for Mashallah Plywood & Hardware Store, Lahore.
