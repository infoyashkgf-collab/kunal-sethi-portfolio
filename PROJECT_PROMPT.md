# dm2develop Portfolio Website - Project Prompt

## Project Overview
**Name:** Kunal Sethi Portfolio (dm2develop)  
**Type:** Single-page portfolio website replicating olive.in design  
**Location:** D:\Projects\my website\index.html  
**Last Updated:** 2026-05-25  
**Theme:** Gold & Dark (Luxury)  

---

## Color Theme
| Element | Color | Hex Code |
|---------|-------|----------|
| Primary Gold | #D4AF37 | Buttons, accents, hover states |
| Dark Gold | #B8860B | Gradients, hover backgrounds |
| Light Gold | #FFD700 | Highlights |
| Muted Gold | #8B7355 | Subtle accents |
| Background Dark | #111111 | Main sections |
| Background Darker | #0A0A0A | Services, deeper sections |
| Text Light | #F5F5F0 | Cream/white text |
| Text Gray | #A0A0A0 | Body text, descriptions |
| Pure White | #FFFFFF | Nav links, headings |
| Border Gray | #444444 | Dividers, borders |

---

## Sections (Top to Bottom)

### 1. Header/Navigation
- **Position:** Fixed/Absolute, z-index: 999
- **Background:** Semi-transparent black (rgba(0,0,0,0.5)) / Solid black on sticky
- **Logo:** dm2develop (Michroma font, white, turns gold on sticky)
- **Nav Links:** About, Services, Portfolio, Contact Us
- **CTA:** "Get In Touch" button (gold background)
- **Mobile:** Hamburger menu with full-screen overlay

### 2. Hero Banner
- **Height:** 1000px (700px mobile)
- **Background:** Parallax image with overlay
- **Text:** "How I help you" + "CODE WITH CONFIDENCE"
- **Effect:** Parallax scroll via JS translate3d

### 3. Blend Banner (About)
- **Height:** 800px
- **Background:** Image with dark overlay (rgba(17,17,17,0.7))
- **Text:** Tagline + "BUILD · DEPLOY · EXCEL"
- **Effect:** Background-attachment: fixed

### 4. Services
- **Background:** #0A0A0A
- **Title:** "A FULL STACK APPROACH, BESPOKE & COLLABORATIVE"
- **Items:** 8 services (01-08) with gradient gold numbers
- **Layout:** Label (25%) + Offer (75%) + Arrow icon
- **Hover:** Arrow SVG stroke animation

### 5. Projects
- **Background:** #111111
- **Heading:** "PROJECTS" - sticky/fixed centered with fade animation
- **Layout:** Masonry grid, 2 columns, staggered (25% offset)
- **Items:** 6 project cards with images
- **Effect:** Fade in/out on scroll via IntersectionObserver

### 6. Brand/Stats Marquee
- **Background:** #111111
- **Marquee:** "5+ YEARS EXPERIENCE", "PROJECTS DELIVERED - 50+", "30+ HAPPY CLIENTS"
- **Animation:** Infinite horizontal scroll (CSS animation)
- **Tech Stack:** 8 circular icons with labels (React, Vue, Node, etc.)
- **CTA:** "My Skills" circle button with gold stroke animation

### 7. Contact/Enquiry
- **Background:** #111111
- **Form:** First Name, Last Name, Company, Mobile, Email
- **Submit:** Gold button
- **Info:** Phone (+91 9289109101), Email (sethivayu@gmail.com), Location (Delhi)

### 8. Footer
- **Background:** #111111
- **Logo:** dm2develop
- **Links:** About, Services, Portfolio, Contact Us
- **Social:** LinkedIn, GitHub (gold icons)
- **Copyright:** 2026 dm2develop by Kunal Sethi

---

## Key CSS Values

### Typography
- Hero H1: 144px / 205px (Michroma)
- Section Titles: 60px / 80px (Michroma)
- Service Numbers: 96px / 100px (Michroma, gradient gold)
- Service Headings: 48px / 59px (Montserrat)
- Body Text: 18px / 35px (Montserrat)
- Nav Links: 16px / 20px (Montserrat)

### Layout
- Container: max-width: 1280px, margin: 0 auto, padding: 0 15px
- Section Padding: 50px 0 (standard), 100px 0 (large)
- Grid: Bootstrap-style (col-md-6, col-lg-3, etc.)

### Animations
- AOS (Animate On Scroll): fade-up, delay 300ms
- Circle Button: SVG stroke-dashoffset 530→1060px
- Sticky Header: Animation 1.2s
- Marquee: 20s, 40s, 15s linear infinite
- Projects Heading: Fade in/out on scroll (400px zone)

---

## JavaScript Features
1. **Sticky Header:** Adds .sticky class after 100px scroll
2. **Parallax Hero:** translate3d on scroll
3. **Mobile Menu:** Toggle fullscreen overlay
4. **Smooth Scroll:** For anchor links
5. **Projects Fade:** IntersectionObserver-based opacity
6. **AOS Library:** Scroll-triggered animations

---

## Contact Information
- **Name:** Kunal Sethi
- **Brand:** dm2develop
- **Phone:** +91 9289109101
- **Email:** sethivayu@gmail.com
- **Location:** Delhi, India

---

## Files
- **Main:** index.html (single file, all CSS/JS inline)
- **Assets:** External (Google Fonts, Font Awesome, AOS, Unsplash images)
- **Backup:** Auto-created with timestamp

---

## Important Notes
1. All colors use gold (#D4AF37) as primary accent
2. Dark backgrounds (#111111, #0A0A0A) for luxury feel
3. White (#FFFFFF) for maximum readability on dark
4. Parallax effect requires images with proper contrast
5. Mobile responsive: 991px, 767px breakpoints
6. No external frameworks (Bootstrap CSS inlined)
7. Single-file architecture for easy deployment

---

## To Modify
1. Replace placeholder projects with real portfolio items
2. Add actual LinkedIn/GitHub links
3. Update Unsplash images with real project screenshots
4. Add reCAPTCHA site key for form security
5. Consider adding Google Analytics

---

**Status:** ✅ COMPLETE - All sections working, all colors applied, all animations functional
**Next Steps:** Add real content, deploy to hosting
