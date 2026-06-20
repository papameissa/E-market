# Design System - E-Market

## Brand Identity

**Brand Name:** E-Market  
**Tagline:** "AFFIRMEZ VOTRE STYLE AU QUOTIDIEN" (Assert your style daily)  
**Category:** E-commerce Fashion / Lifestyle  
**Target:** Modern, quality-conscious consumers seeking everyday style

---

## Color Palette

### Primary Colors
- **Emerald Green** (`#006B4E`) - Main brand color, actions, CTAs
- **Emerald Dark** (`#00573f`) - Hover states, accents
- **Beige Soft** (`#EDE6DA`) - Card backgrounds, soft accents

### Neutral Colors
- **Background Page** (`#F8F6F2`) - Warm off-white, entire page background
- **White** (`#FFFFFF`) - Card/section backgrounds
- **Text Dark** (`#1b1b1b`) - Primary text
- **Text Muted** (`#5a5a5a`) - Secondary text, descriptions

### Visual Palette
- **Hero Circle Background** (`#F4EEE3`) - Decorative background behind hero image

---

## Typography

### Font Family
- **Primary Font:** "Inter", "Helvetica Neue", Arial, sans-serif
- **Weight Hierarchy:**
  - **800** (Bold): Headings, labels, section titles
  - **700** (Semi-bold): Product names, buttons
  - **400** (Regular): Body text, descriptions

### Type Scale
| Element | Size | Weight | Line Height | Usage |
|---------|------|--------|-------------|-------|
| H1 (Hero Title) | clamp(3.8rem, 4.8vw, 5.5rem) | 800 | 0.95 | Main hero headline |
| Section Label | 0.85rem | 800 | 1.0 | "NOUVELLE COLLECTION", section headers |
| Section Title | 1rem | 700 | 1.0 | Product names, card headers |
| Body Text | 1.16rem | 400 | 1.7 | Hero description, main body copy |
| Product Desc | 0.88rem | 400 | 1.4 | Small product descriptions |
| Button Text | 1rem | 700 | 1.0 | "DÉCOUVRIR", "AJOUTER AU PANIER" |

---

## Component Library

### Hero Section
- **Background:** White card with soft shadow
- **Shadow:** `0 36px 140px rgba(15, 107, 63, 0.14)`
- **Border Radius:** `2rem`
- **Padding:** `4.5rem 4rem`
- **Grid Layout:** 2 columns (1.05fr / 0.95fr)
- **Min Height:** `620px`
- **Decorative Circle:** Behind image, `#F4EEE3`, `95% width`, `88% height`

### Product Card
- **Border Radius:** `1rem`
- **Shadow:** `0 18px 45px rgba(0, 0, 0, 0.1)` (on hover: `-6px` translateY)
- **Image Height:** `330px` (object-fit: cover)
- **Padding:** `1.2rem 1rem 1.5rem`

### Price Box
- **Background:** `#EDE6DA` (Beige)
- **Padding:** `0.75rem 1rem`
- **Border Radius:** `0.75rem`
- **Old Price:** `#7a7a7a`, line-through, 0.95rem
- **New Price:** `#006B4E` (Emerald), **800 weight**, 1.05rem

### Buttons
- **Primary (Emerald):** `#006B4E` background, white text
- **Padding:** `1.15rem 2.4rem`
- **Border Radius:** `1rem`
- **Shadow:** `0 18px 40px rgba(0, 0, 0, 0.16)`
- **Text Transform:** Uppercase
- **Letter Spacing:** `0.08em`

### Header
- **Background:** `#006B4E` (Emerald)
- **Border Bottom:** 6px solid white
- **Min Height:** 76px
- **Logo Max Height:** 56px

---

## Spacing System

| Scale | Value | Usage |
|-------|-------|-------|
| xs | 0.5rem | Small gaps, inline spacing |
| sm | 1rem | Button padding horizontal, small margins |
| md | 1.25rem | Section margins |
| lg | 2rem | Component gaps, card padding |
| xl | 3rem | Section padding top/bottom |
| 2xl | 4.5rem | Hero padding, large spacing |

---

## Responsive Breakpoints

| Device | Breakpoint | Layout Changes |
|--------|-----------|-----------------|
| Desktop | ≥1200px | Full 2-column hero grid, 4 products per row |
| Tablet | 768px - 1199px | Hero stacks to 1 column, 2 products per row |
| Mobile | <768px | Full width, 1 product per row, reduced padding |

---

## Imagery

### Hero Image
- **Format:** JPEG or PNG, natural product photography
- **Dimensions:** Full container width, contain fit (no crop)
- **Object Fit:** `contain` - shows full product without cropping
- **Border Radius:** `2rem`
- **Max Width:** `680px`

### Product Images
- **Format:** JPEG or PNG, product shot
- **Aspect Ratio:** ~4:5 (portrait)
- **Height:** 330px fixed, object-fit: cover
- **Border Radius:** `1rem`

---

## Interactions

### Hover States
- **Product Card:** `transform: translateY(-6px)`, shadow increase
- **Buttons:** Shadow enhancement, no background color change
- **Links:** Underline appears

### Transitions
- **Duration:** 0.25s ease
- **Properties:** transform, box-shadow

---

## Accessibility

- **Color Contrast:** Emerald on white ≥ 4.5:1
- **Font Sizes:** Minimum 16px on mobile
- **Touch Targets:** All buttons ≥44px × 44px
- **Label Strategy:** Descriptive alt text on all images

---

## Content Guidelines

### Voice & Tone
- **Professional but warm**
- **Product-focused descriptions**
- **Actionable CTAs** (DÉCOUVRIR, AJOUTER)
- **French language**

### Product Information
- **Name:** Product category (T-shirt, Polo, Robe, etc.)
- **Description:** 1 short sentence, benefit-focused
- **Pricing:** Old price (strikethrough) + New price (Emerald, bold)
- **CTA:** "AJOUTER AU PANIER" (Add to Cart)

---

## Files & Structure

```
projet/
├── index.html              # Main landing page
├── css/
│   └── style.css          # All styling (variables, components)
├── assets/
│   ├── hero.jpg           # Hero image
│   ├── homme*.jpg         # Men's clothing products
│   ├── femme*.jpg         # Women's clothing products
│   └── logo.jpeg          # Brand logo
├── DESIGN.md              # This file
└── .stitch/               # Optional: Stitch design assets
    └── DESIGN.md          # Stitch-specific design context
```

---

## Future Enhancements

1. **Dark Mode** - Provide inverted color palette
2. **Product Filters** - Category, size, color, price range
3. **Shopping Cart** - Persistent cart with checkout flow
4. **User Accounts** - Login, order history
5. **Product Details Page** - Full product view with reviews
6. **Search** - Full-text search across products

---

**Last Updated:** 2026-06-16  
**Design System Owner:** E-Market Brand Team  
**Version:** 1.0 (Bootstrap 5.3.2)
