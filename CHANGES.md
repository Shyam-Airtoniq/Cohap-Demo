# COHAP Homepage — Changes Summary

Revisions made based on client feedback (email + initial meeting + feedback meeting).

## Files in this repo

| File | Purpose |
|---|---|
| `index.html` | Landing page — preview & pick between the two header variants |
| `index1.html` | **Variant 1**: compact single-row header |
| `index2.html` | **Variant 2**: two-tier header with prominent logo (brand row collapses on scroll) |
| `index_proposed.html` | Original first-pass mockup, kept for reference |

---

## Branding

- Switched to the official brand palette from the branding guide PDF:
  - Brand blue **#2D3D7B**
  - Brand gold **#c7862b**
  - Supporting tones: deep navy `#28306c`, light blue `#6A78D1`, light gold `#efac73`
- Updated typography: **Montserrat** for headings, **Open Sans** for body (closest web-safe match to Javanese Text + Montserrat Bold from the guide).
- Replaced the placeholder logo with the singular brand logo (`bigger bird_dullercolor.png`) in header and footer.
- Added placeholder for the Candid Platinum Transparency badge (hero + footer).

## Navigation

Restructured to exactly match client direction:

- **Who We Are** *(was "About")* — Mission, Vision, Goals, Five Core Values, Our Story, About Our Founder, About Our Team
- **Programs** — Housing, Education, Entrepreneurship, Mental Wellness, Mentoring *(age range updated to 12–25)*
- **Get Help** — Request Assistance *(removed "Overview & Eligibility" per feedback)*
- **Get Involved** —
  - Join Our Advisory Board
  - Join a Committee
  - Volunteer for Events Registration
  - Community Vendor Registration
  - Volunteer Opportunities
  - Become a Sponsor *(consolidates all sponsorship flows)*
- **Events** *(standalone)*
- **News & Impact** —
  - Press Releases
  - Media Appearances
  - **Gallery** *(new — added per request)*
  - Newsletters
  - **Impact Reports** with year submenu (2023 / 2024 / 2025)
- **Contact Us** *(standalone)*

## Homepage Content

- **"Breaking the Cycle of Homelessness"** kept prominent in the hero, with a positive subhead.
- New **Facts** section (3 concise stats + "Check the Facts" button linking to a future dedicated facts page).
- New **Story/Video** section with a play-button placeholder, ready for Natasha's testimonial video.
- New **Gallery preview** with "View Full Gallery" CTA.
- **Larger, circular social icons** in the footer (Facebook, YouTube, Instagram, LinkedIn, X, TikTok).
- Hover state added to the "How We Help" outline button — fills with light blue.
- Sponsorship CTAs consolidated under a single "Become a Sponsor" page.

## Imagery

- Replaced the prison/bars-feel hero image with a community-service placeholder from Unsplash (food-drive volunteers).
- Other section images (`education.jpg`, `wellness.jpg`, etc.) left in place pending the client's high-res replacements + section-mapping guidance.

## Header — Variant 2 specifics

- Two-tier header: large logo + wordmark + phone/email + Donate on the top row, navigation menu on the row below.
- **Brand row collapses smoothly on scroll**, leaving only the nav menu sticky.
- Built with `IntersectionObserver` (not scroll events) plus hysteresis (140px collapse threshold, 40px expand threshold) and `overflow-anchor: none` to prevent the browser-scroll-anchoring oscillation seen in earlier iterations.

## Files not in the repo (kept local)

`.gitignore` keeps these out:

- `transcript1.md`, `transcript2.md` — meeting transcripts
- `email.md` — client feedback email
- `COHAP BRANDING guide.pdf` — branding asset PDF

---

## Outstanding — pending from client

- High-resolution photos + section-by-section guidance (which photo goes where)
- Final color codes if different from the branding guide
- Singular logo file (currently using `bigger bird_dullercolor.png`)
- Platinum transparency logo file (placeholder used)
- Testimonial video file
- Photos for: hero, education, recidivism, gallery
- Stripe / sponsorship payment page URLs to link from the Get Involved → Become a Sponsor flow
