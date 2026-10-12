# StreetMagicLab.com — Complete Website Analysis for Replication

> **Platform:** Payhip (custom domain storefront)
> **Domain:** streetmagiclab.com
> **Owner:** Sanad Diab (dba "Card Craft")
> **Contact:** contact@streetmagiclab.com
> **Payhip Seller Username:** BeginnerCardMagic

---

## 1. SITE ARCHITECTURE & URL STRUCTURE

### Pages Discovered

| URL | Type | Title |
|-----|------|-------|
| `/` | Homepage / Storefront | Street Magic Lab |
| `/3-free-self-working-tricks` | Custom sales/landing page | Magic-Masterclass (main sales page) |
| `/b/4Wpkr` | Course product page | Magic Tricks for Beginners: Card, Coin & Street Magic |
| `/b/n8IWh` | Course product (main offer) | Card Craft: Full System |
| `/b/qGQTw` | Mini course | Do That Again Prediction |
| `/b/ojAPI` | Mini course | Mind Reading / Thought-Of Card |
| `/b/nYCdg` | Mini course | 8 Card Brainwave |
| `/b/lSXuW` | Mini course | Simple Yet Deceptive Card Trick |
| `/b/zuiOS` | Mini course | The Three Dice Card Trick |
| `/b/5inzX` | Mini course | Three Card Monte |
| `/b/9-professional-self-working-card-tricks-anyone-can-do-bvu9` | Bundle product | Complete Collection (all 9 tricks) |
| `/blog/card-magic-guides` | Blog category | Card Magic Guides |
| `/blog/card-magic-guides/card-magic-for-beginners-how-to-actually-learn-it` | Blog post | Card Magic for Beginners |
| `/order?link=...&pricing_plan=...` | Payhip checkout | Checkout pages |

### URL Pattern Notes
- Product pages use Payhip's `/b/{shortcode}` format
- Custom landing pages use clean slugs (`/3-free-self-working-tricks`)
- Blog follows `/blog/{category}/{post-slug}` structure
- Checkout uses `/order?link={productId}&pricing_plan={planId}`
- Login at: `payhip.com/BeginnerCardMagic/users/login`

---

## 2. BRAND IDENTITY & DESIGN SYSTEM

### Brand Name
- **Primary:** Street Magic Lab
- **Product name:** Card Craft
- **Legal:** Card Craft — Sanad Diab
- **Copyright:** © 2026 Card Craft — Sanad Diab. All rights reserved.

### Logo
- **URL:** `https://payhip.com/cdn-cgi/image/format=auto,width=300/https://pe56d.s3.amazonaws.com/o_1jcubent1sl91kmo14ha7gh1coe13.png`
- **Alt text:** "Street Magic Lab Logo"
- **Placement:** Top-left of header, links to homepage

### Favicon
- **URL:** `https://payhip.com/cdn-cgi/image/format=auto/https://pe56d.s3.amazonaws.com/o_1jmopmagv1dtg18vfr331o393cd12.png`

### OG / Social Share Image
- **URL:** `https://payhip.com/cdn-cgi/image/format=auto/https://pe56d.s3.amazonaws.com/o_1k40h51m31te8qa516ue1m861tg1g.png`

### CSS Custom Properties (`:root`)
```css
:root {
  --orange: #E8651A;
  --orange-dark: #C4500E;
  --gold: #C9A84C;
  --gold-light: #F0DC8A;
  --dark: #0d0d12;
  --dark2: #111118;
  --dark3: #1a1a24;
  --light: #F9F8F6;
  --white: #FFFFFF;
  --text: #17171A;
  --muted: #52525B;
  --border: #E4E3DF;
  --green: #16a34a;
  --green-l: #4ade80;
  --sans: 'DM Sans', system-ui, sans-serif;
  --serif: 'DM Serif Display', Georgia, serif;
  --nav-w: 230px;
  --sh: 0 1px 2px rgba(0,0,0,.04), 0 4px 20px rgba(0,0,0,.06);
  --sh-lg: 0 8px 40px rgba(0,0,0,.14);
}
```

### Complete Color Palette

#### Primary Brand Colors
| Hex | CSS Var | Usage |
|-----|---------|-------|
| `#E8651A` | `--orange` | Primary CTA buttons, accents, highlights |
| `#C4500E` | `--orange-dark` | Hover states for orange buttons |
| `#C9A84C` | `--gold` | Badges, premium accents |
| `#F0DC8A` | `--gold-light` | Gold text highlights via gradient |

#### Dark Backgrounds
| Hex | CSS Var | Usage |
|-----|---------|-------|
| `#0d0d12` | `--dark` | Darkest background |
| `#111118` | `--dark2` | Dark section backgrounds |
| `#1a1a24` | `--dark3` | Dark card backgrounds |
| `#212121` | — | Nav panel background |
| `#18181b` | — | Stats bar background |
| `#1c1917` | — | Dark card variant |

#### Light Backgrounds
| Hex | CSS Var | Usage |
|-----|---------|-------|
| `#F9F8F6` | `--light` | Light section backgrounds |
| `#FFFFFF` | `--white` | White |
| `#faf9f6` | — | Off-white sections |
| `#fefce8` | — | Yellow tint highlight cards |
| `#fffbeb` | — | Amber tint |
| `#f5f5f4` | — | Stone-50 |

#### Text Colors
| Hex | CSS Var | Usage |
|-----|---------|-------|
| `#17171A` | `--text` | Primary body text |
| `#52525B` | `--muted` | Muted/secondary text |
| `#a1a1aa` | — | Zinc-400 (text on dark) |
| `#d4d4d8` | — | Zinc-300 (text on dark) |
| `#71717a` | — | Zinc-500 |
| `#3f3f46` | — | Zinc-700 |
| `#27272a` | — | Zinc-800 |

#### Borders & Dividers
| Hex | CSS Var | Usage |
|-----|---------|-------|
| `#E4E3DF` | `--border` | Primary border |
| `#e7e5e4` | — | Stone-200 |
| `#d6d3d1` | — | Stone-300 |
| `#27272a` | — | Dark borders |

#### Green (Guarantee/Success)
| Hex | CSS Var | Usage |
|-----|---------|-------|
| `#16a34a` | `--green` | Guarantee badge, success |
| `#4ade80` | `--green-l` | Light green accent |
| `#15803d` | — | Green-700 |
| `#166534` | — | Green-800 |
| `#14532d` | — | Green-900 |
| `#052e16` | — | Green-950 |
| `#f0fdf4` | — | Green-50 (light bg) |

#### Other Accent Colors
| Hex | Usage |
|-----|-------|
| `#eab308` | Yellow-500 (star ratings) |
| `#fbbf24` | Amber-400 |
| `#fcd34d` | Amber-300 |
| `#ef4444` | Red (sale/urgency) |
| `#dc2626` | Red-600 |
| `#3b82f6` | Blue (Payhip default, overridden to orange via JS) |
| `#F5C76A` | Gold hover in nav |

**Color Scheme:** Dark theme overall with light sections for contrast

### Typography

#### Font Families
- **Primary sans:** `'DM Sans', system-ui, sans-serif` (`--sans`)
- **Serif/display:** `'DM Serif Display', Georgia, serif` (`--serif`)
- **Payhip base:** `proxima-nova` (Adobe Typekit, loaded by Payhip)

#### Google Fonts Loaded
```html
<link href="https://fonts.googleapis.com/css2?family=DM+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;1,400&family=DM+Serif+Display:ital@0;1&display=swap" rel="stylesheet">
```

#### Complete Type Scale
| Element | Font | Size | Weight | Line-height | Notes |
|---------|------|------|--------|-------------|-------|
| Body | DM Sans | 16px | 400 | 1.6 | color: var(--text) |
| H1 | DM Serif Display | clamp(1.55rem, 5.8vw, 3.3rem) | 700 | 1.1 | Responsive scaling |
| H2 (.h2) | DM Serif Display | clamp(1.7rem, 4vw, 2.5rem) | — | 1.15 | |
| H3 equiv | DM Serif Display | clamp(1.2rem, 3vw, 1.55rem) | — | 1.25 | |
| Eyebrow | DM Sans | 0.72rem | 700 | — | uppercase, letter-spacing: 0.1em |
| Sub (subtitle) | DM Sans | 1.05rem | 400 | 1.55 | color: var(--muted) |
| Button text | DM Sans | 0.95rem | 700 | — | |
| Hero sub | DM Sans | 1.08rem | 400 | 1.5 | |
| Small/fine print | DM Sans | 0.82–0.88rem | 400–500 | — | |
| Stat numbers | DM Serif Display | clamp(1.3rem, 3vw, 1.9rem) | — | 1 | |
| Nav links | DM Sans | 0.92rem | 500 | — | |

### Component Design Tokens

