# Content Calendar Template — Complete Structural Analysis

> **Source:** Google Sheets (.xlsx uploaded to Google Drive)
> **Title:** "Content Calendar - Posts"
> **Sheet count:** 1 (single sheet)
> **Purpose:** Multi-platform content scheduling template — blank framework ready to be filled with a content plan for any niche/business

---

## 1. SHEET ARCHITECTURE

### Dimensions
- **Columns:** 13 (A through M)
- **Rows:** 42 total (1 header row + 41 data rows)
- **Date range:** 6 weeks — Tuesday May 26 through Sunday July 5
- **Coverage:** Every calendar day (no weekend gaps, no rest days — continuous 7-day scheduling)

### Visual Formatting
| Element | Style |
|---------|-------|
| Header row | Bold text, gray background (`#aaaaaa`), border |
| Even data rows | White background (`#ffffff`) |
| Odd data rows | Light gray background (`#f0f0f0`) — zebra striping |
| Cell padding | 2px |
| Cell spacing | 0 |
| Borders | 1px solid (standard grid) |

---

## 2. COLUMN STRUCTURE (13 Columns)

The columns fall into 4 functional categories:

### Category 1: TIME AXIS (Columns A–B)

| Col | Header | Format | Example | Purpose |
|-----|--------|--------|---------|---------|
| A | **Date** | `Ddd D Mon` | `Tue 26 May` | Calendar date — abbreviated day name + date + abbreviated month |
| B | **Day** | Full day name | `Tuesday` | Redundant day-of-week for easy scanning/filtering |

**Design note:** The Day column duplicates information from Date. This is intentional — it lets you visually scan for "all Tuesdays" or filter by day name without parsing the date string. In a replicable system, this should be auto-generated from the date.

### Category 2: CONTENT CYCLE TRACKING (Columns C–D)

| Col | Header | Purpose |
|-----|--------|---------|
| C | **WB Cycle** | Website/Blog content cycle indicator |
| D | **YT Cycle** | YouTube content cycle indicator |

**What "Cycle" means:** These columns track which phase of a recurring content rotation applies on each day. For example:
- A blog might follow a 4-week cycle: Week 1 = Pillar Post, Week 2 = How-To, Week 3 = Listicle, Week 4 = Case Study
- YouTube might rotate: Week 1 = Tutorial, Week 2 = Vlog, Week 3 = Review, Week 4 = Collab

Cycle columns are **meta-planning columns** — they don't specify individual posts but mark the rhythm/pattern the content should follow. They're separate from the actual content cells.

### Category 3: PLATFORM CONTENT CELLS (Columns E–L)

These are the core scheduling cells — each one represents what gets published on a specific platform on a specific day.

| Col | Header | Platform | Content Type | Format |
|-----|--------|----------|-------------|--------|
| E | **YT Long-Form** | YouTube | Long-form video (10+ min) | Video title / topic |
| F | **YT Short-Form** | YouTube | Shorts (< 60 sec) | Short title / hook |
| G | **IG Reels New Page** | Instagram (new account) | Reels (short video) | Reel concept / hook |
| H | **IG Reels Old Page** | Instagram (legacy account) | Reels (short video) | Reel concept / hook |
| I | **IG Carousel** | Instagram | Carousel posts (multi-image) | Carousel topic / slide count |
| J | **FB Page / Groups** | Facebook | Page posts + Group shares | Post topic / type |
| K | **WhatsApp** | WhatsApp | Status / Broadcast / Group | Message topic |
| L | **Reddit** | Reddit | Subreddit posts / comments | Post title / subreddit |

**Platform architecture patterns:**

1. **YouTube is split by format** (Long-Form vs Short-Form) — not by account. This recognizes that these are fundamentally different content production workflows with different cadences.

2. **Instagram is split by account AND format:**
   - "New Page" vs "Old Page" = managing two IG accounts (common when rebranding or building a new presence while maintaining an existing one)
   - Reels (video) vs Carousel (image) = different content types tracked separately because they have different production workflows

3. **Facebook combines Page + Groups** in one column — these are treated as the same workflow (post once, share to groups).

4. **WhatsApp and Reddit** are included as distribution/community channels — recognizing modern content strategy extends beyond traditional social platforms.

### Category 4: METADATA (Column M)

| Col | Header | Purpose |
|-----|--------|---------|
| M | **Notes** | Free-text notes — campaign launches, holidays, content themes, reminders, deadlines, collabs |

---

## 3. DATE SYSTEM ANALYSIS

### Date Format: `Ddd D Mon`
- **Ddd** = 3-letter abbreviated day (`Mon`, `Tue`, `Wed`, `Thu`, `Fri`, `Sat`, `Sun`)
- **D** = Day of month (no leading zero: `1`, `2`, ... `31`)
- **Mon** = 3-letter abbreviated month (`May`, `Jun`, `Jul`)

### Calendar Span
- **Start:** Tuesday, May 26 (starts mid-week, not on a Monday)
- **End:** Sunday, July 5
- **Total days:** 41
- **Total weeks:** ~5.86 (approximately 6 full weeks)
- **Week boundaries:** The calendar does NOT align to Monday-start weeks — it's a continuous daily list

