# LifestyleRx Marketing Artifacts

Source of truth for marketing pieces. Git holds the **sources**; final PDFs go to the team Drive folder.

## Structure

```
brand/
  fonts/            Averta (Light–Black) + Thirsty Script Bold
  logos/            LifestyleRx logo (SVG), partner marks
  BRAND.md          Palette, type rules, usage
artifacts/
  _templates/       Parameterized layouts — change these to change every variant
  <slug>/           One variant per folder: content only
exports/            Print-ready PDFs (optional; Drive is the distribution shelf)
```

## Naming

`<audience-or-topic>-<piece-type>_<YYYY-MM>_v<n>`

Examples: `t2d-screening-flier_2026-07_v1`, `pharmacist-onepager_2026-08_v2`

Bump `v` for content changes; a new month folder for a new campaign cycle.

## Artifact index

| Slug | Piece | Audience | Status | Approved by |
|---|---|---|---|---|
| t2d-screening-flier | One-page patient flier | Patients with elevated blood sugar found at screening (T2D Network partnership) | Draft | — |
| _templates/screening-flier | Screening-flier layout template | — | Active | — |

## Making a variant

Duplicate an `artifacts/<slug>/` folder and change the content properties — eyebrow, headline (and the Thirsty Script word), intro, program tiles, benefits, stats, "who it's for" chips, CTA steps, QR image, footer. Grid, type scale, colour and page geometry live in `_templates/screening-flier/` and should only be edited there, once, for all variants.

## Working on an artifact

Each `artifacts/<slug>/` folder is self-contained and opens in a browser — no build step. Fonts and logos are referenced from `brand/`.