#### Primary CTA Button (Hero)
```css
.btn-hero-main {
  background: var(--orange);
  color: #fff;
  border-radius: 10px;
  padding: 1rem 2.2rem;
  font-weight: 700;
  font-size: 0.95rem;
  box-shadow: 0 4px 15px rgba(232,101,26,0.35);
  transition: transform 0.2s, box-shadow 0.2s;
}
.btn-hero-main:hover {
  transform: translateY(-2px);
  box-shadow: 0 6px 20px rgba(232,101,26,0.45);
}
```

#### Standard Orange Button
```css
.btn-orange {
  background: var(--orange);
  color: #fff;
  padding: 0.85rem 2rem;
  border-radius: 10px;
  font-weight: 700;
}
```

#### Outline Button
```css
.btn-outline {
  padding: 0.65rem 1.5rem;
  border: 1px solid var(--border);
  border-radius: 8px;
}
```

### Layout System

#### Container Widths
```css
.wrap     { max-width: 1100px; margin: 0 auto; padding: 0 1.25rem; }
.wrap-sm  { max-width: 760px;  margin: 0 auto; padding: 0 1.25rem; }
.wrap-xs  { max-width: 600px;  margin: 0 auto; padding: 0 1.25rem; }
```

#### Full-Width Dark Section Technique
```css
.testi-section, .why-section, .bonus-section, .tv-section, .curriculum-section {
  width: 100vw !important;
  position: relative !important;
  left: 50% !important;
  right: 50% !important;
  margin-left: -50vw !important;
  margin-right: -50vw !important;
  background-color: var(--dark2) !important;
}
```

#### Spacing Scale
| Token | Value | Usage |
|-------|-------|-------|
| xs | 0.25rem (4px) | Tight gaps between inline elements |
| sm | 0.5rem (8px) | Small padding inside chips/badges |
| md | 0.75–1rem (12–16px) | Card inner padding, button padding |
| lg | 1.25rem (20px) | Container side padding, gap between cards |
| xl | 2rem (32px) | Section inner spacing |
| 2xl | 2.5rem (40px) | Gap between major elements |
| 3xl | 3rem (48px) | Mobile section padding |
| 4xl | 4.5rem (72px) | Desktop section padding |

#### Section Spacing Pattern
```css
/* Desktop */ padding: 4.5rem 0;
/* Mobile */  padding: 3rem 0;
/* Between elements */ margin-bottom: 2rem;
/* Heading to content */ margin-bottom: 1.5rem;
```

#### Gap Patterns
```css
.hero-inner { gap: 3.5rem; }     /* Hero columns */
/* Card grids */    gap: 1.5rem;  /* Standard card gap */
/* Carousel */      gap: 1.25rem; /* Between carousel cards */
/* Stat items */    gap: 2rem;    /* Between stat blocks */
```

### Responsive Breakpoints
1. `1024px` + `pointer:coarse` — Payhip tablet
2. `799px` — Payhip mobile
3. **`768px`** — Primary custom mobile breakpoint
4. `720px` — Secondary
5. `640px` — Smaller adjustments
6. `620px` / `600px` — Narrow phone
7. `480px` — Small phone

#### At 768px and below:
- Hero switches to single column (`flex-direction: column`)
- Nav panel converts to full-screen overlay
- Sticky bottom CTA bar becomes visible
- Carousels show 1 card instead of 2-3
- Section padding reduces from 4.5rem to 3rem

### Gradients
1. **Orange divider line:** `linear-gradient(90deg, var(--orange), var(--gold))` — 3px height, 48px width
2. **Green guarantee badge:** `linear-gradient(135deg, var(--green), #15803d)`
3. **Hero ambient glow:** `radial-gradient(ellipse at 70% 50%, rgba(232,101,26,0.08) 0%, transparent 70%)`
4. **Final CTA ambient glow:** `radial-gradient(ellipse at center, rgba(232,101,26,0.06) 0%, transparent 60%)`
5. **Reveal badge gradient:** `linear-gradient(135deg, var(--orange), var(--gold))`
6. **Orange button hover:** `linear-gradient(135deg, #E8651A, #C4500E)`
7. **Dark section overlay:** `linear-gradient(180deg, var(--dark2) 0%, var(--dark) 100%)`
8. **Gold text gradient:** `linear-gradient(90deg, var(--gold), var(--gold-light))` with `-webkit-background-clip: text`

### Framework & Architecture
- **Layout:** Pure Flexbox (no CSS Grid used anywhere)
- **Payhip loads:** Bootstrap 4.4.1, jQuery 3.4.1, Popper.js 1.16.0
- **Custom sections do NOT rely on Bootstrap classes** — all custom CSS
- **Main custom CSS:** 516 rules in a single style block (~64,160 chars)
- **Tone:** Playful
- **Energy:** High
- **Target Audience:** Enthusiasts of magic and card tricks

---

## 3. META TAGS & SEO

### Homepage Meta
```html
<title>Street Magic Lab</title>
<meta name="description" content="Sanad Diab's complete program. 34 lessons + 9 self-working miracle tricks + 9 word-for-word scripts. As seen on 5 national TV shows. 30-day guarantee. $47 one-time.">
<meta name="viewport" content="width=device-width, minimum-scale=1, maximum-scale=1">
<meta name="googlebot" content="noindex,indexifembedded">
```

### Open Graph Tags
```html
<meta property="og:title" content="Street Magic Lab">
<meta property="og:description" content="Sanad Diab's complete system. 34 lessons + 9 self-working miracle tricks + 9 word-for-word scripts. As seen on 5 national TV shows.">
<meta property="og:url" content="https://streetmagiclab.com">
<meta property="og:image" content="https://payhip.com/cdn-cgi/image/format=auto/https://pe56d.s3.amazonaws.com/o_1k40h51m31te8qa516ue1m861tg1g.png">
<meta property="og:type" content="website">
<meta property="og:site_name" content="Street Magic Lab">
```

### Twitter Card Tags
```html
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="Street Magic Lab">
<meta name="twitter:site" content="Street Magic Lab">
<meta name="twitter:url" content="https://streetmagiclab.com">
<meta name="twitter:image" content="[same as og:image]">
```

---

## 4. HEADER / NAVIGATION

### Payhip Default Header (Hidden)
The default Payhip header (`header.header-section-wrapper`, `nav.navbar`) is hidden via a MutationObserver in JavaScript:
```javascript
var obs = new MutationObserver(function() {
  var h = document.querySelector('header.header-section-wrapper');
  if (h) h.style.display = 'none';
});
obs.observe(document.body, { childList: true, subtree: true });
```

### Custom Sticky Header
- **Element:** `.sml-header-bar` (fixed positioning, z-index 500, height 70px)
- **Logo:** Street Magic Lab logo (top-left), links to homepage
- **Nav toggle button:** `#navToggle` (fixed, z-index 501)

### Side Navigation Panel
- **Element:** `#navPanel` (fixed left sidebar, width 230px, slides from left)
- **Background:** `#212121`
- **Links (with scroll tracking):**
  - `#top` — Home
  - `#curriculum` — Full Curriculum
  - `#proof` — Student Reactions
  - `#about` — About Sanad
  - `#tv-shows` — TV Appearances
  - `#bonuses` — Bonuses
  - `#enroll` — Get Access
  - `#faq` — FAQ
  - Private Coaching (opens modal)
- **Active state:** Scroll position tracked via `IntersectionObserver`, active link highlighted

### Payhip Default Header (Other Pages)
On non-custom pages, the standard Payhip header shows:
- **Banner Image:** Full-width header image (the OG image, 1500px wide)
- **Search bar:** "View all results" search functionality
- **Cart icon:** Shopping cart with item count (badge showing "0")
- **Login link:** Links to `payhip.com/BeginnerCardMagic/users/login`
- **Mobile menu:** Hamburger menu on mobile

---

## 5. HOMEPAGE CONTENT (streetmagiclab.com/)

The homepage is a custom-built landing page (NOT the default Payhip storefront). It mirrors the sales page structure but has distinct content — different hero headline, different pricing display, different promo code, and social media links.

### Homepage vs Sales Page Differences
| Element | Homepage (`/`) | Sales Page (`/3-free-self-working-tricks`) |
|---------|---------------|-------------------------------------------|
| Hero headline | "Magic Tricks for Beginners: Card, Coin & Street Magic" | "Learn Card Magic in 30 Days and Amaze Anyone" |
| Hero eyebrow | "Seen on National TV" with dot indicator | "Free Magic Masterclass" |
| Pricing display | "$47 ~~$61~~ (30% off)" | "Worth $160 / For Just: $47" |
| Promo code | `MAGIC` (20% off) | `STREET25` (25% off) |
| Hero video | Vimeo facade (desktop+mobile) | Gumlet player (24:38 masterclass) |
| Social links | Instagram, YouTube, TikTok in footer | Not present |