### Week Breakdown
| Week | Dates | Days |
|------|-------|------|
| Partial Week 1 | May 26 (Tue) – May 31 (Sun) | 6 days |
| Week 2 | Jun 1 (Mon) – Jun 7 (Sun) | 7 days |
| Week 3 | Jun 8 (Mon) – Jun 14 (Sun) | 7 days |
| Week 4 | Jun 15 (Mon) – Jun 21 (Sun) | 7 days |
| Week 5 | Jun 22 (Mon) – Jun 28 (Sun) | 7 days |
| Week 6 | Jun 29 (Mon) – Jul 5 (Sun) | 7 days |

**Design insight:** The 6-week span is a sweet spot for content planning — long enough for a full campaign cycle, short enough to remain actionable. Many content strategists plan in 4–8 week blocks.

---

## 4. PLATFORM COVERAGE MAP

### Platforms tracked (8 platform slots across 6 services):

| Platform | Slots | Content Types |
|----------|-------|---------------|
| **YouTube** | 2 | Long-Form Video, Short-Form (Shorts) |
| **Instagram** | 3 | Reels (New Page), Reels (Old Page), Carousel |
| **Facebook** | 1 | Page Posts + Group Shares |
| **WhatsApp** | 1 | Status / Broadcast / Group Messages |
| **Reddit** | 1 | Subreddit Posts / Comments |
| **Website/Blog** | 1 (cycle only) | Blog posts (tracked as cycle, not individual entries) |

### What's NOT included (potential add-ons for a service):
- TikTok (major gap — most content calendars now include this)
- X / Twitter
- LinkedIn
- Pinterest
- Threads
- Email Newsletter
- Podcast
- Telegram

### Content type distribution:
- **Video-first:** 5 of 8 slots are video content (YT Long, YT Short, IG Reels x2, + FB often video)
- **Image/Static:** 1 slot (IG Carousel)
- **Text/Link:** 2 slots (WhatsApp, Reddit)

---

## 5. CONTENT STRATEGY FRAMEWORK (Implied)

The calendar's column structure implies a specific content strategy methodology:

### 5.1 Hub-and-Spoke Content Model
```
Website/Blog (WB Cycle) ─── "Hub" pillar content
    ├── YouTube Long-Form ─── Deep-dive video version
    ├── YouTube Shorts ─── Micro-clips from long-form
    ├── IG Reels ─── Repurposed short clips
    ├── IG Carousel ─── Key points as visual slides
    ├── FB Page/Groups ─── Share + discussion
    ├── WhatsApp ─── Direct audience reach
    └── Reddit ─── Community engagement / value-first posting
```

### 5.2 Content Repurposing Waterfall
The column order suggests a production workflow:
1. **Plan the cycle** (WB Cycle, YT Cycle) — decide the theme/topic
2. **Produce the long-form** (YT Long-Form) — the "hero" content piece
3. **Extract short-form** (YT Shorts) — clip/edit from long-form
4. **Adapt for IG** (Reels + Carousel) — reformat for Instagram
5. **Distribute** (FB, WhatsApp, Reddit) — share across communities

### 5.3 Multi-Account Strategy
The "New Page" vs "Old Page" split for IG Reels reveals a common growth tactic:
- **Old Page:** Established audience, consistent posting to maintain
- **New Page:** Growth-focused, potentially different niche angle or rebrand
- Both get Reels but potentially different content or timing

---

## 6. TEMPLATE CUSTOMIZATION POINTS

For building a replicable/sellable service, these are the configurable parameters:

### 6.1 Date Configuration
| Parameter | Default | Customizable |
|-----------|---------|-------------|
| Start date | May 26 | Any date |
| End date | Jul 5 | Any date |
| Duration | ~6 weeks | 1 week to 12 months |
| Date format | `Ddd D Mon` | Multiple format options |
| Week start | N/A (continuous) | Monday or Sunday start |
| Include weekends | Yes | Optional rest days |

### 6.2 Platform Selection
| Parameter | Description |
|-----------|------------|
| Platform list | Client picks which platforms they use |
| Accounts per platform | Support multi-account (like IG New/Old) |
| Content types per platform | Split by format (Long/Short, Reels/Carousel/Stories) |
| Custom platform names | "TikTok Personal" vs "TikTok Business" |

### 6.3 Cycle System
| Parameter | Description |
|-----------|------------|
| Cycle columns | Which platforms get cycle tracking |
| Cycle length | 2-week, 4-week, 8-week rotation |
| Cycle labels | Custom names per phase ("Pillar", "Tutorial", "BTS", "Promo") |
| Auto-fill cycles | Pre-populate cycle labels based on pattern |

### 6.4 Visual Theming
| Parameter | Description |
|-----------|------------|
| Brand colors | Header color, accent colors |
| Row striping | Alternating colors or plain |
| Weekend highlighting | Different color for Sat/Sun |
| Today marker | Highlight current date |

### 6.5 Content Pre-Population
| Parameter | Description |
|-----------|------------|
| Niche/Industry | Determines content topic suggestions |
| Content pillars | 3-5 core themes to rotate through |
| Posting frequency per platform | How many posts per week per platform |
| Holidays/Events | Auto-mark relevant dates |
| Campaign blocks | Pre-mark launch/promo windows |

