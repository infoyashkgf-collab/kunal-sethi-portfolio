# MY WEBSITE - PERMANENT CONFIGURATION
## Last Updated: 2026-05-26 10:32 AM
## Status: ✅ PRODUCTION READY

---

## 🎯 CRITICAL REQUIREMENT (DO NOT CHANGE)

**Mobile must display EXACTLY like desktop - same layout, same proportions, same everything.**

### Current Setting (KEEP THIS FOREVER):
```html
<meta name="viewport" content="width=1280">
```

### ❌ NEVER USE THESE (breaks mobile-desktop parity):
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0">
```

**WHY:** `width=1280` forces mobile browsers to render at 1280px desktop width and scale down. Users pinch-zoom to navigate. This preserves the exact desktop experience on mobile.

---

## 📁 PROJECT FILES

| File | Purpose | Status |
|------|---------|--------|
| `index.html` | **LIVE WEBSITE** - Current working version | ✅ Active |
| `BACKUP_index_20260525_151118.html` | Backup before May 26 fixes | 📦 Archive |
| `BACKUP_index_20260526_103206.html` | Backup before mobile fix | 📦 Archive |
| `SAVED_20260526_103239/` | "Gold" save - first stable version | 📦 Archive |
| `MY_WEBSITE_PROMPT/` | **This documentation folder** | 📋 Reference |

---

## 🎨 DESIGN SYSTEM (DO NOT CHANGE)

### Colors:
- Primary Gold: `#D4AF37`
- Gold Light: `#FFD700`
- Gold Dark: `#B8860B`
- Background Dark: `#111111`
- Background Darker: `#0A0A0A`
- Text Light: `#E5DDD0`
- Body Text: `#A0A0A0`

### Fonts:
- Headings: `Michroma` (Google Fonts)
- Body: `Montserrat` (Google Fonts)

### Key Sizes:
- Hero H1: `144px` (desktop), scales down proportionally
- Service Labels: `96px`
- Service Headings: `48px`
- Projects Heading: `144px`
- Blend Banner: `72px`

---

## 📱 MOBILE BEHAVIOR (PRESERVE EXACTLY)

### What Mobile Users See:
1. **Exact desktop layout** - no responsive breakpoints active
2. **Zoomed-out view** - entire page visible on screen
3. **Pinch to zoom** - users zoom into sections they want to read
4. **Horizontal scroll** - available if needed

### Why This Works:
- Design is desktop-first and visually dense
- Responsive breakpoints would break the artistic layout
- Users expect to pinch-zoom on portfolio sites
- Maintains visual integrity across all devices

---

## 🚀 GITHUB REPOSITORY

**Repository:** https://github.com/infoyashkgf-collab/kunal-sethi-portfolio
**Live Website:** https://infoyashkgf-collab.github.io/kunal-sethi-portfolio/

### How to Update in Future:
```bash
# After editing index.html:
git add index.html
git commit -m "Description of changes"
git push origin master
# Wait 1-2 minutes for GitHub Pages to update
```

---

## ⚠️ THINGS THAT MUST NEVER CHANGE

1. **Viewport meta tag** - Keep `width=1280` forever
2. **Hero parallax** - Uses translate3d, not background-attachment
3. **"My Skills" button** - Must have explicit width="140" height="140" on SVG
4. **Projects heading** - Fixed position + JS fade, not CSS sticky
5. **Gold theme** - Dark background (#111) with gold accents (#D4AF37)
6. **Circle button SVGs** - Must have explicit width/height attributes
7. **Mobile menu** - Click outside + Escape key to close

---

## 🔧 TECHNICAL NOTES

### Libraries Used:
- **AOS (Animate On Scroll)** - For scroll animations
- **Google Fonts** - Michroma + Montserrat
- **Font Awesome** - Icons (CDN)
- **Vanilla JS** - No frameworks, pure JavaScript

### CDN Links (Active):
```html
<link href="https://fonts.googleapis.com/css2?family=Michroma&family=Montserrat..." rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
<link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
<script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
```

### Parallax Implementation:
```javascript
// Hero parallax uses translate3d for GPU acceleration
window.addEventListener('scroll', () => {
    const scrolled = window.pageYOffset;
    parallaxBg.style.transform = `translate3d(0, ${scrolled * 0.5}px, 0)`;
});
```

### Projects Heading Fade:
- Uses `position: fixed` + JavaScript opacity calculation
- Fades in/out over 400px scroll zone
- Desktop only behavior (no mobile equivalent needed)

---

## 📞 CONTACT INFORMATION (CURRENT)

- **Name:** Kunal Sethi
- **Brand:** dm2develop
- **Phone:** +91 9289109101
- **Email:** sethivayu@gmail.com
- **Location:** Delhi

---

## 🎓 PORTFOLIO CONTENT

### Stats/Marquee:
- "5+ YEARS EXPERIENCE"
- "PROJECTS DELIVERED - 50+"
- "30+ HAPPY CLIENTS"

### Tech Stack (Brand Logos):
React.js, Vue.js, Node.js, Python, WordPress, Shopify, Next.js, Tailwind

### Services (01-08):
1. Frontend Development
2. Backend Development
3. UI/UX Design
4. E-Commerce Solutions
5. Web App Development
6. CMS & WordPress
7. SEO & Performance
8. API Integration

### Projects (6 Demo):
1. E-Commerce Dashboard
2. Analytics Platform
3. Corporate Website
4. Mobile App Interface
5. SaaS Landing Page
6. Portfolio CMS

---

## ✅ CHECKLIST BEFORE ANY EDIT

Before changing anything, verify:
- [ ] Viewport is still `width=1280`
- [ ] No responsive breakpoints being added
- [ ] SVG circle buttons have explicit width/height
- [ ] Test on mobile to ensure desktop parity
- [ ] Test on desktop to ensure no regression
- [ ] Update this document if anything changes

---

## 🆘 EMERGENCY RECOVERY

If something breaks:
1. Check `BACKUP_index_20260526_103206.html` - last known good
2. Check `SAVED_20260526_103239/` - gold save folder
3. Check GitHub commit history for rollback
4. **Never** delete backups until new version is verified

---

**Remember: The user wants EXACT desktop layout on mobile. Never add responsive breakpoints that change the layout. The viewport width=1280 setting is sacred.**

**Created by:** OpenCode AI Agent
**For:** Kunal Sethi / dm2develop
**Date:** May 26, 2026