### Homepage Hero Structure
```html
<div class="hero" id="top">
  <div class="hero-inner">
    <div class="hero-left">
      <div class="hero-eyebrow"><span class="hero-eyebrow-dot"></span>Seen on National TV</div>
      <div class="hero-video-wrap-mobile"><!-- Vimeo facade (mobile only) --></div>
      <h1>Magic Tricks for Beginners: Card, Coin &amp; Street Magic</h1>
      <p class="hero-sub">...</p>
      <div class="hero-rating">...</div>
      <div class="desktop-only-bullets"><!-- 3 bullet items --></div>
    </div>
    <div class="hero-right">
      <div class="hero-video-wrap"><!-- Vimeo facade (desktop) --></div>
      <div class="hero-right-cta-desktop">
        <a href="...order..." class="btn-hero-main">Start Learning Card Magic Today</a>
        <div>$47 <span style="text-decoration:line-through">$61</span> (30% off)</div>
        <div class="hero-trust-row">
          <span class="trust-chip trust-chip-green">30-Day Guarantee</span>
          <span class="trust-chip">Lifetime access</span>
        </div>
      </div>
      <div class="hero-right-cta-mobile"><!-- same CTA for mobile --></div>
    </div>
  </div>
</div>
```

### Homepage Section Order (with eyebrow labels)
1. **Hero** — "Seen on National TV"
2. **What You'll Learn** (`.wyl-section`)
3. **Stats Bar** — dark bar with 4 stat items
4. **Reviews Bar** — star ratings
5. **Curriculum** (`.curriculum-section#curriculum`)
6. **Testimonials** (`.testi-section#proof`) — carousel
7. **Why This Course** (`.why-section`)
8. **Instructor** (`.instructor-section#about`)
9. **TV Shows** (`.tv-section#tv-shows`) — carousel
10. **Bonuses** (`.bonus-section#bonuses`) — tabbed accordion
11. **Guarantee/Enroll** (`.guarantee-section#enroll`)
12. **FAQ** (`.faq-section#faq`) — accordion
13. **Final CTA** (`.final-cta`)

### Social Media Links (Homepage Only)
- **Instagram:** streetmagiclab
- **YouTube:** Sanad Diab channel
- **TikTok:** streetmagiclab

### Products Listed on Homepage

#### Main Course
- **Title:** Magic Tricks for Beginners: Card, Coin & Street Magic
- **URL:** `/b/4Wpkr`
- **Image:** `pe56d.s3.amazonaws.com/o_1jl7ocllcnq3omq1sq8t7a1msmc.png`

#### Mini Courses (Individual Tricks) — $4.99 each
1. **Do That Again Prediction** — `/b/qGQTw`
2. **Mind Reading / Thought-Of Card** — `/b/ojAPI`
3. **8 Card Brainwave** — `/b/nYCdg`
4. **Simple Yet Deceptive Card Trick** — `/b/lSXuW`
5. **The Three Dice Card Trick** — `/b/zuiOS`
6. **Three Card Monte** — `/b/5inzX`

#### Bundle
- **Complete Collection** (all 9 tricks, 50% off) — `/b/9-professional-self-working-card-tricks-anyone-can-do-bvu9`

---

## 6. MAIN SALES PAGE (/3-free-self-working-tricks)

This is the most sophisticated page on the site — a full sales funnel / landing page. Below is every section in order:

### 6.1 Hero Section
- **Subheading:** "Free Magic Masterclass"
- **Main Headline:** "Free Magic Masterclass By Sanad Diab"
- **CTA button:** "Free MasterClass"
- **Video:** Gumlet-hosted video player (24:38 duration)
  - Video ID: `697e02885ff8d4ab5d1e1188`
  - Collection: `697ced71bbfa4f281aefa3e6`
  - Thumbnail: `https://video.gumlet.io/.../thumbnail-1-0.png`

### 6.2 Value Proposition Section
- **Headline:** "Learn CARD MAGIC and get INSANE reactions tonight"
- **Subheadline:** "Street Magic Lab | Fool Real People With a Deck of Cards Starting Tonight"
- **Logo badge:** Street Magic Lab logo repeated

### 6.3 Anchor Navigation Bar
- Inline navigation with unicode icons (⌂★✦▶♠♣♦?◇)
- Links to page sections via anchor scrolling
- "Private Coaching" highlighted differently

### 6.4 Social Proof Bar
- "Seen on National TV" badge

### 6.5 Main Hero / CTA Section
- **Headline:** "Learn Card Magic in 30 Days and *Amaze Anyone*"
- **Subtext:** "Step-by-step training to help you perform powerful tricks with confidence even if you've never touched a deck before."
- **Three value bullets:**
  - ✦ **Command the Room:** Turn every social gathering into your stage.
  - ✦ **Zero-to-Hero Results:** Perform your first miracle by tonight.
  - ✦ **A Portable Superpower:** Be ready to amaze anyone, anytime.
- **Promo Video:** Vimeo embed (ID: 1179697740)
  - Caption: "Sanad shows you exactly what's inside the system"

### 6.6 Pricing CTA Block
- **CTA:** "Get Instant Access →"
- **Price display:** "Worth $160 / For Just: $47"
- **Social proof:** ★★★★★ **4.9/5** · 5,000+ verified students
- **Trust badges:**
  - ✓ 30-Day Guarantee
  - ◈ Lifetime access
- **Checkout URL:** `streetmagiclab.com/order?link=n8IWh&pricing_plan=YLBNYlpNzK`

### 6.7 Stats Bar
| Stat | Value |
|------|-------|
| Students Worldwide | 0+ (dynamic counter) |
| Years of Experience | 11 yrs |
| Seen on National TV | 5 Shows |
| Online Views | 6M+ |

### 6.8 Student Testimonials Section
- **Label:** "Student Testimonials"
- **Headline:** "Don't Take Our Word For It. *Take Theirs.*"
- **Subline:** "Real students sharing the moment they pulled off their first miracle."
- **Carousel:** Left/right arrows (← →)
- **Rating summary:** "4.9 ★★★★★ Rated 4.9 / 5 across 5,000+ students"

### 6.9 "What Is Card Craft?" Section
- **Label:** "Why This Works"
- **Headline:** "What Is *Card Craft?*"
- **Description:** "Card Craft is a premium step-by-step online magic course..."

#### Three Feature Blocks:
1. **Learn Fast / The Easiest Way to Learn**
   - "Every tutorial is concise, structured and filmed in 4K from multiple angles..."
   - Image: `pe56d.s3.amazonaws.com/o_1jnasn1ej1v6816c1d4917h11kjac.png`

2. **Impress Anyone / Learn How to Impress Anyone**
   - "The course gives you the ability to entertain anyone..."
   - Image: `pe56d.s3.amazonaws.com/o_1jnathv0cqkk1uar1181ctganrm.png`

3. **Master Performance / Master the Art of Performance**
   - "You don't just learn tricks. You learn how to perform them..."
   - Image: `pe56d.s3.amazonaws.com/o_1jnd8busm1fnc1fpe1rja111312f8l.png`

### 6.10 About Instructor Section
- **Image:** `pe56d.s3.amazonaws.com/o_1jd1ckhnmmsefff1dufkp81ap23o.jpg`
- **Label:** "Meet Your Instructor"
- **Name:** Sanad Diab
- **Subtitle:** "Professional Magician · 11+ Years · 5× National TV"
- **Bio:** Full multi-paragraph bio about his journey, TV appearances, credentials
- **Key stats mentioned:** 11 years experience, 5 TV appearances, 6 million online views

### 6.11 TV Appearances Section
- **Headline:** "5 Live National TV Performances. *Zero Edits.*"
- **Subline:** "This is the man teaching you. Watch the host's face every time..."

#### TV Shows Listed:
1. **Libya Panorama** — LibyaLive — "Live card change followed by a razor-blade act."
2. **218 TV Libya** — LibyaLive — "Signed card vanishes... reappears inside a sealed plastic water bottle."
3. **218 TV Libya** — LibyaLive — "Freely chosen, signed card found inside a whole intact lemon."
4. **218 TV Libya** — LibyaLive — "Selected card vanishes and materialises sealed inside an unopened cigarette pack."

- **Stats bar:** 5+ National TV Shows | All Live No Cuts | Millions Watching Live

### 6.12 Bonuses Section
- **Label:** "Included Free With Your Enrollment"
- **Headline:** "You Also Get Access To *2 Amazing Bonuses*"
- **VSL Video:** Vimeo embed (ID: 1186677822) — enhanced VSL

#### Bonus 1: 9 Self-Working Miracle Tricks
- "Zero sleight of hand. Zero practice required."
- Features: 9 complete tricks, mind-reading/predictions, perform same night, works with any deck

