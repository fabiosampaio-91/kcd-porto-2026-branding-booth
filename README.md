# synvert xgeeks at KCD Porto 2026: Branding and Booth Plan

Internal team presentation for xgeeks on how synvert xgeeks shows up at **KCD Porto x DevOps Days Portugal 2026** (19 + 20 November 2026, Super Bock Arena / Palacio de Cristal, Porto): what we do at our booth, how we brand the rest of the venue, and why we host the CTO's Dinner.

**Live site:** https://fabiosampaio-91.github.io/kcd-porto-2026-branding-booth/
**PDF:** [KCD-Porto-2026-Branding-and-Booth.pdf](KCD-Porto-2026-Branding-and-Booth.pdf)

## Who it is for

The internal xgeeks team preparing the event (marketing, sales, people, the organising crew). It is a working document: several slides end in options to pick from and the last slide is a list of open decisions with owners still to be assigned.

## What is in the deck (21 slides)

1. **Framing.** All eyes will be on us: we are the legal entity behind KCD Porto and DevOps Days Portugal, and everyone coming from GL, Hitachi and Synvert has to feel the conference is ours. Three objectives: brand exposure, business development, hiring where relevant. Key numbers: 10+ sponsors, 20-30 qualified conversations, 10+ qualified leads as the target.
2. **Pillar 01, the Booth.** The "Stand KCD" spot on Piso -1 sits at the bottom of the entrance stairs: it is the ticket in. Reuse last year's backdrop with a printed cover strip ("synvert xgeeks, a Synvert GL Company"), new TV frame, new front panels for two tables, possibly two screens, a high table with a conversation hook (wording options for a business and a technical angle), Instax corner, games and giveaways, with the budget as an open question.
3. **Pillar 02, branding across the venue.** Every sponsor asset that does not get sold, we use ourselves: check-in backdrop (wording options from subtle to explicit), side room naming, the xgeeks Lounge on Piso 0 (no plaque exists, so we create the visual asset that spreads the name, plus a high table with a business hook), wifi name and password, lanyards, barista and coffee rollup (pun options), the "Sponsor room brought to you by synvert xgeeks" sign at the foyer, water bottles.
4. **Pillar 03, CTO's Dinner.** The official welcome dinner on day one, sponsored by synvert xgeeks, and why it matters for business development and for our stakeholders.
5. **Open decisions and next steps** with owners to be assigned.

## How to open it

### Website

Open the live site above, or open [`index.html`](index.html) locally in any modern browser. No build step, no external dependencies: everything the page needs is in this repository.

- **Keyboard:** arrow keys, space, Page Up / Page Down, Home / End. `F` toggles fullscreen.
- **Mouse / touch:** scroll or swipe; each slide snaps into place on desktop. On a phone the slides flow as sections of one page.
- **Deep links:** `index.html#s7` opens slide 7.
- **Buttons:** the arrows in the bottom-right corner also move between slides.

### PDF

[`KCD-Porto-2026-Branding-and-Booth.pdf`](KCD-Porto-2026-Branding-and-Booth.pdf) is a 16:9 export of the same slides, ready to share or print. GitHub previews it directly.

To regenerate the PDF after editing `index.html` (macOS, uses the installed Google Chrome):

```bash
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless=new \
  --no-pdf-header-footer --virtual-time-budget=5000 \
  --print-to-pdf="KCD-Porto-2026-Branding-and-Booth.pdf" index.html
```

The page carries a print stylesheet (`@page` size 1280 x 720 px, one slide per page), so any Chromium-based browser's "Print to PDF" gives the same result.

## Repository layout

```
index.html                              the presentation (website and PDF source)
KCD-Porto-2026-Branding-and-Booth.pdf   PDF export of the deck
assets/                                 all images used by the slides
sources/                                the source material the deck was built from
```

### Assets

- `cover-palacio.jpg`, `kcd-logo-white.png`, `kcd-logo-porto.png`, `devopsdays-logo.png`, `cncf-icon.png`: taken from the KCD Porto 2026 CEO presentation (same cover, same logos).
- `plan-piso-1-stand-zoom.png`, `plan-piso-1-full.png`: official Piso -1 floor plan with the Stand KCD highlighted.
- `plan-piso0-lounge-zoom.png`, `plan-piso0-full.png`: official Piso 0 floor plan with the lounge (sofas and poufs) highlighted.
- `booth-2025.jpg`: the synvert xgeeks booth at KCD Porto 2025.
- `venue-*.jpg`, `team-2025.jpg`, `stage-*.jpg`, `*-booth-2025.jpg`, `audience-2025.jpg`, `lunch-2025.jpg`, `podium-kcd.jpg`, `porto-ribeira.jpg`: venue and event photos from the sponsorship prospectus and the CEO presentation. A few are not shown in the slides and are kept for follow-up material (social posts, briefs for the print supplier).

### Sources

- `KCD_Porto_2026_CEO_Presentation.pdf`: visual identity (colours, fonts, cover), venue images, event numbers.
- `KCD_Porto_2026_Storytelling.pdf`: the extended business case (lead generation and reach figures).
- `KCD_Porto_x_DevOps_Days_2026_Sponsorship_Prospectus_150dpi.pdf`: sponsor packages and add-on prices (barista, lanyards, wifi, room naming). Size-reduced copy at 150 dpi; the original is 116 MB, above GitHub's file size limit.
- `KCD26_Planta-Centro-Congressos-SBA_Piso0_150dpi.pdf` and `KCD26_Planta-Centro-Congressos-SBA_Piso-1_150dpi.pdf`: official venue floor plans (05/2026), rendered at 150 dpi for the same reason.
- `xgeeks-booth-kcd-porto-2025.png`: photo of last year's booth.

## Visual identity

Colours and fonts follow the KCD Porto 2026 CEO presentation: blue `#0828B2`, accent blue `#0086FF`, cyan `#93EAFF`, pink `#D62293`, light grey `#E5E5E5` background; Trebuchet MS for headings and Calibri (with fallbacks) for body text.
