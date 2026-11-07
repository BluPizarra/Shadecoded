# Shadecoded — Your shade, but make it perfect.

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![UI/UX Design](https://img.shields.io/badge/UI%2FUX-Design%20Prototype-B3665B?style=for-the-badge)](https://github.com/BluPizarra/Shadecoded)

> **Cross-brand foundation shade intelligence prototype designed with formula-first guidance, real-time lighting simulations, and user-centered design principles.**

Developed by **Bludylan Cyrus A. Pizarra** for the **User Experience Design ([USERDES])** course final requirement.

---

## 🌟 Overview & Problem Statement

Finding the correct foundation shade across beauty brands is notoriously frustrating. Different cosmetic houses use divergent shade-naming systems (e.g., MAC’s inverted NC/NW system vs. Fenty’s 3-digit numbering vs. L'Oréal’s letter-number codes), while environmental lighting and skin oxidation cause foundations that looked perfect in-store to appear mismatched in daylight.

**Shadecoded** addresses this challenge with an intuitive, human-centered web application that translates foundation shades across 5 major formula houses, simulates real-world lighting conditions, accommodates seasonal skin tone shifts, and flags formula-skin compatibility issues.

---

## 🗂️ Organized Project Architecture

```text
Shadecoded/
├── index.html                           # Main entry point (GitHub Pages ready)
├── shadecoded.html                      # Standalone full application file
├── [USERDES] PIZARRA_SHADECODED.html    # Academic submission alias
├── assets/
│   └── swatches/                        # High-resolution foundation swatches & brand assets
│       ├── fenty.jpg
│       ├── fenty_swatch.jpg
│       ├── loreal.jpg
│       ├── loreal_swatch.jpg
│       ├── mac.jpg
│       ├── mac_swatch.jpg
│       ├── maybelline.jpg
│       ├── maybelline_swatch.jpg
│       ├── nars.jpg
│       └── nars_swatch.webp
├── archive/
│   └── v1_prototype/                    # Initial exploration & early design iterations
│       ├── index_v1.html
│       ├── styles_v1.css
│       ├── app_v1.js
│       ├── Untitled-1.html
│       ├── Copilot_20260808_181745.png
│       └── README_v1.md
├── .gitignore
└── README.md                            # Comprehensive project documentation
```

### ✨ Key Organizational Highlights
- **Production-Ready Web Hosting**: `index.html` provides seamless root access out-of-the-box for GitHub Pages and static web servers.
- **Academic Submission Parity**: Preserves `shadecoded.html` and `[USERDES] PIZARRA_SHADECODED.html` aliases to satisfy institutional grading requirements.
- **Modular Asset Separation**: Extracted brand swatches and reference photography into `assets/swatches/` while archiving early prototype iterations in `archive/v1_prototype/`.
- **Zero External Runtime Dependencies**: Built entirely with vanilla web standards (HTML5, responsive CSS Grid/Flexbox, native JavaScript ES6+, and Google Fonts).

---

## 🚀 Key Features

### 1. 🔍 Cross-Brand Shade Intelligence Matrix
- Comprehensive **15 skin-tone matrix rows** spanning **Fair, Light, Light-Medium, Medium, Tan, and Deep** depths across **Cool, Neutral, and Warm** undertones.
- Direct cross-lookup among 5 global foundation leaders:
  - **MAC**: *Studio Fix Fluid* (NC / NW notation)
  - **Fenty Beauty**: *Pro Filt'r Soft Matte* (100–490 series)
  - **Maybelline**: *Fit Me Matte + Poreless* (100–300 series)
  - **L'Oréal Paris**: *True Match Super-Blendable* (C / N / W notation)
  - **NARS**: *Light Reflecting & Sheer Glow* (Named shades, e.g., Mont Blanc, Deauville, Syracuse)

### 2. 💡 Dynamic Real-Time Lighting Visualizer
Simulate how your selected shade swatch responds to real environmental color temperatures:
- **Daylight (5500K)** — High-CRI natural sky reference for true color evaluation.
- **Office Fluorescent (4000K)** — Cool office lighting highlighting oxidation and ashiness.
- **Golden Hour (3200K)** — Warm afternoon sun accentuating golden/olive undertones.
- **Evening Candlelight (2400K)** — Low warm ambiance simulating dinner and event settings.

### 3. 📸 Client-Side Photo Shade Scanner
- Interactive photo upload modal allowing users to test skin tone and undertone balance directly in the browser.
- **Privacy-first**: Images are processed strictly on client-side memory using `URL.createObjectURL` and never uploaded to remote servers.

### 4. ☀️ Seasonal Tone Adjustment
- One-click seasonal toggle (**Winter Pale**, **True Match**, **Summer Tan**) that dynamically shifts recommendations by ±1 tone depth to match natural melanin cycles.

### 5. 🔬 Skin Type & Ingredient Compatibility Checker
- Evaluates skin conditions (**Oily, Dry, Combination, Sensitive**) against formula components (Silicones, Perlite/Clay, Skincare Botanicals, Denatured Alcohol, Fragrance) with clear warnings and recommendations.

### 6. 🌓 Responsive Design & Dark Mode
- Full dark/light mode toggle with smooth CSS variable transitions (`body.dark-lighting`).
- Tactile, editorial design aesthetic featuring typography from **Fraunces**, **Inter**, and **IBM Plex Mono**.
- Accessible keyboard navigation and mobile-responsive layout.

### 7. 🗳️ Interactive Community Polls
- Embedded real-time polling widget capturing user feedback on formula longevity, shade breadth, and skin-type preferences.

---

## 🎨 Color Palette & Typography

### Design System Colors

| Token Name | Hex Code | Visual Swatch | Role |
| :--- | :--- | :---: | :--- |
| `--paper` | `#FBF9F5` | ![#FBF9F5](https://placehold.co/16x16/FBF9F5/FBF9F5.png) | Warm parchment background (Light mode) |
| `--card` | `#F2EFE9` | ![#F2EFE9](https://placehold.co/16x16/F2EFE9/F2EFE9.png) | Elevated card surface |
| `--line` | `#EAE5DD` | ![#EAE5DD](https://placehold.co/16x16/EAE5DD/EAE5DD.png) | Subtle architectural dividers |
| `--ink` | `#1A1A1A` | ![#1A1A1A](https://placehold.co/16x16/1A1A1A/1A1A1A.png) | Primary body and heading typography |
| `--ink-soft` | `#5B5650` | ![#5B5650](https://placehold.co/16x16/5B5650/5B5650.png) | Secondary descriptions and metadata |
| `--rose` | `#B3665B` | ![#B3665B](https://placehold.co/16x16/B3665B/B3665B.png) | Primary brand accent & interactive focus |
| `--rose-soft` | `#E3C6BE` | ![#E3C6BE](https://placehold.co/16x16/E3C6BE/E3C6BE.png) | Cool undertone reference |
| `--gold` | `#B79A5B` | ![#B79A5B](https://placehold.co/16x16/B79A5B/B79A5B.png) | Warm undertone reference |
| `--plum` | `#4A3A44` | ![#4A3A44](https://placehold.co/16x16/4A3A44/4A3A44.png) | Neutral undertone reference |

### Typography Hierarchy
- **Editorial Headings**: `Fraunces` (variable optical sizes, serif)
- **Body & Controls**: `Inter` (geometric sans-serif)
- **Technical Codes & Labels**: `IBM Plex Mono` (monospaced)

---

## 💻 How to View & Run Locally

### 1. Clone the Repository
```bash
git clone https://github.com/BluPizarra/Shadecoded.git
cd Shadecoded
```

### 2. Open in Any Browser
Simply double-click `index.html` or `shadecoded.html`, or launch using a local static server:

```bash
# Python 3
python -m http.server 8000

# Node / npx
npx serve .
```
Navigate to `http://localhost:8000` in your web browser.

---

## 🌐 Live GitHub Pages Deployment

To enable free instant hosting on GitHub Pages:
1. Go to **Settings** > **Pages** in the [GitHub Repository](https://github.com/BluPizarra/Shadecoded).
2. Under **Build and deployment**, select **Deploy from a branch**.
3. Choose branch `main` and folder `/ (root)`.
4. Click **Save**. The live URL will be accessible at:
   `https://blupizarra.github.io/Shadecoded/`

---

## 🎓 Academic Information

- **Student Name**: Bludylan Cyrus A. Pizarra
- **Course**: User Experience Design ([USERDES])
- **Academic Year / Term**: 2nd Year, Term 1
- **Project Topic**: Precision Cross-Brand Foundation Shade Intelligence & Matrix Lookup System
- **Repository**: [https://github.com/BluPizarra/Shadecoded](https://github.com/BluPizarra/Shadecoded)