---

## 7. DATA MODEL FOR REPLICATION

### Core Schema
```
ContentCalendar {
  title: string                    // "Content Calendar - Posts"
  sheets: Sheet[]                  // Currently just one sheet
}

Sheet {
  name: string                     // "Posts"
  dateRange: {
    start: Date                    // 2025-05-26
    end: Date                      // 2025-07-05
  }
  columns: Column[]
  rows: Row[]
}

Column {
  id: string                       // "yt_long_form"
  header: string                   // "YT Long-Form"
  category: enum                   // TIME | CYCLE | PLATFORM | META
  platform?: string                // "youtube", "instagram", etc.
  contentType?: string             // "long_form_video", "short_form_video", "carousel", etc.
  accountLabel?: string            // "New Page", "Old Page"
}

Row {
  date: Date
  dayName: string                  // "Tuesday"
  cells: Map<columnId, string>     // content for each platform
}
```

### Platform Registry (for the service)
```
Platform {
  id: string                       // "instagram"
  name: string                     // "Instagram"
  icon: string                     // IG icon
  contentTypes: ContentType[]
  supportsMultiAccount: boolean
  supportsCycle: boolean
}

ContentType {
  id: string                       // "reels"
  name: string                     // "Reels"
  format: enum                     // VIDEO | IMAGE | TEXT | CAROUSEL | STORY
  maxDuration?: number             // seconds (for video)
  dimensions?: string              // "1080x1920" (for image/video)
}
```

---

## 8. EXPORT FORMATS

The original is a Google Sheets/Excel file. A replicable service should support:

| Format | Use Case |
|--------|----------|
| **Google Sheets** | Primary — collaborative, real-time, sharable |
| **Excel (.xlsx)** | Download for offline use, corporate environments |
| **CSV** | Import into scheduling tools (Buffer, Hootsuite, Later) |
| **PDF** | Print-friendly version for meetings/planning sessions |
| **Notion** | Import as Notion database with platform properties |
| **Airtable** | Import as Airtable base |
| **HTML** | Interactive web-based calendar view |
| **JSON** | API-friendly for programmatic use |

---

## 9. SERVICE PRODUCTIZATION BLUEPRINT

### What the service sells:
A **personalized, pre-filled content calendar** customized to the client's:
1. **Niche/Industry** — fitness, SaaS, e-commerce, coaching, etc.
2. **Platforms** — only the ones they use
3. **Posting frequency** — realistic cadence based on their capacity
4. **Content pillars** — 3-5 core topics derived from their business
5. **Date range** — any start date, any duration
6. **Holidays/Events** — industry-specific dates pre-marked
7. **Content ideas** — AI-generated topic suggestions per cell

### Differentiation from generic templates:
- Not just an empty grid — comes **pre-filled with content ideas**
- Content topics are **niche-specific** (not generic "post about X")
- Includes the **repurposing strategy** (how one piece becomes 5+)
- Cycle columns show the **strategic rhythm**, not just random topics
- Notes column pre-filled with **campaign timing and key dates**

### Pricing tiers (suggested):
| Tier | Includes | Price Range |
|------|----------|-------------|
| **Template Only** | Empty calendar, configured platforms, formatted | $0–$29 |
| **Strategy Calendar** | Pre-filled with content pillars + topics for 4–8 weeks | $47–$97 |
| **Full Service** | Strategy calendar + scripts/hooks + first week drafted | $197–$497 |
| **Subscription** | Monthly personalized calendar refresh + strategy call | $97–$297/mo |

---

## 10. REPLICATION CHECKLIST

### To build the calendar generator:
- [ ] Date range input (start date + duration or end date)
- [ ] Date format generator (`Ddd D Mon` pattern)
- [ ] Day name auto-fill from date
- [ ] Platform selector (checkbox list of all platforms)
- [ ] Multi-account support per platform (custom labels)
- [ ] Content type splitter (Long-Form / Short-Form per platform)
- [ ] Cycle column generator (configurable rotation pattern)
- [ ] Visual theme system (colors, fonts, row striping)
- [ ] Weekend/rest day toggle
- [ ] Holiday/event database per region
- [ ] Content pillar input (3-5 topics)
- [ ] AI content idea generator (fill cells with niche-specific suggestions)
- [ ] Export to Google Sheets API
- [ ] Export to Excel (.xlsx)
- [ ] Export to CSV
- [ ] Export to PDF
- [ ] Export to HTML (interactive version)

### To build it as a service:
- [ ] Client intake form (niche, platforms, frequency, pillars, date range)
- [ ] Calendar generation engine
- [ ] AI content suggestion engine (niche-aware topic generation)
- [ ] Repurposing strategy mapper (long-form → short-form → posts)
- [ ] Review/edit interface
- [ ] Delivery system (share Google Sheet link / download)
- [ ] Payment integration
- [ ] Template library (pre-built for common niches)

---

*Analysis completed: October 13, 2026*
*Source: Google Sheets content calendar template*
