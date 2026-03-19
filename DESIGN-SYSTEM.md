# Felport Capital — Design System

## 1. COLOR SYSTEM

### Primary
| Role       | Name         | HEX       | Usage                                      |
|------------|-------------|-----------|---------------------------------------------|
| Primary    | Navy        | `#003358` | Headlines, buttons, nav, footer background  |
| Secondary  | White       | `#FFFFFF` | Backgrounds, button text on dark, body bg   |

### Accent
| Role       | Name         | HEX       | Usage                                      |
|------------|-------------|-----------|---------------------------------------------|
| Accent     | Slate Blue  | `#1A5276` | Hover states, active links, secondary CTA   |
| Gold Muted | Warm Sand   | `#C5A96A` | Sparingly — divider accents, pillar numbers |

### Neutrals
| Role       | Name         | HEX       | Usage                                      |
|------------|-------------|-----------|---------------------------------------------|
| Charcoal   | Dark Text   | `#2C3E50` | Body text primary                           |
| Mid Gray   | Muted Text  | `#5D6D7E` | Captions, secondary text, descriptions      |
| Soft Gray  | Borders     | `#D5D8DC` | Dividers, card borders, form borders        |
| Light Gray | Backgrounds | `#F2F3F4` | Card backgrounds, alternate section bg      |
| Off White  | Canvas      | `#F8F9F9` | Hero background, section alternation        |

### Usage Rules
- Navy (`#003358`) is used ONLY for: headlines, nav background (scrolled), footer, buttons, strong borders
- Body text is ALWAYS Charcoal (`#2C3E50`), never pure black
- Backgrounds alternate between White and Off White — never consecutive dark sections except footer
- Gold (`#C5A96A`) used at max 5% of any page — reserved for subtle accents only
- Dividers use Soft Gray (`#D5D8DC`) at 1px
- Dark sections (Contact, Footer) use Navy as background with White text

---

## 2. TYPOGRAPHY SYSTEM

### Font Stack
- **Serif:** `'Cormorant Garamond', Georgia, serif` — Headlines (H1, H2, H3), logo, pillar numbers
- **Sans-serif:** `'Inter', -apple-system, 'Segoe UI', Helvetica, Arial, sans-serif` — Body, captions, labels, navigation, buttons

### Hierarchy

| Element   | Font          | Weight | Size (desktop)     | Size (mobile)   | Line Height | Letter Spacing | Transform   |
|-----------|---------------|--------|--------------------|-----------------|-------------|----------------|-------------|
| H1        | Serif         | 500    | 3.5rem (56px)      | 2.5rem (40px)   | 1.12        | -0.01em        | None        |
| H2        | Serif         | 500    | 2.25rem (36px)     | 1.75rem (28px)  | 1.25        | -0.01em        | None        |
| H3        | Serif         | 600    | 1.5rem (24px)      | 1.25rem (20px)  | 1.3         | 0              | None        |
| Body      | Sans-serif    | 300    | 1rem (16px)        | 1rem (16px)     | 1.75        | 0              | None        |
| Body SM   | Sans-serif    | 300    | 0.95rem (15.2px)   | 0.95rem         | 1.7         | 0              | None        |
| Caption   | Sans-serif    | 400    | 0.85rem (13.6px)   | 0.8rem          | 1.5         | 0.04em         | None        |
| Label     | Sans-serif    | 500    | 0.78rem (12.5px)   | 0.75rem         | 1.4         | 0.1em          | Uppercase   |
| Nav Link  | Sans-serif    | 400    | 0.85rem (13.6px)   | 1.1rem          | 1           | 0.04em         | Uppercase   |
| Button    | Sans-serif    | 500    | 0.85rem (13.6px)   | 0.85rem         | 1           | 0.06em         | Uppercase   |

### Rules
- Serif is ONLY for headings and decorative numbers — never for body text
- Sans-serif body weight is 300 (light) for elegance; 400 for captions; 500 for labels/buttons
- Never use bold (700+) on body text
- Maximum 2 font sizes per visual block

---

## 3. LAYOUT & SPACING

### Spacing Scale (8px base grid)
| Token | Value  | Usage                           |
|-------|--------|---------------------------------|
| xs    | 4px    | Tight internal gaps             |
| sm    | 8px    | Icon gaps, tight padding        |
| md    | 16px   | Form field padding, small gaps  |
| lg    | 24px   | Card internal padding           |
| xl    | 32px   | Column gaps                     |
| 2xl   | 48px   | Between content blocks          |
| 3xl   | 64px   | Section padding (mobile)        |
| 4xl   | 96px   | Section padding (desktop)       |
| 5xl   | 112px  | Section padding (large)         |