#### 7 Free Performance Videos (YouTube Embeds)
| # | Duration | Description | YouTube Thumbnail |
|---|----------|-------------|-------------------|
| 1 | 16 min | Mind-reading thought-of-card revelation | `DN37rG8T0vM` |
| 2 | 11 min | Predict outcomes twice in a row | `iUn2yT6zFrM` |
| 3 | 10 min | Dice, chaos & impossible odds | `vVqlxlaP-6A` |
| 4 | 9 min | Spectators sort red & black | `Hfyoa5cYSBc` |
| 5 | 7 min | Influence stranger with psychology | `y-YluOiteLM` |
| 6 | 12 min | Fast, unfair gambling routine | `2YADGp3TfT8` |
| 7 | 22 min | Two showstoppers | `b7-GZqcY32U` |

#### Bonus 2: Performance Scripts
- **Image:** `pe56d.s3.amazonaws.com/o_1jibgj9lj14t65tc14lsktv10g6c.jpg`
- "The exact word-for-word scripts Sanad uses for each trick."
- Features: Character/patter/reveal scripts, storytelling hooks, timing/pauses/crowd notes, tested on thousands

### 6.13 Pricing CTA (Repeated)
- "Total value: $160 Today just $47"
- CTA: "Get Full Access + All Bonuses →"

### 6.14 Full Course Curriculum Section
- **Label:** "Inside The Course"
- **Headline:** "Full Course *Curriculum*"
- **Stats:** 6 sections · 34 lectures · 1h 22m total · Free previews

