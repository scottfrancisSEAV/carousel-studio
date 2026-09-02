# Brand assets

## What is here

| File | Purpose | Source |
| --- | --- | --- |
| `avior-logo.png` | Primary lockup — mark plus wordmark, for **light** slide backgrounds | `website.aviormarine.com/AviorLogo3.png` |
| `avior-logo-mark.png` | Compass mark alone | `website.aviormarine.com/avior logo.png` |

Both were downloaded from Avior Marine's own website on 19 August 2026 with their transparent
backgrounds intact, and had their empty padding trimmed (1920 × 1080 → 1422 × 1022, and 689 × 689 →
644 × 669). **Nothing was recoloured, redrawn or reproportioned** — trimming removes transparent
space only, so the artwork and its aspect ratio are untouched.

## What is still missing

| File | Purpose | Status |
| --- | --- | --- |
| `avior-logo-reversed.png` | White/reversed lockup for **dark** slide backgrounds | **not supplied** |

The published lockup is drawn for light backgrounds: navy star segments, a blue "AVIOR" and a black
"MARINE INC.". The studio also places the logo on dark backgrounds — the cover slide is Avior blue
and the verification and safety slide is deep navy — where those elements disappear.

Avior has not published a reversed lockup, and **the studio will not invent one**: recolouring a logo
is redrawing it. Until the brand owner supplies the file, the dark slides show the visible
`AVIOR LOGO PLACEHOLDER`, which is the honest outcome. Drop the reversed asset in at this path and
those slides pick it up with no code change.

A unit test asserts that the two shipped assets exist and that the reversed one does not — so when
it arrives, the test flips and tells you.

## Approval

Every variant ships with `approved: false`. These are the correct assets, but only the brand owner
can mark them cleared for use — a tick box in the studio's **Brand** section. Variants are keyed by
the background they are cleared for (`light`, `dark`, `any`), and each slide requests the variant
matching its own background.

The logo is always rendered at its natural aspect ratio with `object-fit: contain`, at 92 px height
on the 1080 px design canvas.