### Container
- Max width: `1120px`
- Horizontal padding: `clamp(1.25rem, 4vw, 2.5rem)`
- Centered with `margin: 0 auto`

### Section Padding
- Desktop: `96px` top and bottom (6rem)
- Mobile: `64px` top and bottom (4rem)

### Grid
- 2-column: Used for header+body layouts (About, Approach, Contact)
- 3-column: Used for cards/pillars (About pillars, Focus cards)
- 4-column: Used for inline lists (Other Investment Strategies)
- 5-column: Used for Transaction Types
- Gap: `clamp(2rem, 5vw, 4rem)` between grid columns
- Always left-aligned text — never center-aligned body text

---

## 4. UI ELEMENTS

### Buttons
**Primary (dark on light background):**
- Border: 1.5px solid `#003358`
- Text: `#003358`
- Background: transparent
- Hover: Background `#003358`, text `#FFFFFF`
- Padding: 14px 36px
- Transition: 0.35s ease

**Secondary (light on dark background):**
- Border: 1.5px solid `#FFFFFF`
- Text: `#FFFFFF`
- Background: transparent
- Hover: Background `#FFFFFF`, text `#003358`
- Same padding and transition

**Rules:**
- No border-radius (sharp corners)
- No shadows
- No gradient fills
- No icons inside buttons

### Form Fields
- Background: `rgba(255,255,255, 0.06)` on dark
- Border: 1px solid `rgba(255,255,255, 0.15)` on dark
- Focus border: `rgba(255,255,255, 0.4)`
- Padding: 14px 16px
- Font: Sans-serif, 1rem, weight 300
- Labels: uppercase, 0.8rem, weight 500, `rgba(255,255,255, 0.5)`
- No border-radius

### Cards
- Background: `#F2F3F4`
- Padding: 2rem (32px)
- No border-radius
- No shadow
- Internal divider: 1px solid `#D5D8DC`

### Dividers
- Section dividers: 1px solid `#D5D8DC`, full container width
- Card internal: 1px solid `#D5D8DC`
- Accent borders (transaction items): 2px solid `#003358`, top only

---

## 5. IMAGE STYLE GUIDELINES

### Use
- Architecture: modern buildings, skylines, structural details
- Industrial: manufacturing floors, logistics, infrastructure
- Business: professional settings, conference rooms, handshakes (real, not staged)
- Landscape: regional landmarks (Cerro de la Silla, Monterrey skyline)

### Avoid
- Generic stock photos with forced smiles
- Flat illustrations or startup-style graphics
- Overly staged corporate photos
- Photos with text overlays or watermarks
- Bright, saturated colors

### Treatment
- Slight desaturation for consistency (filter: `saturate(0.85)`)
- Maintain natural contrast — do not wash out
- Object-fit: cover, always
- Consistent aspect ratios within each section
- No rounded corners on images
- No borders or shadows on images

---

## 6. TONE & VISUAL PRINCIPLES

1. **Timeless over trendy** — No design fads. Every element should look appropriate 10 years from now.
2. **Understated over expressive** — Let white space and typography communicate, not decoration.
3. **Clarity over complexity** — Every element must serve a purpose. If it does not inform, remove it.
4. **Restraint over abundance** — Fewer elements, better executed.
5. **Structure over style** — Strong grid, consistent spacing, predictable hierarchy.
6. **Credibility over persuasion** — The design should convey competence and trust, not sell.
7. **Precision over approximation** — Exact alignment, consistent spacing, no visual noise.

---

## 7. DO / DON'T

### DO
- Use generous white space
- Maintain strict alignment to grid
- Use serif for headlines, sans-serif for body
- Keep color palette within defined system
- Use sharp corners on all elements
- Maintain consistent vertical rhythm
- Use subtle, smooth transitions (0.3s–0.4s ease)

### DON'T
- Use gradients anywhere
- Use bright or saturated accent colors
- Use rounded corners (border-radius)
- Use drop shadows or glows
- Use icons or emoji in content
- Use startup-style illustrations
- Use more than 2 typefaces
- Use centered body text
- Use animations that draw attention (bounce, shake, pulse)
- Use stock photo cliches (chess pieces, puzzle pieces, handshake silhouettes)
- Use decorative borders or ornaments
