# Hill St. Kiosk — Design System

Extracted from Figma file (Page 1: home-1440, book, gallery).

---

## Colors

| Name | Hex | Usage |
|---|---|---|
| Sage Green | `#c4ddce` | Sidebar background |
| Sage Green (light) | `#cfe5d8` | Active nav item highlight |
| White | `#ffffff` | Main content background |
| Black | `#000000` | Primary text |
| Dark Gray | `#353535` | Secondary text, Classic tier header |
| Mid Gray | `#cfcfcf` | Classic tier price row |
| Light Gray | `#c5c5c5` | Image placeholder border |
| Button Gray | `#b0b0b0` | Button stroke |
| Logo Red | `#fe4531` | Logo icon (top shape) |
| Logo Green | `#407656` | Logo icon (bottom shape) |
| Premium Red | `#c90000` | Premium tier header |
| Premium Pink | `#ffdede` | Premium tier price row |
| Signature Gold | `#ffc955` | Signature tier header |
| Signature Cream | `#fff1d4` | Signature tier price row |

---

## Typography

### Fonts in use

| Font | Weights/Styles | Where used |
|---|---|---|
| Helvetica Neue | Bold | Site title "Hill St. Kiosk" |
| Times New Roman | Bold, Regular, Italic | Headings, body, contact, footer |
| Brush Script MT | Italic | Sidebar nav links |

### Font Sizes

| Size | Font | Usage |
|---|---|---|
| 56px | Helvetica Neue Bold | Page title |
| 24px | Times New Roman Bold | Section subheadings ("Ready to book?", "Welcome to…") |
| 24px | Brush Script MT Italic | Sidebar nav link labels |
| 18px | Times New Roman Bold | Section labels ("Contact Us!", "Question?") |
| 18px | Times New Roman Regular | Body copy, email address |
| 14px | Times New Roman Regular | Footer attribution |
| 14px | Times New Roman Italic | Copyright line |

---

## Spacing Patterns

| Pattern | Value |
|---|---|
| Sidebar width | **200px** (fixed rule — hard-coded in all HTML files, do not derive from Figma) |
| Main content width | 1254px |
| Total canvas width | 1440px |
| Logo top offset | 80px from top |
| Nav item height | 45px |
| Nav starts at | y = 254px |
| Content column width | ~480px (centered in main area) |
| Pricing card width | 560px |
| Tier title row height | 39px |
| Tier price row height | 39px |
| Tier content row height | 106px |

---

## Reusable Components

### 1. Sidebar
- **200px wide** (fixed rule — hard-coded, do not change)
- Full viewport height
- Sage green background (`#c4ddce`)
- Contains: logo + nav list

### 2. Nav Links (`sidebar-pages`)
Two states, each 200×45px:
- **Default** (`page-default`) — no fill
- **Selected** (`sidebar-page-selected`) — fill `#cfe5d8`
- Labels: Home, Book, Gallery, About — Brush Script MT Italic 24px

### 3. Pricing Cards (`tier-box`)
Three tiers, each 560×184px with a black stroke border:

| Tier | Header color | Price row color | Price |
|---|---|---|---|
| CLASSIC | `#353535` dark gray | `#cfcfcf` light gray | $450–550/event |
| PREMIUM | `#c90000` red | `#ffdede` pink | $750–900/event |
| SIGNATURE | `#ffc955` gold | `#fff1d4` cream | $950–1100/event |

Each card: title row (39px) → price row (39px) → 3 content boxes (106px total)

### 4. Send Button
- Size: 57×29px
- Fill: linear gradient `#ffffff` → `#f1f1f1`
- Stroke: `#b0b0b0`
- Label: "Send" (Times New Roman)

### 5. Form Inputs
- Single-line input: 560×29px
- Textarea: 560×109px

### 6. Image Placeholder (`missing-img-wrap`)
- 240×120px, white fill, `#c5c5c5` stroke

### 7. Image+Text Cards (`img-text`)
- 224×143px — image on top, body text (Times New Roman Regular 18px) below

### 8. Contact Section
- Heading: Times New Roman Bold 18px, `#000000`
- Email: Times New Roman Regular 18px, `#000000`

### 9. Footer
- Attribution: Times New Roman Regular 14px, `#000000`
- Copyright: Times New Roman Italic 14px, `#353535`

---

## Notes

No registered Figma styles, variables, or formal component library exist yet — everything is applied ad-hoc. Top candidates to formalize:
- Sidebar nav items (two clear states)
- Pricing cards (repeated 3-tier structure)
- Send button