#### Section 1: Sleight-of-Hand Foundations (6 lectures · 11min)
1. How to Hold Playing Cards – Part 1 (Mechanic's Grip) — ▶ Free Preview 2:02
2. How to Hold Playing Cards – Part 2 (Biddle Grip) — 1:13
3. How to Hand a Card to Someone Like a Pro — 1:32
4. What is the Pinky Break — 1:17
5. Controlling a Spectator's Card to the Top of the Deck — 2:06
6. Changing Any Card in a Spectator's Hands — 2:36

#### Section 2: Pro Card Shuffles (4 lectures · 8min)
1. The Swing Cut — ▶ Free Preview 1:21
2. The Hindu Shuffle — 1:22
3. Shuffling While Keeping the Order Intact — 1:24
4. Professional Riffle Shuffle — 3:53

#### Section 3: Mind Control & Advanced Manipulation (6 lectures · 15min)
1. Controlling a Spectator's Mind & Card – Part 1 — 2:59
2. Controlling a Spectator's Mind & Card – Part 2 — 3:00
3. Turning Any Random Card Into Their Chosen One — 2:25
4. The Snap Change — 2:57
5. Hiding Cards Effectively — 1:51
6. Revealing Cards With the Glide Technique — 1:53

#### Section 4: Showstopper Card Flourishes (2 lectures · 5min)
1. Make Cards Fly Like a Pro (The Spring) — 2:08
2. The Famous Fan Flourish — 3:03

#### Section 5: Powerful Tricks That Always Work (7 lectures · 25min)
1. The Four Thieves Trick — 3:47
2. The Self-Working Trick — 3:09
3. Coin Vanish: French Drop — 1:34
4. Sponge Balls Vanish — 2:33
5. Cups and Balls — 3:02
6. The Magic Rope Trick — 7:14
7. Dice Magic Trick — 3:34

#### Section 6: Practice & Performance Mastery (9 lectures · 19min)
1. Daily Practice for Real Skill Growth — 1:29
2. Always Record Your Practice — 1:19
3. Practicing in Front of a Mirror — 0:58
4. Hand Flexibility Warm-Ups — 1:54
5. Practicing on Friends & Family First — 0:58
6. Building Strong Audience Connection — 2:04
7. Presenting Tricks Like a Story — 2:47
8. Handling Live Mistakes Like a Pro — ▶ Free Preview 5:20
9. Finding New Tricks After This Course — 2:03

### 6.15 Guarantee Section
- **Label:** "Zero Risk to You"
- **Headline:** "The 30-Day Street Mastery *Guarantee*"
- **Icon:** 🔒
- **Sub-headline:** "30-Day Money-Back Promise"
- **Title:** "Perform a Trick. Or It's Free."
- **Body:** Full guarantee copy explaining the 30-day refund policy

### 6.16 Reviews Section
- **Label:** "5,000+ Student Reviews"
- **Headline:** "Real Results From *Real Beginners.*"
- **Subline:** "Unfiltered. Unedited. Real students who started exactly where you're sitting right now."

#### Reviews:
1. **Jake Morrison** (JM) — Austin, Texas — ★★★★★
   - "I'd burned weeks on YouTube tutorials and gotten nowhere..."
2. **Chloe Harrington** (CH) — Portland, Oregon — ★★★★☆
   - "Honestly wasn't sure what to expect for $47..."
3. **Tyler Weston** (TW) — Nashville, Tennessee — ★★★★☆
   - "The performance scripts are something I never knew I needed..."
4. **Brittany Owens** (BO) — Atlanta, Georgia — ★★★★★
   - "Day 7's 1-in-362,880 trick is unreal..."
5. **Marcus Delgado** (MD) — Miami, Florida — ★★★★☆
   - "Solid course. I did wish there were a few more lectures..."
6. **Sarah Kim** (SK) — Seattle, Washington — ★★★★★
   - "I knocked out the bonus in one afternoon..."

### 6.17 FAQ Section
- **Label:** "Real Answers"
- **Headline:** "Everything You're Wondering"

#### FAQ Items (Accordion):
1. **Do I need any natural talent or experience?** — No experience needed
2. **Why pay for this when YouTube has free magic?** — Structured system vs scattered videos
3. **What gear do I actually need?** — Standard deck of playing cards
4. **Exactly what's included for $47?** — 34 lessons + 9 bonus tricks + 9 scripts
5. **How fast can I actually perform for real people?** — Self-working tricks: tonight
6. **What if it just doesn't work for me?** — 30-day money-back guarantee
7. **Will this work outside the US? Will it work for shy people?** — Yes, 40+ countries
8. **Can I work with Sanad one-on-one?** — Yes, Private Coaching available

### 6.18 Final CTA Section
- **Label:** "One Question Left"
- **Headline:** "Stop Watching Magic. *Start Being Watched.*"
- **Body:** Emotional closing copy
- **Price:** "Total value: $160 / For Just: $47"
- **CTA:** "Get The Complete System →"
- **Trust badges:** 🔒 Secure checkout ▶ Instant access ◈ Lifetime access 🕐 30-Day Guarantee ★ 5,000+ students

### 6.19 Sticky Bottom Bar
```
Card Craft: Full System — 34 lessons + 9 bonus tricks
[Start Learning $47 →]
```

---

## 7. INTERACTIVE ELEMENTS & POPUPS

### 7.1 Exit-Intent Popup — Mystery Card Game (25% Discount)
- **Element:** `#mcOverlay` overlay with modal
- **Trigger:**
  - Desktop: `mouseleave` event when cursor exits viewport top (`e.clientY <= 0`)
  - Mobile: Fast upward scroll near top (currentY < 150, deltaY > 60, deltaTime < 300ms)
  - Repeat prevention: `localStorage.getItem('mc_shown')`
- **Headline:** "Wait: before you go, you've unlocked a Secret Discount"
- **Interactive element:** "Pick a card to reveal exactly how much you save" with 3 card options (♠ ♥ ♦)

#### 3D Card Flip Animation
```css
.mc-card { perspective: 600px; }
.mc-card-inner { transform-style: preserve-3d; transition: transform 0.6s; }
.mc-card.flipped .mc-card-inner { transform: rotateY(180deg); }
.mc-card-front, .mc-card-back { backface-visibility: hidden; }
.mc-card-back { transform: rotateY(180deg); }
```

- **Reveal:** All cards show 25% OFF
- **Note:** "Any card you pick reveals the same offer. Your choice is yours"
- **Discount code:** `STREET25`
- **Discounted price:** $35.25
- **Email capture form:** "Drop your details below and we'll send your code instantly"
- **CTA:** "Get My 25% Coupon Code →"
- **After submit:** Shows code and "Apply Code at Checkout →" link

### 7.2 Social Proof Notification Popup
- **Format:** Small notification card (bottom corner)
- **Content:** "[Name] just enrolled in Street Magic Lab"
- **Example:** "JM Jake Morrison · just enrolled · 2 minutes ago · Instant access granted"
- **Dismissible:** ✕ button

### 7.3 Private Coaching Modal (Multi-Step Form)

**Step 1 — Level Selection:**
- Headline: "Book a 1-on-1 With Sanad"
- Subtitle: "60 minutes. Fully personalised. Limited spots each month."
- Question: "First: what's your current level?"
- Options:
  - ♠ Complete beginner: never touched a card
  - ♣ I know a few basic tricks
  - ♥ Intermediate: perform occasionally
  - ♦ Advanced: want to level up further

**Step 2 — Contact Form:**
- Headline: "Almost There"
- Subtitle: "Sanad's team will reach out within 24 hours to confirm your session."
- Fields: Your Name, Email Address
- CTA: "Request My Session →"
- Back button: "← Go back"

**Step 3 — Confirmation:**
- Headline: "Request Received!"
- Message: "Sanad's team will be in touch within 24 hours. Watch your inbox."
- Playing card suit decorations: ♠ ♥ ♣ ♦

### 7.4 Cookie Consent Banner
- "By using this website, you agree to our use of cookies..."
- Buttons: Reject | Accept

### 7.5 Modals
- "Thank you!" — message sent confirmation
- "Could not add item to cart" — error modal
- "Write a Review" — redirects to download page

---

## 8. PRODUCT PAGE TEMPLATE (/b/{shortcode})

### Structure (from /b/qGQTw):
1. **Header** — Same site-wide header
2. **Hero Image** — Full-width product image
3. **Product Title** — Large heading with subtitle
4. **Effect Description** — "What Happens" section describing the trick
5. **YouTube Video Embed** — Performance video
6. **Price & Buy Button** — "$4.99" + "Buy Now" button
7. **What You'll Learn** — Bullet list of learning outcomes
8. **What's Included** — Bullet list of deliverables
9. **Cross-Sell Banner** — "Best value: Get all tricks in the Complete Collection and save 50%"
10. **Testimonials** — Screenshot-style comment testimonials
11. **FAQs** — Accordion-style Q&A
12. **Course Curriculum** — Lesson list with free preview links
13. **Footer** — Standard footer

### Product Pricing
- Individual mini courses: **$4.99** each
- Main course (Card Craft Full System): **$47** one-time
- Complete Collection (9 tricks bundle): **$24.99** (50% off individual)
- Value anchor: "Worth $160"
- Discount code: **STREET25** (25% off = $35.25)

---

## 9. COURSE PAGE TEMPLATE (/b/4Wpkr)

### Structure:
1. **Header** — Standard
2. **Demo Content Sections** — Image + text blocks (Payhip store builder defaults)
3. **Pricing Plans** — (this product shows "no pricing plans")
4. **Course Curriculum** — Expandable section list with lesson names
   - Free Preview links available on select lessons
   - 6 sections, 34 lessons total
5. **Footer** — Standard

---

## 10. BLOG SECTION (/blog/)

### Structure:
- **Category page:** `/blog/card-magic-guides`
- **Post format:** Card layout with placeholder image, author name, date, excerpt
- **Author:** Sanad Diab
- **Known posts:**
  - "Card Magic for Beginners: How to Actually Learn It" (October 04, 2026)
- **Default image:** `streetmagiclab.com/images/themes/_core/media-not-provided-dark.svg`

---

## 11. FOOTER (All Pages)

### Payment Methods Accepted
- Maestro
- Mastercard
- PayPal
- Visa
- Discover

### Payhip Branding
- "Powered by Payhip"
- Links: Privacy | GDPR | EU VAT | Sell Digital Downloads | Sell Memberships

### Custom Footer
- **Brand link:** "CardCraft" (links to current page)
- **Links:** Privacy Policy | Terms | Contact (mailto:contact@streetmagiclab.com)
- **Copyright:** © 2026 Card Craft — Sanad Diab. All rights reserved.

---

## 12. EXTERNAL SERVICES & INTEGRATIONS

### Core Platform
- **Payhip** — E-commerce platform, storefront builder, checkout, course hosting, blog, user accounts
  - Theme: `enigma`
  - Builder: `EditorV2`
  - Environment key: `O3BeAoPmB5`
  - CDN: `payhip.com/cdn-cgi/image/format=auto/...`
  - Asset storage: `pe56d.s3.amazonaws.com/...`
  - Custom domain: streetmagiclab.com
  - Seller dashboard: `payhip.com/BeginnerCardMagic`

### Video Hosting
| Service | Usage | IDs |
|---------|-------|-----|
| **Gumlet** | Free masterclass video (24:38) | Video: `697e02885ff8d4ab5d1e1188`, Collection: `697ced71bbfa4f281aefa3e6` |
| **Vimeo** | Promo/VSL videos (9 embeds on homepage) | `1179697740`, `1186677822`, `7zR0hJYmRLk`, `YxPEWPZ_xHE`, `z4M-3K0aS7I`, `2kblp-4VWnY`, `G2RFlXX-WCg`, `dg7Cz0TW49M` + others |
| **YouTube** | Free trick tutorials (10+ videos) | `DN37rG8T0vM`, `iUn2yT6zFrM`, `vVqlxlaP-6A`, `Hfyoa5cYSBc`, `y-YluOiteLM`, `2YADGp3TfT8`, `b7-GZqcY32U`, `xbJ9olMa5lw`, `znlXJZXVmVk`, `H5nszTP8NA8` |

### Analytics & Tracking
| Service | ID | Type |
|---------|-----|------|
| **Google Analytics 4** | `G-BT5GSR1E4G` | Site GA4 property |
| **Google Analytics 4** | `G-49K529ZBBV` | Payhip platform GA4 |
| **Universal Analytics** | `UA-34658431-1` | Legacy GA (Payhip) |
| **Facebook Pixel** | `370293969737866` | FB/Meta Ads tracking |
| **PostHog** | `phc_eUaGMMh9xTPUGkYkiGkC8l1sDwNp3N7PZJhxCRs9YY0` | Product analytics |

### Email & Forms
| Service | Usage | Details |
|---------|-------|---------|
| **ConvertKit** | Email capture (hero/footer/exit popup) | API Key: `19qfj5xRo0i-vDiJorDrtg`, Form ID: `9538639` |
| **Formspree** | Coaching intake form | Endpoint: `https://formspree.io/f/mjgppnwk` |

#### ConvertKit Integration
```javascript
CK_API_KEY = '19qfj5xRo0i-vDiJorDrtg';
CK_FORM_ID = '9538639';
// POST to: https://api.convertkit.com/v3/forms/9538639/subscribe
// Body: { api_key, email, first_name, fields: { last_name }, tags: ['selectcard'] }
```

### CDN & Infrastructure
- **Cloudflare** — Via Payhip's CDN (`payhip.com/cdn-cgi/`)
- **AWS S3** — Asset storage (`pe56d.s3.amazonaws.com`)
- **Gumlet CDN** — `video.gumlet.io`, `assets.gumlet.io`
- **Vimeo CDN** — `i.vimeocdn.com`
- **YouTube CDN** — `i.ytimg.com`

### Libraries Loaded (via Payhip)
- jQuery 3.4.1
- Bootstrap 4.4.1
- Popper.js 1.16.0
- SweetAlert v2.9
- Mustache.js (cart/search template rendering)
- js-cookie 3.0.1
- hCaptcha
- vanilla-lazyload 17.3.1
- interact.js 1.9.20
- Vimeo Player API
- SimpleLightbox
- Toastify v1.11
- Swiper (carousel)

---

## 13. ALL IMAGES CATALOG

### Brand & Header Images
| Image | URL (S3 Key) | Usage |
|-------|-------------|-------|
| Logo | `o_1jcubent1sl91kmo14ha7gh1coe13.png` | Site logo, instructor badge |
| Favicon | `o_1jmopmagv1dtg18vfr331o393cd12.png` | Browser tab icon |
| OG/Header Banner | `o_1k40h51m31te8qa516ue1m861tg1g.png` | Social share image, header banner |

### Sales Page Images
| Image | URL (S3 Key) | Usage |
|-------|-------------|-------|
| Sanad Diab Photo | `o_1jd1ckhnmmsefff1dufkp81ap23o.jpg` | About instructor section |
| Learn Card Magic | `o_1jnasn1ej1v6816c1d4917h11kjac.png` | "Learn Fast" feature block |
| Impress Anyone | `o_1jnathv0cqkk1uar1181ctganrm.png` | "Impress Anyone" feature block |
| Master Performance | `o_1jnd8busm1fnc1fpe1rja111312f8l.png` | "Master Performance" feature block |
| Performance Scripts Book | `o_1jibgj9lj14t65tc14lsktv10g6c.jpg` | Bonus 2 scripts book cover |

### Product Page Images
| Image | URL (S3 Key) | Usage |
|-------|-------------|-------|
| Course Product Image | `o_1jl7ocllcnq3omq1sq8t7a1msmc.png` | Main course card |
| Do That Again Hero | `o_1jd15tp8r5e21vd21hkpaj1bis17.png` | Product hero image |
| Do That Again OG | `o_1jdeamq7bbna6bsr5pv9i1c3fc.png` | Social share |
| What You'll Learn | `o_1jd16jgo8pdg3babivluf1sor22.png` | Inline graphic |

### Testimonial Screenshots (Product Pages)
- `o_1jdm3m4mo1obn1598fgi1vr8gl8h.png`
- `o_1jdm3m4moi9n1sau1sm918512mjg.png`
- `o_1jdm4fam2cia1urr1o76hm61u75p.jpeg`
- `o_1jdm4fam23pu1gues7c2aci8pn.jpeg`
- `o_1jdm4fam21mo6q5jlln4qh17sjo.jpeg`
- `o_1jdm41g3c1iog1ir1no71b9g139lc.png`

### YouTube Thumbnails (Free Performances)
| Video ID | Thumbnail URL |
|----------|--------------|
| `DN37rG8T0vM` | `https://i.ytimg.com/vi/DN37rG8T0vM/maxresdefault.jpg` |
| `iUn2yT6zFrM` | `https://i.ytimg.com/vi/iUn2yT6zFrM/maxresdefault.jpg` |
| `vVqlxlaP-6A` | `https://i.ytimg.com/vi/vVqlxlaP-6A/maxresdefault.jpg` |
| `Hfyoa5cYSBc` | `https://i.ytimg.com/vi/Hfyoa5cYSBc/maxresdefault.jpg` |
| `y-YluOiteLM` | `https://i.ytimg.com/vi/y-YluOiteLM/maxresdefault.jpg` |
| `2YADGp3TfT8` | `https://i.ytimg.com/vi/2YADGp3TfT8/maxresdefault.jpg` |
| `b7-GZqcY32U` | `https://i.ytimg.com/vi/b7-GZqcY32U/maxresdefault.jpg` |

### Lesson Preview Thumbnails (YouTube)
| Video ID | Lesson |
|----------|--------|
| `xbJ9olMa5lw` | Mechanic's Grip |
| `znlXJZXVmVk` | Swing Cut |
| `H5nszTP8NA8` | Handling Live Mistakes |

### Payhip Demo Images (Course Builder Defaults)
- `static-demo-media-content-section-camera-man-1-v2.jpg`
- `static-demo-media-content-section-camera-woman-1-v1.jpeg`

---

## 14. ALL LINKS CATALOG

### Internal Navigation
- `/` — Homepage
- `/3-free-self-working-tricks` — Main sales/landing page
- `/b/4Wpkr` — Beginners course
- `/b/n8IWh` — Card Craft Full System (main product)
- `/b/qGQTw` — Do That Again Prediction
- `/b/ojAPI` — Mind Reading
- `/b/nYCdg` — 8 Card Brainwave
- `/b/lSXuW` — Simple Yet Deceptive
- `/b/zuiOS` — Three Dice
- `/b/5inzX` — Three Card Monte
- `/b/9-professional-self-working-card-tricks-anyone-can-do-bvu9` — Complete Collection
- `/blog/card-magic-guides` — Blog
- `/blog/card-magic-guides/card-magic-for-beginners-how-to-actually-learn-it` — Blog post

### Checkout Links
- `/order?link=n8IWh&pricing_plan=YLBNYlpNzK` — Main course checkout ($47)
- `/order?link=qGQTw&pricing_plan=MrW6mNrAGN` — Individual trick checkout ($4.99)
- `/order?link=4Wpkr&free_preview_mode=1` — Free preview mode

### External Links
- `payhip.com/BeginnerCardMagic/users/login` — User login
- `payhip.com/builder/public?builderStartUrl=...` — Store builder
- `payhip.com/privacy` — Payhip privacy
- `payhip.com/gdpr` — GDPR info
- `payhip.com/eu-vat` — EU VAT info
- `payhip.com/features/sell-digital-downloads` — Payhip features
- `payhip.com/features/sell-memberships` — Payhip features
- `mailto:contact@streetmagiclab.com` — Contact email

### Video Links
- `vimeo.com/1179697740` — Promo video
- `vimeo.com/1186677822` — Enhanced VSL
- `youtube.com/watch?v=iUn2yT6zFrM` — Do That Again performance
- YouTube channel: `youtube.com/channel/UCHSV_5kbfvGwow8ZevXvF6w` (Sanad Diab)

---

## 15. PAYHIP-SPECIFIC IMPLEMENTATION DETAILS

### Platform Features Used
1. **Custom Domain** — streetmagiclab.com maps to Payhip storefront
2. **Store Builder** — Visual page builder for product/sales pages
3. **Course Hosting** — Video lessons with drip/section structure
4. **Product Types:** Courses (mini courses), digital downloads
5. **Pricing Plans** — Per-product pricing with plan IDs
6. **Free Preview** — Select lessons available without purchase
7. **Shopping Cart** — Built-in cart with item count badge
8. **User Accounts** — Login/registration for course access
9. **Custom Pages** — Landing pages like `/3-free-self-working-tricks`
10. **Blog** — Built-in blog with categories
11. **Cookie Consent** — GDPR-compliant cookie banner
12. **Review System** — Post-purchase review functionality
13. **Coupon Codes** — Discount system (STREET25 = 25% off)
14. **Payment Processing** — Maestro, Mastercard, PayPal, Visa, Discover

### Payhip Product IDs
| Product | Payhip Code | Pricing Plan |
|---------|------------|--------------|
| Card Craft Full System | `n8IWh` | `YLBNYlpNzK` |
| Do That Again Prediction | `qGQTw` | `MrW6mNrAGN` |
| Beginners Course | `4Wpkr` | — |

### Asset CDN Pattern
```
https://payhip.com/cdn-cgi/image/format=auto,width={width}/https://pe56d.s3.amazonaws.com/{s3_key}
```

### Payhip Platform Config (JavaScript)
```javascript
window.payhipShop = {
  global: { /* 19 keys, 105 constants */ },
  editor: { globalSettings: { /* color, cookie, font settings */ } },
  lang: { /* 1785 localization strings */ }
};
```

### Payhip CSS (18 style blocks total)
1. **Block 1** (22,850 chars): Payhip header CSS
2. **Block 5** (194,241 chars): Payhip enigma theme generated CSS
3. **Block 6** (2,773 chars): Custom menu/cart/nav overrides
4. **Block 8** (864 chars): Custom sticky header bar styles
5. **Block 10** (64,160 chars): **MAIN custom CSS** — 516 rules covering all custom sections (most important for replication)

### Replication Notes (Payhip-Specific)
1. **Without Payhip:** Replace checkout system, cart, search, header, and theme CSS
2. **Custom CSS override strategy:** The site hides Payhip's default header with MutationObserver and overrides Payhip's blue (#3b82f6) with orange (#E8651A) via JavaScript — a standalone replica would not need these hacks
3. **The 64,160-char main CSS block** (style block 10) contains all 516 custom rules needed for the visual design — this is the most critical block to extract
4. **No CSS Grid used anywhere** — everything is Flexbox-based
5. **Bootstrap 4.4.1 is loaded by Payhip** but custom sections don't use Bootstrap classes

---

## 16. SALES FUNNEL STRATEGY ANALYSIS

### Funnel Structure
1. **Traffic Source:** Facebook ads (indicated by `fbclid` parameter in URL), organic search, YouTube
2. **Landing Page:** `/3-free-self-working-tricks` — Free masterclass video hooks visitor
3. **Value Delivery:** 7 free performance videos on the sales page itself
4. **Social Proof:** 5,000+ students, 4.9/5 rating, TV appearances, testimonials
5. **Price Anchor:** "Worth $160 / For Just: $47"
6. **Guarantee:** 30-day money-back
7. **Exit Intent:** 25% discount popup (STREET25 → $35.25)
8. **Upsell Path:** Individual tricks at $4.99 → Complete Collection at $24.99 → Full System at $47
9. **High-Ticket:** Private 1-on-1 coaching with Sanad

### Persuasion Elements
- **Authority:** 5 national TV appearances, 11 years experience
- **Social proof:** Student count, ratings, testimonials with names/locations
- **Scarcity/Urgency:** "Limited spots each month" (coaching)
- **Risk reversal:** 30-day guarantee
- **Reciprocity:** Free masterclass video, 7 free performances
- **FOMO:** Social proof notification popup ("just enrolled")
- **Anchoring:** $160 value → $47 price

### CTA Variations Used
- "Get The System · $47 →"
- "Get Instant Access →"
- "Get Full Access + All Bonuses →"
- "Unlock All 34 Lessons + Bonuses →"
- "Get The Complete System →"
- "Start Learning $47 →"
- "Buy Now"
- "Get 50% OFF"
- "Free MasterClass"

---

## 17. HTML COMPONENT PATTERNS

### 17.1 Section Header (reused across ALL sections)
```html
<span class="eyebrow"><span class="eyebrow-dot"></span>LABEL TEXT</span>
<span class="divider"></span>
<h2 class="h2">Main Title <em>Italic Emphasis</em></h2>
<p class="sub">Descriptive subtitle paragraph</p>
```
```css
.eyebrow { font-size: 0.72rem; font-weight: 700; text-transform: uppercase; letter-spacing: 0.1em; }
.eyebrow-dot { width: 6px; height: 6px; border-radius: 50%; background: var(--orange); display: inline-block; margin-right: 0.5rem; }
.divider { background: linear-gradient(90deg, var(--orange), var(--gold)); height: 3px; width: 48px; border-radius: 2px; }
```

### 17.2 Trust Chip
```html
<span class="trust-chip trust-chip-green">30-Day Guarantee</span>
<span class="trust-chip">Lifetime access</span>
```

### 17.3 YouTube Facade (Lazy Load)
```html
<div class="yt-facade" data-id="VIDEO_ID" onclick="loadYT(this)">
  <img src="https://i.ytimg.com/vi/VIDEO_ID/maxresdefault.jpg" alt="..." loading="lazy">
  <div class="yt-play"><!-- SVG play button --></div>
</div>
```

### 17.4 Carousel
```html
<div class="carousel-viewport">
  <div class="carousel-track" id="NAME-track">
    <div class="carousel-card"><!-- card content --></div>
  </div>
</div>
<div class="carousel-nav">
  <button onclick="moveCarousel('NAME',-1)"><!-- left arrow --></button>
  <div class="carousel-dots">
    <span class="carousel-dot active" onclick="goToSlide('NAME',0)"></span>
  </div>
  <button onclick="moveCarousel('NAME',1)"><!-- right arrow --></button>
</div>
```

### 17.5 FAQ Accordion Item
```html
<div class="faq-item">
  <button class="faq-q" onclick="toggleFaq(this)">
    <span>Question text here?</span>
    <span class="faq-icon"><!-- plus/minus SVG --></span>
  </button>
  <div class="faq-a"><p>Answer text here.</p></div>
</div>
```
```css
.faq-a { max-height: 0; overflow: hidden; transition: max-height 0.35s ease; }
.faq-item.open .faq-a { max-height: 600px; }
```

### 17.6 Stat Item
```html
<div class="stat-item">
  <div class="stat-num">4.9/5</div>
  <div class="stat-lbl">Student Rating</div>
</div>
```

### 17.7 Testimonial Card
```html
<div class="testi-card">
  <div class="testi-stars"><!-- 5 star SVGs --></div>
  <p class="testi-text">"Review quote text..."</p>
  <div class="testi-author">
    <div class="testi-avatar"><!-- initials or image --></div>
    <div>
      <div class="testi-name">Name</div>
      <div class="testi-role">Verified Student</div>
    </div>
  </div>
</div>
```

### 17.8 Curriculum Module Accordion
```html
<div class="curr-module">
  <button class="curr-toggle" onclick="toggleSection('module-N')">
    <span class="curr-module-title">Module N: Title</span>
    <span class="curr-meta">X lectures - XX min</span>
    <span class="curr-chevron"><!-- chevron SVG --></span>
  </button>
  <div class="curr-lectures" id="module-N">
    <div class="curr-lecture" onclick="togglePreview('preview-N-M', event)">
      <span class="curr-lecture-icon"><!-- play/lock icon --></span>
      <span class="curr-lecture-title">Lecture Title</span>
      <span class="curr-lecture-dur">5:23</span>
    </div>
  </div>
</div>
```

### 17.9 Modal Overlay
```html
<div class="cm-overlay" id="coachingOverlay" onclick="if(event.target===this)closeCoachingModal()">
  <div class="cm-modal">
    <button class="cm-close" onclick="closeCoachingModal()">&times;</button>
    <!-- modal content -->
  </div>
</div>
```
```css
.cm-overlay {
  position: fixed; inset: 0; z-index: 9999;
  background: rgba(0,0,0,0.6); backdrop-filter: blur(4px);
  display: none;
}
.cm-overlay.open { display: flex; align-items: center; justify-content: center; }
.cm-modal {
  background: #fff; border-radius: 16px; max-width: 520px; width: 90%;
  box-shadow: var(--sh-lg); animation: modalUp 0.4s ease;
}
```

### 17.10 Sticky Mobile Bar
```html
<div class="sticky-bar" id="stickyBar">
  <a href="...order..." class="btn btn-orange" style="width:100%;justify-content:center">Start Learning Magic Now</a>
  <p>$47 one-time - Lifetime access</p>
</div>
```

### 17.11 Footer
```html
<footer class="cc-footer">
  <div class="cc-foot-inner">
    <a class="cc-foot-logo">Card<span>Craft</span></a>
    <div class="cc-foot-links">
      <a>Privacy Policy</a><a>Terms</a><a href="mailto:contact@streetmagiclab.com">Contact</a>
    </div>
    <p class="cc-foot-copy">&copy; 2026 Card Craft - Sanad Diab. All rights reserved.</p>
  </div>
</footer>
```

---

## 18. CSS CLASS NAMING CONVENTIONS

### Prefix System
| Prefix | Section | Examples |
|--------|---------|----------|
| `hero-` | Hero section | `hero-inner`, `hero-left`, `hero-right`, `hero-eyebrow`, `hero-sub`, `hero-rating`, `hero-video-wrap`, `hero-trust-row` |
| `nav-` | Navigation | `nav-link`, `nav-overlay` |
| `stat-` | Stats bar | `stat-item`, `stat-num`, `stat-lbl` |
| `testi-` | Testimonials | `testi-section`, `testi-card`, `testi-name`, `testi-role` |
| `why-` | Why section | `why-section`, `why-card`, `why-icon` |
| `inst-` | Instructor | `inst-card`, `inst-img`, `inst-info` |
| `tv-` | TV shows | `tv-section`, `tv-card`, `tv-overlay` |
| `bonus-` / `bonus1-` / `bonus2-` | Bonus sections | |
| `curr-` | Curriculum | `curr-module`, `curr-lecture`, `curr-toggle` |
| `guarantee-` | Guarantee | |
| `rev-` / `review-` | Reviews | |
| `faq-` | FAQ | `faq-item`, `faq-q`, `faq-a` |
| `final-` | Final CTA | |
| `sticky-` | Sticky bar | |
| `cc-foot-` | Footer | `cc-footer`, `cc-foot-inner`, `cc-foot-logo`, `cc-foot-links`, `cc-foot-copy` |
| `cm-` | Coaching modal | |
| `mc-` | Mystery card popup | |
| `cp-` | Course preview modal | |
| `yt-` | YouTube facade | |
| `popup-` | Popup styles | |
| `sml-` | Street Magic Lab branded | |
| `btn-` | Buttons | `btn-orange`, `btn-hero-main`, `btn-outline` |
| `wyl-` | What You'll Learn | |
| `carousel-` | Carousel | |

### State Modifier Classes
- `.open` — Accordion/modal open state
- `.active` — Active nav link / tab
- `.visible` — Scroll-revealed element
- `.scrolled` — Header after scroll
- `.selected` — Selected card/option
- `.dimmed` — Non-selected cards dimmed
- `.flipped` — 3D card flipped
- `.picked` — Mystery card picked
- `.done` — Completed step
- `.copied` — Copy button success state

### Utility Classes
- `.wrap`, `.wrap-sm`, `.wrap-xs` — Container widths
- `.reveal` — Scroll reveal target
- `.desktop-only-bullets` — Desktop visibility
- `.trust-chip` — Trust badge pill
- `.eyebrow` — Section label
- `.divider` — Orange gradient line
- `.sub` — Subtitle paragraph

---

## 19. JAVASCRIPT PATTERNS

### 19.1 YouTube Facade Lazy Loading
```javascript
function loadYT(el) {
  var id = el.getAttribute('data-id');
  var iframe = document.createElement('iframe');
  iframe.src = 'https://www.youtube.com/embed/' + id + '?autoplay=1&rel=0';
  iframe.allow = 'autoplay;encrypted-media';
  iframe.allowFullscreen = true;
  el.innerHTML = '';
  el.appendChild(iframe);
  el.classList.add('playing');
}
```

### 19.2 CSS-Based Carousel
```javascript
function updateCarousel(name) {
  var track = document.getElementById(name + '-track');
  track.style.transform = 'translateX(-' + (state.idx * (cardW + gap)) + 'px)';
  // CSS: transition: transform 0.4s cubic-bezier(.4,0,.2,1)
}
function moveCarousel(name, dir) { /* increment/decrement index, clamp, updateCarousel */ }
function goToSlide(name, idx) { /* jump to specific slide */ }
```

### 19.3 Scroll-Reveal Animation
```javascript
var revealObserver = new IntersectionObserver(function(entries) {
  entries.forEach(function(entry) {
    if (entry.isIntersecting) {
      entry.target.classList.add('visible');
      revealObserver.unobserve(entry.target);
    }
  });
}, { threshold: 0.08 });
document.querySelectorAll('.reveal').forEach(function(el) {
  revealObserver.observe(el);
});
```
```css
.reveal { opacity: 0; transform: translateY(24px); transition: opacity 0.7s, transform 0.7s; }
.reveal.visible { opacity: 1; transform: translateY(0); }
```

### 19.4 FAQ Accordion (One-at-a-Time)
```javascript
function toggleFaq(btn) {
  var item = btn.parentElement;
  var isOpen = item.classList.contains('open');
  document.querySelectorAll('.faq-item.open').forEach(function(el) { el.classList.remove('open'); });
  if (!isOpen) item.classList.add('open');
}
```

### 19.5 Scroll-Tracking Side Nav
```javascript
window.addEventListener('scroll', function() {
  var sections = ['top','curriculum','proof','about','tv-shows','bonuses','enroll','faq'];
  sections.forEach(function(id) {
    var el = document.getElementById(id);
    if (el) {
      var rect = el.getBoundingClientRect();
      if (rect.top <= 200 && rect.bottom > 200) {
        document.querySelectorAll('.nav-link').forEach(function(l) { l.classList.remove('active'); });
        document.querySelector('.nav-link[data-section="' + id + '"]').classList.add('active');
      }
    }
  });
});
```

### 19.6 Dynamic Payhip Color Override
```javascript
document.querySelectorAll('*').forEach(function(el) {
  var cs = getComputedStyle(el);
  if (cs.backgroundColor === 'rgb(59, 130, 246)') { // #3b82f6 Payhip blue
    el.style.backgroundColor = 'var(--orange)';
  }
});
```

### 19.7 Multi-Step Coaching Modal
```javascript
function openCoachingModal() { /* show overlay, reset to step 1 */ }
function cmNext() { /* validate current step, advance to next */ }
function cmBack() { /* go to previous step */ }
function cmSubmit() {
  // POST to: https://formspree.io/f/mjgppnwk
  // Collects: name, email, experience, goals, preferred_time
}
```

### 19.8 Keyframe Animations (8 total)
| Name | Purpose |
|------|---------|
| `pulse` | CTA button pulsing scale |
| `pulseTag` | Tag badge pulsing |
| `popupBlink` | Popup attention blink |
| `fadeIn` | Generic fade in |
| `modalUp` | Modal slide up from bottom |
| `mcPhaseIn` | Mystery card phase in |
| `mcOverlayIn` | Mystery card overlay fade |
| `mcModalIn` | Mystery card modal entrance |
| `spin` | Loading spinner rotation |

---

## 20. DOM STRUCTURE MAP

### Major DOM Sections (in order)
```
<body>
  ├── header.header-section-wrapper (Payhip default — hidden via MutationObserver)
  ├── nav.navbar (Payhip default — hidden)
  ├── .sml-header-bar (custom sticky header, fixed, z-500, h:70px)
  ├── #navToggle (fixed nav toggle button, z-501)
  ├── #navPanel (fixed left sidebar, w:230px, slides from left)
  ├── .hero#top > .hero-inner (flex row: 48%/flex-1 split)
  │   ├── .hero-left (text + CTA)
  │   └── .hero-right (video facade + CTA)
  ├── .wyl-section (What You'll Learn)
  ├── Stats bar (inline-styled dark bar, 4 stat items)
  ├── Reviews bar (inline-styled, star ratings)
  ├── .curriculum-section#curriculum (accordion)
  ├── .testi-section#proof (testimonial carousel)
  ├── .why-section (Why This Course)
  ├── .instructor-section#about
  ├── .tv-section#tv-shows (TV carousel)
  ├── .bonus-section#bonuses (tabbed accordion)
  ├── .guarantee-section#enroll
  ├── .faq-section#faq (accordion)
  ├── .final-cta
  ├── .sticky-bar#stickyBar (mobile only, fixed bottom)
  ├── footer.cc-footer
  └── Modals:
      ├── #coachingOverlay (coaching modal)
      ├── #mcOverlay (mystery card / exit-intent)
      └── #cpOverlay (course preview)
```

### DOM Stats
- 808 `<div>` elements
- 260 `<span>` elements
- 75 SVG elements
- 65 buttons
- 12 `<section>` elements

---

## 21. REPLICATION CHECKLIST

To replicate this site, you need:

### Platform Setup
- [ ] Payhip account (or equivalent e-commerce platform)
- [ ] Custom domain configuration
- [ ] SSL certificate (handled by Payhip)

### Content Required
- [ ] Logo (PNG, transparent background)
- [ ] Favicon
- [ ] OG/social share image (1500px wide)
- [ ] Instructor professional photo
- [ ] Product/course images
- [ ] 34 video lessons (hosted on Payhip course system)
- [ ] Promo video (hosted on Vimeo/Gumlet)
- [ ] 7 free performance videos (YouTube)
- [ ] Written testimonials (6 reviews with names, locations, ratings)
- [ ] TV appearance descriptions
- [ ] Performance scripts (bonus content)
- [ ] Blog content
- [ ] FAQ content (8 questions with answers)
- [ ] Guarantee copy
- [ ] About instructor bio

### Design Implementation
- [ ] CSS custom properties (`:root` variables — see Section 2)
- [ ] Dark theme (background `#0d0d12` / `#111118` / `#1a1a24`)
- [ ] DM Serif Display for headings (Google Fonts — weights 400, italic)
- [ ] DM Sans for body text (Google Fonts — weights 300–700, italic 400)
- [ ] Primary accent color `#E8651A` (orange) with `#C4500E` hover
- [ ] Gold accent `#C9A84C` / `#F0DC8A` for premium elements
- [ ] Pure Flexbox layout (no CSS Grid)
- [ ] Container widths: 1100px / 760px / 600px
- [ ] Responsive breakpoints (768px primary, 7 total)
- [ ] 16px base font size with `clamp()` responsive headings
- [ ] 10px border-radius on CTA buttons
- [ ] Orange glow shadow on CTA buttons (`0 4px 15px rgba(232,101,26,0.35)`)
- [ ] Full-width dark section bleed technique (`100vw` + negative margins)
- [ ] 8 gradient definitions (see Section 2)
- [ ] Scroll-reveal animations (IntersectionObserver + `.reveal`/`.visible` classes)

### Interactive Features
- [ ] Exit-intent popup with 3D card-flip animation (CSS perspective/rotateY)
- [ ] Social proof notification popup (fake enrollment alerts)
- [ ] Multi-step coaching inquiry form/modal (3 steps, Formspree endpoint)
- [ ] Accordion FAQ section (one-at-a-time, max-height transition)
- [ ] Testimonial carousel with arrows (CSS translateX + cubic-bezier)
- [ ] TV shows carousel
- [ ] Sticky bottom CTA bar (mobile only, fixed bottom)
- [ ] Side navigation panel with scroll-tracking active state
- [ ] Custom sticky header (hides Payhip default via MutationObserver)
- [ ] YouTube lazy-load facades (click-to-load iframe pattern)
- [ ] Cookie consent banner
- [ ] Video players (Gumlet, Vimeo, YouTube embeds)
- [ ] Course preview modal (`#cpOverlay`)
- [ ] Payhip blue-to-orange color override (JavaScript)
- [ ] 9 keyframe animations (pulse, fadeIn, modalUp, etc.)

### Email & Analytics
- [ ] ConvertKit email capture integration (API key + form ID)
- [ ] Formspree form submission (coaching modal)
- [ ] Google Analytics 4 (`G-BT5GSR1E4G`)
- [ ] Facebook Pixel (`370293969737866`)
- [ ] PostHog product analytics

### E-Commerce Features
- [ ] Shopping cart with badge counter
- [ ] Multiple product listings
- [ ] Course curriculum with expandable sections
- [ ] Free preview functionality
- [ ] Coupon code system (`STREET25` = 25%, `MAGIC` = 20%)
- [ ] Multiple payment methods (Visa, Mastercard, PayPal, Discover, Maestro)
- [ ] User login/registration
- [ ] Order confirmation flow

### SEO & Social
- [ ] Open Graph meta tags
- [ ] Twitter Card meta tags
- [ ] Favicon
- [ ] Page titles and descriptions
- [ ] Blog with categories
- [ ] `noindex,indexifembedded` robots directive (Payhip default)
- [ ] Social media links (Instagram, YouTube, TikTok)

---

*Analysis completed: October 12, 2026*
*Source: streetmagiclab.com (Powered by Payhip)*
