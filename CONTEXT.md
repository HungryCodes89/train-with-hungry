# Train With Hungry — Site Context

## Brand Identity
- **Coach:** Sean "Hungry" Norgan
- **Brand name:** Train With Hungry
- **Tagline:** Feed What Matters.
- **Email:** sean@trainwithhungry.com

## Specialties
1. Kettlebell & Mace Training
2. Ancestral Nutrition & Diet
3. Natural Hormone Optimization
4. Men's Shadow Work & Integration Coaching
5. Personal Accountability Systems
6. Breathwork

## Tone
Primal, sovereign, cinematic, masculine, esoteric but grounded.
Ancient warrior meets modern high performer. Not a gym bro. Not a wellness guru.

## Aesthetic (v3 — current)
- Background: `#060608` near-black
- Accent: `#C8FF3E` electric lime — NOT amber
- Text: `#F2F0EA` warm white
- Muted text: `#8C8D96` (must stay above this — anything darker is unreadable)
- Fonts: **Bebas Neue** (all headlines) + **Inter** (body)
- Grain overlay (CSS SVG feTurbulence, body::before)
- No glassmorphism cards — clean typographic layouts only
- Custom cursor: lime dot + ring, desktop only

## Technical Stack
- Single HTML file — no build tools
- CDN: GSAP 3.12.5 + ScrollTrigger, Lenis 1.0.42
- Google Fonts: Bebas Neue, Inter
- No canvas — CSS animated gradient hero background
- Ghost text watermark: "TRAIN WITH HUNGRY" at bottom of hero

## Sections & Key Decisions
1. **Preloader** — Status lines appear (SYSTEM / COACH / MODE / STATUS), then massive `%` counter fills to 100, full-width lime progress bar glows, then screen wipes upward via clip-path reveal
2. **Nav** — Fixed, glassmorphism on scroll, "TRAIN WITH HUNGRY" Bebas logo left, lime CTA right
3. **Hero** — Left-aligned, full-viewport. Stat bar at bottom: `6 Disciplines / 1:1 Private Coaching / 90 Day Transformation / 0 Excuses Tolerated`
4. **Philosophy** — Rotated vertical sidebar label, full paragraph with em/strong highlights
5. **Disciplines** — Horizontal numbered list rows (01–06), title + right-aligned short desc, hover turns title lime
6. **The Method** — 3-col grid: 01 Hunger / 02 Forge / 03 Embody. Large ghosted lime numbers behind text
7. **Who This Is For** — 5 statements. First 3 use "For the man who...", last 2 break cadence deliberately. Hover slides text right with lime bar. No &nbsp; in em tags.
8. **Work With Me** — 2-col: left = offer list + CTA, right = large editorial quote with lime left border
9. **Footer** — Bebas brand name, lime tagline, muted social links

## Who This Is For — copy (locked)
- For the man who is done being *comfortable.*
- For the man who has tried every program — and knows the problem was never the *program.*
- For the man who feels the gap between who he is and who he *knows he could be.*
- Done explaining yourself. Ready to start *becoming* yourself.
- You understand that suffering avoided is *potential abandoned.*

## Offer
**The Sovereign Program** — 1-on-1 Private Coaching
- Custom kettlebell & mace training protocols
- Ancestral nutrition blueprint, built for your body
- Natural hormone optimization roadmap
- Weekly 1-on-1 accountability check-ins
- Shadow work & integration sessions
- Breathwork protocol for performance & recovery

## Design Rules (do not break)
- `--muted` must stay at `#8C8D96` or brighter — darker is unreadable on the dark bg
- No &nbsp; inside em tags — creates visible gap before highlighted word
- No bento/glassmorphism cards — that was v2, not this direction
- Ghost watermark text uses `-webkit-text-stroke` only, never fill color
- Who lines: use `padding-left` slide on hover, NOT flex gap + ::before width (causes text jump)
- Preloader must be visible minimum ~3 seconds before exit

## Version History
- v1 — Original concept prompt (never built, just the prompt text)
- v2 — First full build: Cinzel + Space Grotesk, obsidian/ember palette, particle canvas, bento cards
- v3 — Complete redesign: Bebas Neue + Inter, electric lime on near-black, horizontal discipline list, proper preloader, no cards
  - v3.1 — Contrast fixes: muted text brightened, who-lines opacity up, blockquote opacity up
  - v3.2 — Who This Is For audit: removed text-jump hover bug, fixed &nbsp; copy artifacts, varied cadence on last 2 lines
