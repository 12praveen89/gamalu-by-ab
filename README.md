# GAMALU by AB &bull; Artisanal Luxury Candle E-Commerce

Welcome to **Gamalu by AB**, an interactive, single-file luxury artisanal e-commerce web application engineered with quiet luxury aesthetics, editorial minimalism, tactile warmth, and a complete online ordering engine.

---

## 🌟 Visual Design System & Aesthetics

- **Color Palette**:
  - **Background Primary**: Warm Alabaster (`#FAF9F6`)
  - **Background Secondary / Cards**: Soft Linen (`#F3EFEA`) and Raw Silk (`#E5DFD5`)
  - **Primary Typography & Accents**: Obsidian (`#1A1715`) and Espresso Charcoal (`#2C2724`)
  - **Muted Text & Borders**: Deep Bark (`#4A443F`) and Warm Sand (`#D1C7B8`)
  - **Luxury Highlight**: Brushed Gold (`#C59B27` / `#D4AF37`)
- **Typography**:
  - **Display / Headings**: *Cormorant Garamond* (Serif, editorial elegance, subtle italic accents)
  - **Body / Micro-labels**: *Inter* (Clean sans-serif with wide uppercase tracking)
- **Micro-Interactions**:
  - Glassmorphic sticky header (`backdrop-blur-md`)
  - Smooth 700ms image zoom transitions (`hover:scale-105`)
  - Non-blocking custom toast notification stack
  - Real-time complimentary shipping progress bar (Free shipping at ₹3,500)

---

## 🏛️ Architecture & Key Features

### 1. Editorial Hero & Craftsmanship
- Asymmetrical two-column layout featuring micro-batch badge, editorial headline, value proposition (100% soy-coconut wax, cedarwood wicks, pure botanicals), and dual CTAs.
- Lifestyle hero showcase with a floating glassmorphic spec badge.
- 3-pillar craftsmanship strip detailing botanical formulation, FSC-certified cedarwood crackle, and soot-free burn.

### 2. Interactive Product Catalog ("The Collection")
- **Category Filter Pills**: Dynamically filters across *All Scents*, *Woody & Earthy*, *Floral & Botanical*, *Spiced & Warm*, and *Fresh & Citrus*.
- **Sorting Engine**: Sort by Curated, Price (Low to High, High to Low), or Burn Time.
- **8 Signature Candles**:
  1. `No. 01 — Santal & Smoked Cardamom` (Woody & Earthy &bull; ₹2,450)
  2. `No. 02 — Fig Leaf & Solar Jasmine` (Floral & Botanical &bull; ₹2,600)
  3. `No. 03 — Hinoki Wood & Forest Mist` (Woody & Earthy &bull; ₹2,850)
  4. `No. 04 — Amber Resin & Clove Hearth` (Spiced & Warm &bull; ₹2,950)
  5. `No. 05 — Bergamot Zest & White Vetiver` (Fresh & Citrus &bull; ₹2,350)
  6. `No. 06 — Oudh Imperial & Damask Rose` (Floral & Botanical &bull; ₹3,200)
  7. `No. 07 — Smoked Vanilla & Bourbon Tobacco` (Spiced & Warm &bull; ₹2,750)
  8. `No. 08 — Wild Neroli & Sea Salt Driftwood` (Fresh & Citrus &bull; ₹2,500)
- **Quick View / Scent Profile Modal**: Displays comprehensive Olfactory Pyramid (Top, Heart, Base notes), Vessel specs, Burn time, and an instant Add-to-Bag stepper.

### 3. Interactive Olfactory Mood Guide
- Explore candles by sensory intention: *Evening Warmth & Intimacy*, *Deep Focus & Grounding*, and *Serene Renewal & Breath*.
- Dynamic breakdown of note evaporation over 15 mins, 1–3 hours, and lingering memory.

### 4. The Burning Ritual & Vessel Longevity
- 4-step interactive visual guide to memory melt, cedarwick trimming, snuffer usage, and vessel repurposing.

### 5. Client-Side E-Commerce & Ordering Flow
- **Slide-Over Shopping Bag Drawer**:
  - Live subtotal and dynamic **Complimentary Shipping Progress Bar** calibrated to the ₹3,500 threshold.
  - Item increment/decrement controls, live thumbnail previews, and instant item removal.
  - State persisted via `localStorage`.
- **Checkout Modal**:
  - Client & delivery form (Name, Email, 10-digit Phone, 6-digit PIN, Address, State).
  - Optional hand-calligraphed complimentary gift note toggle with preview.
  - Payment selector (UPI/QR, Credit/Debit Card, Cash on Delivery) with validation.
- **Digital Order Confirmation Receipt**:
  - Generates unique order identifier (e.g. `#GAB-8492`).
  - Summarizes purchased objects, client information, pricing breakdown, and climate-controlled delivery timeline.
  - Built-in "Print Receipt" (`window.print()`) utility.

---

## 🚀 How to Run

1. Open `index.html` directly in any modern browser (Chrome, Safari, Firefox, Edge, Brave):
   ```bash
   open ~/Desktop/gamalu-by-ab/index.html
   ```
2. Or serve it locally using any static web server:
   ```bash
   cd ~/Desktop/gamalu-by-ab
   python3 -m http.server 8000
   ```
   Then navigate to `http://localhost:8000`.

---

## 🛠️ Tech Stack

- **HTML5 & Vanilla ES6+ JavaScript**: Zero dependencies or build steps required.
- **Tailwind CSS (CDN)**: Customized with bespoke quiet luxury design tokens.
- **Google Fonts**: Cormorant Garamond & Inter.
- **Lucide Icons (CDN)**: Crisp SVG icons.
- **LocalStorage API**: Seamless persistent bag state across browser refreshes.
