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

### Color Palette

| Role | Hex | Usage |
|------|-----|-------|
| **Primary / Accent** | `#E8651A` | CTA buttons, highlights, accents (orange) |
| **Secondary** | `#007BFF` | Links, secondary actions (blue) |
| **Background (dark)** | `#111111` | Main page background |
| **Text Primary** | `#111111` | Body text on light sections |
| **Link Color** | `#FEF0E6` | Link text on dark backgrounds (cream) |
| **Button Text** | `#FFFFFF` | White text on primary buttons |
| **Secondary Button BG** | `#E5E5E5` | Light gray button backgrounds |
| **Secondary Button Text** | `#333333` | Dark text on secondary buttons |

**Color Scheme:** Dark theme overall

### Typography

| Role | Font Family | Stack | Size |
|------|-------------|-------|------|
| **Headings** | DM Serif Display | `DM Serif Display, Georgia, serif` | H1: 52.8px, H2: 25.6px |
| **Body** | DM Sans | `DM Sans, system-ui, sans-serif` | 14px |
| **Additional** | Proxima Nova | (used in specific contexts) | varies |

**Font Source:** Google Fonts (DM Sans, DM Serif Display)

### Component Design Tokens

#### Primary Button
```css
background: #E8651A;
color: #FFFFFF;
border-radius: 14px;
box-shadow: rgba(232, 101, 26, 0.38) 0px 8px 32px 0px;
```

#### Secondary Button
```css
background: #E5E5E5;
color: #333333;
border-radius: 0px;
box-shadow: rgba(0, 0, 0, 0.35) 0px 6px 28px 0px;
```

#### General Spacing
- Base unit: 4px
- Border radius: 6px (general), 14px (buttons)

### Framework
- **CSS Framework:** Bootstrap
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

### Structure (Consistent Across All Pages)
- **Logo:** Street Magic Lab logo (top-left), links to homepage
- **Banner Image:** Full-width header image (the OG image, 1500px wide)
- **Search bar:** "View all results" search functionality
- **Cart icon:** Shopping cart with item count (badge showing "0")
- **Login link:** Links to `payhip.com/BeginnerCardMagic/users/login`
- **Mobile menu:** Hamburger menu on mobile

### Sales Page Navigation (Anchor Links on /3-free-self-working-tricks)
```
Navigation
⌂ Home
★ Student Reactions
✦ About Sanad
▶ TV Appearances
♠ Bonuses
♣ Full Curriculum
♦ Get Access
? FAQ
◇ Private Coaching
```

---

## 5. HOMEPAGE CONTENT (streetmagiclab.com/)

The homepage serves as the main storefront displaying all available products.

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

### 7.1 Exit-Intent Popup (25% Discount)
- **Trigger:** Mouse leaves viewport (exit intent)
- **Headline:** "Wait: before you go, you've unlocked a Secret Discount"
- **Interactive element:** "Pick a card to reveal exactly how much you save" with 3 card options (♠ ♥ ♦)
- **Reveal:** All cards show 25% OFF
- **Note:** "✦ Any card you pick reveals the same offer. Your choice is yours"
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
  - CDN: `payhip.com/cdn-cgi/image/format=auto/...`
  - Asset storage: `pe56d.s3.amazonaws.com/...`
  - Custom domain: streetmagiclab.com
  - Seller dashboard: `payhip.com/BeginnerCardMagic`

### Video Hosting
| Service | Usage | IDs |
|---------|-------|-----|
| **Gumlet** | Free masterclass video (24:38) | Video: `697e02885ff8d4ab5d1e1188`, Collection: `697ced71bbfa4f281aefa3e6` |
| **Vimeo** | Promo/VSL videos | `1179697740` (promo), `1186677822` (enhanced VSL) |
| **YouTube** | Free trick tutorials (7 videos) | `DN37rG8T0vM`, `iUn2yT6zFrM`, `vVqlxlaP-6A`, `Hfyoa5cYSBc`, `y-YluOiteLM`, `2YADGp3TfT8`, `b7-GZqcY32U` |

### CDN & Infrastructure
- **Cloudflare** — Via Payhip's CDN (`payhip.com/cdn-cgi/`)
- **AWS S3** — Asset storage (`pe56d.s3.amazonaws.com`)
- **Gumlet CDN** — `video.gumlet.io`, `assets.gumlet.io`
- **Vimeo CDN** — `i.vimeocdn.com`
- **YouTube CDN** — `i.ytimg.com`

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

## 17. REPLICATION CHECKLIST

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
- [ ] Dark theme (background #111111)
- [ ] DM Serif Display for headings (Google Fonts)
- [ ] DM Sans for body text (Google Fonts)
- [ ] Primary accent color #E8651A (orange)
- [ ] Bootstrap framework
- [ ] Responsive layout (mobile-first)
- [ ] 14px base font size
- [ ] 14px border-radius on CTA buttons
- [ ] Orange glow shadow on CTA buttons

### Interactive Features
- [ ] Exit-intent popup with card-picking animation
- [ ] Social proof notification popup (fake enrollment alerts)
- [ ] Multi-step coaching inquiry form/modal
- [ ] Accordion FAQ section
- [ ] Testimonial carousel with arrows
- [ ] Sticky bottom CTA bar
- [ ] Anchor navigation (smooth scroll)
- [ ] Cookie consent banner
- [ ] Video players (Gumlet, Vimeo, YouTube embeds)

### E-Commerce Features
- [ ] Shopping cart with badge counter
- [ ] Multiple product listings
- [ ] Course curriculum with expandable sections
- [ ] Free preview functionality
- [ ] Coupon code system
- [ ] Multiple payment methods
- [ ] User login/registration
- [ ] Order confirmation flow

### SEO & Social
- [ ] Open Graph meta tags
- [ ] Twitter Card meta tags
- [ ] Favicon
- [ ] Page titles and descriptions
- [ ] Blog with categories
- [ ] `noindex,indexifembedded` robots directive (Payhip default)

---

*Analysis completed: October 12, 2026*
*Source: streetmagiclab.com (Powered by Payhip)*
