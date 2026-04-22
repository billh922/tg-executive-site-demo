# Executive HTML Site Template
## TalentGuy.io | Built April 2026

A 4-page standalone executive profile site. Hosted free on GitHub Pages.
Better than a resume. Shareable as a LinkedIn Featured card.

---

## Files

| File | Page | Purpose |
|------|------|---------|
| `index.html` | Home | Photo, stats, positioning, doc cards |
| `onepager.html` | One-Pager | Summary, competencies, career, education |
| `bio.html` | Full Bio | Narrative bio, expertise areas, detailed career, what they want |
| `valueplan.html` | Value Plan | 30/60/90 (or 30/60/90/120) day plan |
| `styles.css` | Shared | All styles — change CSS variables to rebrand |
| `photo.jpg` | All pages | Client headshot (replace this file) |

---

## How to Customize Per Client

### Step 1 — Replace all placeholder text

Search for `[` and replace every `[PLACEHOLDER]` with real content.

| Placeholder | What to put |
|-------------|-------------|
| `[CLIENT_FIRST]` | First name |
| `[CLIENT_LAST]` | Last name |
| `[CLIENT_MIDDLE_INITIAL]` | Middle initial (or remove the `.` and use last name in italic) |
| `[CLIENT_INITIAL]` | Single letter for photo fallback (e.g. "D") |
| `[LOCATION]` | City, State |
| `[EMAIL]` | Email address |
| `[PHONE]` | Phone number |
| `[LINKEDIN_URL]` | Full LinkedIn URL |
| `[LINKEDIN_HANDLE]` | Just the handle (e.g. davideasley) |
| `[HEADLINE_SHORT]` | Short headline for meta description |
| `[SPECIALTY_1-4]` | Their 4 main areas (shown under name) |
| `[STAT_1-4_NUM]` | The big number (e.g. $166M+) |
| `[STAT_1-4_LABEL]` | Short label (e.g. COST SAVINGS) |
| `[STAT_1-4_SUB]` | Sub-label in italic (e.g. Cloud & App Rationalization) |
| `[POSITIONING_SENTENCE]` | 1-sentence hero statement |
| `[POSITIONING_FULL_SENTENCE]` | 2-3 sentence positioning para on home page |
| `[VALUE_PLAN_THEME]` | What their plan covers (for home page doc card) |

### Step 2 — Replace the photo

Drop client's headshot as `photo.jpg` in the same folder.
Square crop, min 400x400px. The template handles circular clipping.

### Step 3 — Change the color scheme (optional)

Edit the `:root` variables at the top of `styles.css`:

```css
:root {
  --nav-bg: #0F1923;    /* Nav bar color */
  --gold: #C9A84C;      /* Accent color */
  --bg: #F8F5EF;        /* Page background */
}
```

### Step 4 — Remove TalentGuy credit (white-label)

In each HTML file, find and delete:
```html
<div class="footer-credit">Executive profile built with <a href="https://talentguy.io">TalentGuy.io</a></div>
```

### Step 5 — Deploy to GitHub Pages

1. Client creates a free GitHub account at github.com
2. Create a new repository named `[their-name]` (e.g. `jerrydonwd`)
3. Upload all files (index.html, onepager.html, bio.html, valueplan.html, styles.css, photo.jpg)
4. Go to Settings → Pages → Source: Deploy from branch → main → Save
5. Live in ~2 minutes at: `[username].github.io/[repo-name]`

### Step 6 — Custom domain (optional, $12/year)

1. Client buys their domain at namecheap.com or godaddy.com
2. In repo Settings → Pages → Custom Domain → enter domain
3. In domain DNS settings: add CNAME record pointing to `[username].github.io`
4. Done — site is live at their own domain

---

## LinkedIn Featured Card Setup

This is the magic move. Each client should do this:

1. Navigate to their live site home page
2. Take a full-page screenshot (Mac: Cmd+Shift+4, then screenshot the browser)
3. On LinkedIn → Profile → Featured section → Add media → Upload image
4. Set the link URL to their GitHub Pages URL
5. Title: their name + role
6. Description: their positioning statement
7. Repeat with a second card for the Value Plan page

Result: Two professional image cards in their Featured section that look like press coverage.
When a recruiter clicks — they land on a polished executive profile site.

---

## Pricing (Bill's Model)

| Version | Branding | Price |
|---------|----------|-------|
| Add-on to coaching program | "Built with TalentGuy" footer | $497 |
| White-label (their domain, no credit) | 100% theirs | $997 |
| Standalone (no coaching) | 100% theirs | $1,497 |

---

## Client Folder Structure

When building for a client:
```
clients/[client-name]/
  site/
    index.html
    onepager.html
    bio.html
    valueplan.html
    styles.css
    photo.jpg
```

Copy this template folder to `clients/[name]/site/`, customize, done.
