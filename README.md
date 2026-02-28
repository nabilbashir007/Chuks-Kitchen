# Chuks Kitchen – Frontend Web Project

## Project Overview
**Client:** Mr. Chukwudi Okorie (Mr. Chuks) | **Business:** Chuks Kitchen  
**Prepared by:** Nabil Bashir, Frontend Developer 
**Period:** Feb 13 – Feb 27, 2025

6 responsive static pages for a Nigerian food ordering platform, converted pixel-accurately from Figma designs using plain HTML, CSS, and JavaScript.

---

## Tech Stack
| Tool | Purpose |
|------|---------|
| HTML5 | Semantic page structure |
| CSS3 | Styling using exact Figma color/font/spacing values |
| Vanilla JavaScript | Cart interactions, toggles, nav |
| Google Fonts | Island Moments (logo), Inter (body), Jost + Poppins (footer) |

No frameworks. No build tools. Open any `.html` file in a browser.

---

## Project Structure
```
chuks-kitchen/
├── index.html              # Welcome / Landing page
├── signin.html             # Sign In page
├── signup.html             # Create Account page
├── cart.html               # Your Cart page
├── order-summary.html      # Order Summary page
├── delivery-details.html   # Delivery Details page
├── css/
│   └── style.css           # All styles (shared + page-specific via <style> blocks)
├── js/
│   └── main.js             # Shared JS: nav toggle, back-to-top, password toggle
└── assets/                 
    ├── Rectangle 1.jpg            
    ├── Food 1.jpg           
    ├── Food 2.jpg
    ├── Food 3.jpg
    └── Food 4.jpg
```

---

## Design Decisions (from Figma Specs)

### Colors
| Variable | Hex | Usage |
|----------|-----|-------|
| `--orange` | `#FF7A18` | Primary buttons, logo accent, active nav |
| `--blue` | `#1E88E5` | Secondary buttons, links, forgot password |
| `--blue-light` | `#64B5F6` | Privacy/Terms links on Welcome page |
| `--dark` | `#1F2937` | Body text, total amount |
| `--gray-bg` | `#F3F4F6` | Page backgrounds (Cart, Order Summary, Auth pages) |
| `--gray-border` | `#BDBDBD` | Input borders, cart item borders, Pickup button |
| Footer BG | `linear-gradient(rgba(255,122,24,0.3), rgba(255,122,24,0.3)), #1F2937` | Footer |

### Typography
| Font | Usage | Source |
|------|-------|--------|
| Island Moments 400 | "Chuks Kitchen" logo everywhere | Google Fonts |
| Inter 700 32px | Page headings, cart item names | Google Fonts |
| Inter 600 16px | Button labels, nav Login button | Google Fonts |
| Inter 500 16px | Nav links, body paragraphs, feature items | Google Fonts |
| Inter 500 24px | Section titles (Order Summary labels) | Google Fonts |
| Jost 400 24px | Footer column headings | Google Fonts |
| Poppins 400 12px | Footer body text (opacity 0.75) | Google Fonts |

### Navbar Differences (per Figma)
- **Welcome page**: Sign In button is **outlined blue** (border: 2px solid #1E88E5)
- **Cart / Order Summary / Delivery pages**: Login button is **solid orange** (#FF7A18)
- **Auth pages (Sign In / Sign Up)**: No nav links, logo only

### Feature Icons (Welcome page)
- Icon container: 44×44px, background `#FFE1C4`, border-radius `13px`
- Icon fill: `#FF7A18`
- Layout: flex-row wrap, gap `19px 70px`

### Cart Page
- Item name: Inter 700 **32px** (large, as per Figma)
- Item description: Inter 500 **24px** `#4B5563`
- Quantity number: Inter 500 **51.5px**
- Remove icon: orange X SVG (cancel-presentation-rounded)
- Item border: `0.5px solid #BDBDBD`, border-radius `5px`

### Order Summary Page
- Delivery button: `#FF7A18`, border-radius `8px 0 0 8px`
- Pickup button: `#BDBDBD` (grey), border-radius `0 8px 8px 0`
- Total amount: `#1F2937` (dark, NOT orange)
- Promo apply button label: "Login" (as per Figma)

---

## Assumptions Made
1. **Delivery Details** —  Included as a bonus page beyond the required 5.
2. **Auth page navbar** — Figma shows no nav links on Sign In/Sign Up screens, only the logo. Implemented as-is.

---

## Limitations & Improvements
- No backend/API (per project scope)
- Form validation is HTML-only; real validation would use JS
- Cart state resets on refresh — localStorage could persist it

---


**Page flow:** `index.html` → `signin.html` / `signup.html` → `cart.html` → `order-summary.html` → `delivery-details.html`
