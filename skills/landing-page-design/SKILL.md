---
name: landing-page-design
description: "Complete design system for building or redesigning landing pages, websites, web apps, and live stream overlays: intake, page structure, conversion copy, SEO, strict rules for type, spacing, radius, color, icons, and motion, an audit and fix flow for existing sites, broadcast rules for OBS (camera frames, chat, video players, alerts, goals, timers, stingers, control docks), and a switchable aesthetic layer (esports, neon, pixel, cozy, editorial, brutalist, glass, or custom). Use it whenever building, editing, redesigning, restyling, auditing, or writing copy for ANY landing page, website, web app, component, prototype, stream overlay, scene, webcam frame, chat box, alert, or video player, including when the user says a page looks bad, cheap, generic, or AI made, or asks to change its look, theme, or vibe. Consult it before choosing sections, headlines, CTAs, fonts, sizes, spacing, radii, colors, icons, transitions, or overlay layout."
---

# Landing Page Design

A landing page is not a homepage. A homepage serves multiple intents. A landing page wins one intent:

**one offer → one audience → one primary action.**

An overlay is not a web page either. Nobody scrolls it, hovers it, or clicks it. It is composited over video, compressed, and watched on a phone for hours:

**one canvas → one scene at a time → never in the way of the content.**

This skill has five parts. **Part A** decides what a landing page says and how it is structured. **Part B** is the default visual system, and it is non negotiable unless an aesthetic from Part D is active. **Part C** adapts that system to stream overlays, video players, and interactive widgets. **Part D** is the aesthetic layer: it defines which visual values may change when the user asks for a different look (neon, pixel, cozy, esports, and so on), which never change, and how to switch looks without rebuilding anything. **Part E** redesigns something that already exists, a normal website, web app, component, or overlay: it audits it against B, C, and D, moves its values into tokens, and fixes it in place without breaking what works. Work through A (or the C1 intake for overlays, or the E2 scan for redesigns) before touching B.

## Scope

Apply to all web UI work: landing pages, marketing sites, normal websites, web apps, components, dashboards, prototypes, stream overlays, embedded players, redesigns, and design reviews. When a rule here conflicts with a framework default, this file wins. When the user's explicit prompt conflicts with a rule, the user wins.

**Which parts apply**

| Building | Part A | Part B | Part C |
|---|---|---|---|
| Landing page or marketing site | Yes | Yes | Only C7 (video player) and C9 (interactions) if the page has them |
| Stream overlay, scene, alert, or chat widget | No, use C1 instead | Yes, with the C0 overrides | Yes |
| Streamer control dock or settings panel | No | Yes, fully, it is a normal interactive UI | C10 for how it talks to the overlay |
| Standalone video player or camera app | No | Yes | C5 camera, C7 player, C9 interactions |
| Twitch overlay extension (viewers click it) | No | Yes, fully, with B9 states | C2 safe areas, C3 legibility, C9 |
| Static stream package (panels, banners, offline screen, emotes) | No | Yes | C13 |
| Existing website, web app, or component (redesign) | A4, A5, and A8 only if it is a marketing page | Yes, through the E3 audit | C7 and C9 if it has video or widgets |
| Existing overlay or provider widget (redesign) | No | Yes, with the C0 overrides | Yes, as the E9 audit |

**Part D applies on top of any row** as soon as the user names a look, mood, vibe, reference, or theme. With no aesthetic named, the **Base** aesthetic is active, which is Part B exactly.

**Part E applies** whenever the work starts from something that already exists, rather than from a blank page: "improve", "polish", "fix", "modernize", "redesign", "it looks cheap or generic", or "make my site look like X".

**Companion skill.** Part E covers the same ground as the standalone `redesign-existing-projects` skill ([github.com/elayadesign/redesign-skill](https://github.com/elayadesign/redesign-skill)), extended with the aesthetic layer and overlays. If both are installed, follow Part E; the values agree.

---

# PART A — Strategy and structure

## A1. Intake

Gather these before designing or writing. Ask only for what is missing, and ask in one batch rather than one question at a time.

**Purpose**
- What is the ONE primary action? (trial, demo, buy, waitlist, download)
- What is the offer, exactly what do they get?
- What counts as a conversion? (click, signup, purchase)

**Audience and context**
- Who is the ICP?
- What problem are they trying to solve?
- Top three objections, meaning why they do not convert today
- Traffic source: ads, search, social, email
- What do visitors already know when they land?

**Proof and assets**
- Proof points: logos, testimonials, numbers, case studies
- Screenshots, demo video, product GIFs
- Guarantees, refund terms, cancellation terms

**Constraints**
- Brand voice: casual or professional
- Design direction: minimal editorial, playful 3D, glass UI
- Mobile priority?

If the user cannot answer, make a reasonable assumption, state it in one line, and continue. Do not stall the build.

## A2. Page structure

**Above the fold (required)**
1. Headline, outcome plus audience
2. Subheadline, clarifies how and adds specificity
3. Primary CTA, clear verb plus what they get
4. One proof signal, logo strip, stat, or short testimonial
5. Hero visual, product screenshot or video, or a strong illustration

**Mid page (the argument)**
6. Problem to solution, one section
7. Benefits, three to five, outcome driven
8. How it works, three steps
9. Social proof, testimonials or a case study

**Bottom (objection handling)**
10. FAQ, six to twelve questions
11. Risk reversal, trial, cancel anytime, guarantee
12. Final CTA, identical to the top

Include the mandatory tagline reveal section from B11 somewhere in the mid page argument, typically right after the hero or after benefits.

## A3. Layout selection

Pick one and say why.

| Type | Use when |
|---|---|
| **A. Classic hero plus sections** | The product is understandable from a hero screenshot. Most common. |
| **B. Long form story** | You need to educate and overcome skepticism. |
| **C. Minimal conversion page** | High intent traffic (email to known users), or a short offer like a download or waitlist. |
| **D. Comparison page** | Search intent includes alternatives ("X vs Y", "best for"). Usually paired with SEO pages. |

## A4. Conversion rules

**Match message to source.** If traffic comes from ads, mirror the ad headline in the hero and keep the same promise and visual tone.

**Make the next step obvious.** One primary CTA. Never place competing CTAs above the fold.

**Write benefit first.** Features are what it does. Benefits are what that means for them.

**Be specific.**
- ❌ "Save time and streamline"
- ✅ "Cut your weekly reporting from 4 hours to 15 minutes"

**Reduce risk.** Pick at least one: free trial, free plan, no credit card, cancel anytime, money back guarantee.

**Treat objections as a section, not a footnote.** Move the FAQ earlier for high friction offers. Put proof directly beside the claim it supports.

## A5. Copywriting

**Headline formulas**
- "{Outcome} without {pain}"
- "The {category} for {audience}"
- "Ship {result} in {time}"

**Subheadline.** One or two sentences. Clarify what it is and who it is for.

**CTA.** Verb plus what they get. Never "Learn more" or "Submit". Use "Start free trial", "Book a demo", "Get the checklist".

**Benefit bullets.** Bold benefit, then the proof or detail. Example: **Faster iteration** — generate three layout variants in one click.

Note: the copy rules in B1 still apply. No hyphens inside sentences, no orphaned words.

## A6. Build order

Work section by section, in this order:

1. Hero
2. Benefits
3. How it works
4. Proof
5. FAQ
6. Final CTA

Never rebuild the whole page on each iteration. Section by section keeps control and keeps diffs reviewable.

## A7. SEO and AEO

**Do not index** ad only campaign pages or highly time bound offers. Use `noindex` or keep them behind a non indexed path.

**Do index** evergreen offers and pages where search intent matches the promise. Add a clear title and meta description, internal links from the homepage and feature pages, and the FAQ in plain question and answer form for AEO. Add FAQ schema if appropriate.

## A8. Pitfalls

- Too many CTAs above the fold
- Vague value prop: "streamline", "optimize"
- A large feature list with no outcomes
- Proof buried at the bottom
- Mobile layout that breaks readability
- No clear next step

---

# PART B — Visual system

Every visual value must resolve through these rules instead of being invented ad hoc.

## B1. Typography

### Fonts

**Use:** Geist, Manrope, Geist Mono, Poppins.

**Never use:** Inter, Roboto, Arial, Open Sans, Helvetica.

**Never use italic fonts** anywhere in the interface.

**One typeface per site.** Do not pair two fonts unless the prompt explicitly asks for it. Geist Mono is allowed alongside a primary font only for code, data, or numeric UI where a monospace is functionally required.

**Never use ultra bold weights** (900 / black). Cap at semibold or bold.

### Copy rules

**No hyphens in text.** Do not use `-` inside body copy, headings, or labels. Rewrite the phrase instead.

**No orphaned words.** A single word must never sit alone on the last line. Apply `text-wrap: balance` for headings and `text-wrap: pretty` for body copy.

### Type scale

Always resolve font sizes to Tailwind's default type scale. Never leave arbitrary values in place, including `text-[19px]`, `font-size: 22px`, or `1.4rem`.

If an existing size does not land exactly on a step, snap it to the **closest step below**, taking both the size and its paired line height.

| Class | Size | Line height |
|---|---|---|
| `text-xs` | 12px (0.75rem) | 16px |
| `text-sm` | 14px (0.875rem) | 20px |
| `text-base` | 16px (1rem) | 24px |
| `text-lg` | 18px (1.125rem) | 28px |
| `text-xl` | 20px (1.25rem) | 28px |
| `text-2xl` | 24px (1.5rem) | 32px |
| `text-3xl` | 30px (1.875rem) | 36px |
| `text-4xl` | 36px (2.25rem) | 40px |
| `text-5xl` | 48px (3rem) | 1 |
| `text-6xl` | 60px (3.75rem) | 1 |
| `text-7xl` | 72px (4.5rem) | 1 |
| `text-8xl` | 96px (6rem) | 1 |
| `text-9xl` | 128px (8rem) | 1 |

Do not combine scale snapping with independently set custom line heights elsewhere in an audit. Tracking and line height may only be adjusted **within** the value the matched step already provides, so the two rules never fight each other.

### Text styles

Every piece of text uses one of these named styles. Never style text with a loose size and weight. Use the names exactly as written, including capitalization.

| Style | Scale step | Size / line height | Weight |
|---|---|---|---|
| Heading 1 | `text-6xl` | 60 / 60 | Semibold |
| Heading 2 | `text-5xl` | 48 / 48 | Semibold |
| Heading 3 | `text-4xl` | 36 / 40 | Semibold |
| Heading 4 | `text-3xl` | 30 / 36 | Semibold |
| Heading 5 | `text-2xl` | 24 / 32 | Semibold |
| Heading 6 | `text-xl` | 20 / 28 | Semibold |
| Title 1 | `text-xl` | 20 / 28 | Medium |
| Title 2 | `text-lg` | 18 / 28 | Medium |
| Title 3 | `text-base` | 16 / 24 | Medium |
| Title 4 | `text-sm` | 14 / 20 | Medium |
| Title 5 | `text-xs` | 12 / 16 | Medium |
| Body 1 | `text-base` | 16 / 24 | Semibold |
| Body 2 | `text-base` | 16 / 24 | Medium |
| Body 3 | `text-base` | 16 / 24 | Regular |
| Body 4 | `text-sm` | 14 / 20 | Semibold |
| Body 5 | `text-sm` | 14 / 20 | Medium |
| Body 6 | `text-sm` | 14 / 20 | Regular |
| Button-lg | `text-lg` | 18 / 28 | Semibold |
| Button-md | `text-base` | 16 / 24 | Semibold |
| Button-sm | `text-sm` | 14 / 20 | Semibold |
| Button-Xsm | `text-xs` | 12 / 16 | Semibold |
| Caption 1 | `text-sm` | 14 / 20 | Medium |
| Caption 2 | `text-sm` | 14 / 20 | Regular |
| Caption 3 | `text-xs` | 12 / 16 | Semibold |
| Caption 4 | `text-xs` | 12 / 16 | Medium |
| Caption 5 | `text-xs` | 12 / 16 | Regular |

How the groups work:

- **Heading** for page and section headings, largest to smallest. Heading 1 is the hero.
- **Title** for card titles, list item titles, labels that lead a block, and nav items.
- **Body** for running text. Within each size, 1 is the strongest weight and the last is regular.
- **Button** for text inside buttons only. Main buttons use Button-md, small header buttons use Button-sm.
- **Caption** for metadata, helper text, badges, timestamps, and fine print.

The sizes come from the type scale above, so a style never introduces an off scale value. If a project needs a new style, add the next number in its group (for example Body 7) built from a scale step, rather than inventing a new name.

In code, define each style once as a reusable class or token with the same name in kebab case (`heading-1`, `body-4`, `button-md`, `caption-2`) and apply that, instead of repeating size and weight utilities on every element.

## B2. Spacing

Only these values. Nothing between them, nothing outside them.

| Token | Value |
|---|---|
| Spacing-0 | 0 |
| Spacing-25 | 2px |
| Spacing-50 | 4px |
| Spacing-75 | 8px |
| Spacing-100 | 12px |
| Spacing-200 | 16px |
| Spacing-300 | 24px |
| Spacing-400 | 32px |
| Spacing-500 | 40px |
| Spacing-600 | 48px |
| Spacing-700 | 64px |
| Spacing-800 | 80px |
| Spacing-900 | 96px |

**Main buttons:** 8px vertical padding, 12px horizontal padding.

## B3. Corner radius

Only use Tailwind's radius values.

**Nested radius formula.** When a shape sits inside another shape and the gap between them is **less than 32px**:

```
inner radius = outer radius − gap
```

Apply this only when the result is **greater than 2**. Below that, leave the inner shape square or unchanged.

Example: an outer card at `rounded-2xl` (16px) with 8px of internal padding gives an inner element an 8px radius (`rounded-lg`).

## B4. Borders and backgrounds

- **Never apply a border to only one side of a card.** Borders go all the way around or not at all.
- **Never use gradients in backgrounds.** Backgrounds are flat.

### Dark mode background colors

Use only these:

`#000000` · `#181818` · `#1F1F1F` · `#272727` · `#313131` · `#131209`

## B5. Hero section

### Heading color

- **Dark theme:** left to right gradient on the heading text, `#FFFFFF` → `#9B9B9B`.
- **Light theme:** left to right gradient on the heading text, `#000000` → `#666666`.

This is the one place gradients are used, and only on text, never on the background.

### Layout

- Heading and subheading both get a **max width of 680px**.
- Read the heading copy and insert line breaks at **meaningful** points.
- Never break a line in a way that cuts a phrase awkwardly or makes the sentence harder to read. Break where the thought breaks.

## B6. Icons

**Use:** Phosphor, Solar, or Iconamoon.

**Never use:** Material Icons, Material Symbols.

## B7. Motion

Motion should feel weighted and decelerate into place. Never ship a browser default curve (`ease`, `linear`, `ease-in-out`).

**Base curve:** `ease-[cubic-bezier(0.22,1,0.36,1)]` with `duration-500` for layout and position changes. Color and opacity shifts on hover may use `duration-300`, never shorter than 200ms.

Animate only `transform` and `opacity`. Never animate `top`, `left`, `width`, or `height`.

Respect `prefers-reduced-motion`: replace movement with a plain opacity change.

### Navigation

**Resting state.** A compact bar that floats off the top edge rather than sitting flush against it, centered and sized to its content. It uses a translucent surface over a background blur so page content stays faintly visible behind it. Spacing comes from B2, radius from B3.

**Menu toggle.** The open and close icon transforms between its two states instead of swapping instantly. Use an icon from B6 or draw the lines yourself; either way the change is animated with the base curve.

**Mobile menu.** Opens as a full height panel, not a small dropdown. The panel background uses the theme's base surface at high opacity with a strong blur.

**Link entrance.** Links inside the open menu arrive one after another in reading order, each moving up a short distance (Spacing-300, 24px) while fading in. Step each item 60ms after the previous one and cap the total sequence at 400ms so long menus never feel slow.

### Scroll reveals

Sections entering the viewport rise a short distance (Spacing-400, 32px) and fade from 0 to full opacity over 600 to 800ms on the base curve. Reveal each section once; do not replay on scroll back up.

Trigger reveals with `IntersectionObserver` or Framer Motion's `whileInView`. Never attach work to an unthrottled `window.addEventListener('scroll')`, since it runs on every frame and drags down mobile performance.

---

## B8. Content realism

Every piece of sample content should read like it came from a real product with real users.

- **Write the copy.** No placeholder Latin, no "Your headline here". Draft real sentences in the product's voice.
- **People.** Give testimonials and team members full, specific names that fit the product's audience and region. Never reuse one face for two people.
- **Brands and logos.** Invent names that sound like they belong in the product's industry. A logistics tool's customers sound like logistics companies, not generic tech startups.
- **Never invent facts.** On a real product's page, prices, guarantees, statistics, customer counts, testimonials, and logos must come from the user or a real source. When a fact is missing, use a clearly marked placeholder such as `{{price}}` or `{{testimonial}}` instead of making one up.
- **Sample numbers.** In fictional demos and prototypes (where the invented names and brands above are fine), avoid suspiciously round figures. Pricing should look like real pricing, metrics should carry a decimal or an odd final digit, and dates across a list should vary.
- **Banned filler words.** Do not write "revolutionize", "supercharge", "cutting edge", "effortless", "transform your workflow", "take it to the next level", "harness the power", or "world class". Say what the product does in plain terms instead.
- **Sentence case** for headings and buttons.
- **System messages.** Confirmations are calm and specific ("Invoice sent to Dana"). Errors say what failed and what to do next ("Upload failed. The file is over 20 MB."). No cute interjections, no exclamation marks.

## B9. States

Every interactive element ships with its full state set:

- **Hover** — background shift, slight scale, or translate
- **Active** — `scale(0.98)` or `translateY(1px)` for physical feedback
- **Focus** — a visible focus ring. Accessibility requirement, not optional.
- **Loading** — skeleton loaders shaped like the real layout, not circular spinners
- **Empty** — a composed "getting started" view, never a blank panel
- **Error** — inline and specific. Never `window.alert()`.

No dead links. A button pointing at `#` is either linked or visually disabled. The current page must be indicated in the navigation.

## B10. Ship requirements

Things that get forgotten and make a page feel unfinished:

- Privacy policy and terms links in the footer
- A custom, branded 404
- Client side form validation for email format and required fields
- A skip to content link for keyboard users
- Cookie consent where the jurisdiction requires it
- A branded favicon
- `<title>`, meta description, `og:image`, and social sharing tags
- Alt text on every meaningful image
- Semantic HTML: `<nav>`, `<main>`, `<article>`, `<aside>`, `<section>`
- A way back from every page
- A check at 390px wide: no horizontal overflow, buttons keep their text inside, and the primary action is visible in the first screen

## B11. Tagline reveal section (mandatory)

Every landing page includes one large type section stating the core benefit or tagline, separate from the hero. It sits further down the page as its own moment, not stacked directly under the hero.

**Copy**
- Minimum two lines of text.
- A benefit statement or tagline, written in the voice of A5, not a generic section heading.

**Typography**
- Use Heading 3 to Heading 1 from the B1 text styles, depending on line count.
- Max width capped like the hero, so lines break at meaningful points per B5.

**Animation**
- Text starts in a subtle, muted tone, roughly 25 to 35% opacity of the theme's base text color.
- As the section scrolls into view, each word transitions individually from that muted tone to the full text color, in reading order.
- Words activate one at a time as they cross a trigger line, not the entire block flipping at once. The transition uses the base curve from B7, never a linear fade.
- Implement with `IntersectionObserver` per word, or a single scroll listener throttled through `requestAnimationFrame`. Never an unthrottled `window.addEventListener('scroll')`, per B7.
- Under `prefers-reduced-motion`, show the final text at full color right away, with no word by word animation.

---

# PART C — Overlays, players, and interactive media

Part B (or the active Part D aesthetic) still decides every font, spacing value, radius, color, icon, and curve. Part C only adds what changes when the output is composited into a live broadcast or is a media surface people operate.

**Write overlays against tokens, never literal values.** Every color, font, radius, stroke, shadow, and motion value in overlay CSS comes from a variable in the D2 token contract. This is what lets the whole overlay change aesthetic by swapping one theme, and it is not optional.

## C0. Overrides to Part B

These Part B rules behave differently on a broadcast overlay. Everything not listed here applies unchanged.

| Part B rule | On a broadcast overlay |
|---|---|
| B1 type scale | Same scale and names, but with a legibility floor. See C3. |
| B4 dark backgrounds | The page background is fully transparent. Surface colors are used for **plates** (the solid panels that sit behind text), never for the full canvas, except in full screen scenes (C2). In the Base aesthetic the surfaces are the B4 colors; other aesthetics set their own (D5). |
| B7 translucent blur | `backdrop-filter` cannot blur the game or camera behind a browser source, because it only sees its own page. Use a solid plate at 90 to 100% opacity instead of glass. The glass aesthetic (D5) shows how to fake it legibly. |
| B7 reduced motion | OBS has no user preference, so `prefers-reduced-motion` never fires there. Keep the media query for web viewing, and expose a `?motion=reduced` URL parameter for streamers who want calmer overlays. |
| B9 hover, active, focus | Do not exist on a broadcast output. They apply in full to control docks (C10) and to players or widgets people click (C7, C9). |
| B9 empty, loading, error | Never shown to viewers. See C11. |
| B10 ship requirements | Replaced by C12 for overlays. Landing pages keep B10. |
| B11 tagline reveal | Landing pages only. Never on an overlay. |

## C1. Overlay intake

Ask in one batch, only for what is missing. Assume and state a default in one line when the user cannot answer.

**Broadcast**
- Platform: Twitch, YouTube, Kick, TikTok Live, or several at once
- Canvas: 1920×1080 landscape (default), 2560×1440, or 1080×1920 vertical. Ask whether they stream both landscape and vertical at once (for example with a dual output plugin); if so, each canvas gets its own layout files that share one theme.
- Software: OBS Studio (default), Streamlabs, vMix, or a web app that renders the scene itself
- Content type: gameplay, just chatting, creative, music, talk show, event

**Scenes needed** (default set: Starting soon, Live, BRB, Ending, plus a stinger transition if they want one)

**Sources already available**
- Camera: one or more, aspect ratio, framed or cut out (green screen or background removal), guests joining remotely
- Game or screen capture: which game, and where its HUD sits (minimap, health, killfeed)
- Chat: native platform chat, a provider widget (StreamElements, Streamlabs), or a custom widget built here; one platform or merged from several
- Alerts provider, or events wired directly (Twitch EventSub, YouTube Live API)

**Look**: an aesthetic by name or mood (D4), a reference image, or the game or genre to evoke. If nothing is given, use Base and say so in one line.

**Brand**: logo, brand colors, the channel name, social handles, schedule

If the game's HUD layout is unknown, ask for one screenshot of gameplay. Overlays that cover the minimap or health bar are the most common failure in this category.

## C2. Canvas, scenes, and safe areas

**Fixed canvas.** Build every overlay at the exact canvas size in CSS pixels (`width: 1920px; height: 1080px`), with `overflow: hidden` and no scrollbars. Do not make broadcast overlays responsive; OBS scales the output. Use absolute positions in pixels so the user can match sources in OBS exactly.

**Transparent page.** `html, body { background: transparent; margin: 0; }`. Never leave a white default, and never ship a background color "for preview". For previewing, add a `?preview=1` parameter that draws a sample gameplay frame behind the overlay.

**Safe area.** Keep every persistent element (camera frame, chat, labels, goals) inside a margin of Spacing-900 (96px) left and right, Spacing-600 (48px) top and bottom on a 1080p canvas. Platform players briefly cover the bottom edge with controls, and TVs crop the edges.

**Vertical canvas (1080×1920).** Mobile apps cover the right side with action buttons and the bottom with the caption and comment area. Keep critical content out of roughly the right 160px, the bottom 480px, and the top 160px, and check the platform's current safe zone template before shipping.

**Layout around the content, not on top of it.** In a gameplay scene, the game owns the center and its HUD corners. The camera and chat take the corners and edges the HUD leaves free. Never place a persistent element over the area the streamer points at.

**Scene types**

| Scene | Background | Purpose | Required elements |
|---|---|---|---|
| Starting soon | `--surface-scene` | Hold early viewers | Countdown (C9), schedule or topic of the stream, chat visible |
| Live, gameplay | Transparent | Frame the game | Camera frame, chat or recent events, optional goal |
| Live, just chatting | Transparent or `--surface-scene` | Frame the camera | Large camera frame, chat, topic label |
| BRB | `--surface-scene` | Keep viewers through a pause | Short message, chat, optional video loop (C7) |
| Ending | `--surface-scene` | Send viewers somewhere | Next stream time, raid target or socials |

Every scene shares one set of tokens (`tokens.css` plus the active theme) so switching scenes never changes the type, spacing, or palette.

**Layer stack.** Plan the OBS source order from bottom to top, and state it in the handoff:

1. Scene background (full screen scenes only)
2. Game or screen capture
3. Under layer: plates and decoration that should sit **behind** a cut out streamer
4. Camera source
5. Over layer: camera frame, chat, alerts, goals

A framed camera needs only layer 5. A cut out camera (green screen or background removal) has no frame: put its name tag and any panel it overlaps in layer 3 so the streamer appears in front of them.

**Stinger transitions.** A stinger is a short video with transparency that covers the screen while OBS switches scenes.
- Length 0.8 to 1.5 seconds. The **transition point** (the moment OBS cuts) is the frame where the cover is complete; state it in milliseconds in the handoff.
- Built from the active theme's surfaces, accent, and motion personality, so it reads as part of the same package.
- Covering shapes move with `transform` only. Nothing smaller than the C3 text floor; a stinger is gone before anyone reads it, so it carries at most the logo or the channel name.
- To render one from HTML: drive the animation with the Web Animations API, pause it, step `currentTime` frame by frame, and capture each frame with a headless browser using a transparent background (`omitBackground: true` in Playwright). Encode with `ffmpeg -framerate 60 -i frame_%04d.png -c:v libvpx-vp9 -pix_fmt yuva420p -b:v 0 -crf 20 stinger.webm` to keep the alpha channel.

## C3. Broadcast legibility

The stream is compressed and often watched on a phone at one third of the canvas size. Detail that looks crisp in a browser turns into noise on the stream.

**Text floor on a 1080p canvas.** Nothing below 18px. Use these overlay styles, which follow the B1 naming rule by adding the next number in each group:

| Style | Scale step | Size / line height | Weight | Use |
|---|---|---|---|---|
| Caption 6 | `text-lg` | 18 / 28 | Medium | Timestamps, badges, secondary labels. The minimum. |
| Body 7 | `text-xl` | 20 / 28 | Medium | Chat messages |
| Body 8 | `text-2xl` | 24 / 32 | Medium | Anything a viewer must read at a glance: goal labels, now playing, topic |
| Title 6 | `text-2xl` | 24 / 32 | Semibold | Usernames in alerts, camera name tag |

Headings keep their B1 styles. On a vertical canvas, use the same sizes as 1080p, since the width is the same.

**Higher resolution canvases.** Always author in 1920×1080 logical pixels. For a 2560×1440 canvas, set the browser source itself to 2560×1440 and pass `?scale=1.3333`, which applies `zoom` to the root wrapper so text renders sharp at native resolution. Never author a 1080p source and stretch it in OBS; the upscale blurs every edge before compression makes it worse. This keeps every size on the B1 scale at every resolution.

**Contrast.** Text sits on a plate, never bare over gameplay or camera, because the content behind it changes every frame. Body text on a plate must reach at least 7:1 contrast, muted text and usernames at least 4.5:1. Never signal an event type by color alone; pair the color with an icon or a word.

**Compression safe detail**
- Strokes and borders are at least 2px. A 1px line flickers and disappears at low bitrates.
- No fine noise, grain, or subtle textures. They eat bitrate and turn into blocks.
- Shadows are short and dense, not wide and soft. A wide blur bands badly.
- Keep large areas still. Constant motion over a big area lowers the quality of the whole stream.

## C4. Plates and surfaces

A **plate** is the solid panel behind any overlay text: chat, labels, goals, alerts.

- Fill: `--surface-plate`, at 90 to 100% opacity. Only the glass aesthetic goes lower, to 80% at the least (D5).
- Radius: `--radius-plate`, a Tailwind radius. Everything inside a plate uses `--radius-inner`, which applies the nested radius formula.
- Shape: `--plate-clip` when the aesthetic has chamfered or cut corners. A `clip-path` also clips borders and shadows, so a clipped plate draws its stroke with a second clipped layer behind it, one `--stroke-width` larger.
- Padding: Spacing-200 (16px) minimum, Spacing-300 (24px) for plates with a heading.
- Border: `--stroke-width` (2 to 4px) in `--stroke`, all the way around (B4), never on one side. Dividers between rows inside a plate are allowed.
- One accent color per overlay (`--accent`), taken from the brand when there is one. Use it for one thing (the active progress fill, the alert highlight, the live dot), not for every plate. Only aesthetics that define `--accent-2` may use a second one.

## C5. Camera frame

**The camera is not drawn by the HTML.** In OBS, the webcam is a native video capture source. The overlay draws only the frame around it. The overlay source sits above the camera source in the OBS source list, and the frame's hole lines up with the camera.

**Define the hole in pixels.** Every camera frame ships with its hole stated as `x, y, width, height` in canvas pixels, plus the aspect ratio (16:9, 4:3, or 1:1), so the user can position the camera with Edit Transform. Print these values in a comment at the top of the file and in the handoff (C12).

**Rounded camera corners without a mask.** Draw the frame as an opaque ring whose transparent hole is slightly smaller than the camera source. Position the camera so it extends at least Spacing-50 (4px) under the ring on every side. The ring then covers the camera's square corners. The hole's radius follows the B3 formula: outer radius − ring width, when the ring is narrower than 32px.

```css
/* Hole: x=96 y=600 w=480 h=270 (16:9). Place the camera at x=92 y=596 w=488 h=278. */
.cam-frame {
  position: absolute; left: 84px; top: 588px; width: 504px; height: 294px;
  box-sizing: border-box;                    /* the size includes the ring */
  border: 12px solid var(--surface-plate-solid); /* ring width, B2 Spacing-100 */
  border-radius: 24px;                       /* outer, rounded-3xl */
  /* inner hole radius = 24 − 12 = 12px, drawn automatically by the border */
}
```

**The ring must be opaque where it hides corners.** The trick only works if the camera's square corners are covered by a fully opaque ring. A translucent, glowing, or outline only frame shows those corners. In that case, round the camera itself with an alpha mask PNG (exact hole size and radius) applied through OBS's Image Mask/Blend filter on the camera source, then draw the decorative frame on top. Use the same mask when the camera must have no visible ring at all.

**Any other frame shape** (chamfered, notched pixel corners, a sticker outline, a hexagon): draw the ring as one inline SVG path with `fill-rule="evenodd"`, made of the outer shape followed by the hole shape. The hole is then exactly transparent, the ring is solid, and the shape scales without blur. Decorations (corner brackets, stickers, the live dot) sit outside the hole.

**Name tag.** Optional, Title 6 on a plate, attached to the bottom or top edge of the frame. Never overlapping the face area (the top two thirds of the hole).

**Several cameras or remote guests.** Give every hole the same size and aspect ratio, separate them with one B2 gap (Spacing-300 or Spacing-400), and give each its own name tag. Plan the layouts for one, two, three, and four people up front, so adding a guest is a scene switch and not a redesign. A guest joining over a browser link is just another source placed in its hole.

**Camera in a web app (getUserMedia).** When the camera is rendered in the browser instead of OBS:
- Request access only after a user action, with a short line explaining why.
- Design the states: asking for permission, permission denied (with how to reenable it), no camera found, camera in use by another app, and live.
- Mirror the self view with `transform: scaleX(-1)` for the person looking at themselves. Never mirror what gets recorded or sent to others.
- Use `object-fit: cover` inside the rounded container, and stop every track when the view unmounts so the camera light turns off.
- Do not use getUserMedia inside an OBS browser source to show a webcam. Camera access there depends on launch flags and conflicts with the native source.

## C6. Chat widget

**Layout.** Newest message at the bottom, older messages move up. Cap the visible list (8 to 12 messages, or by height) and **remove** DOM nodes past the cap, so a six hour stream does not leak memory. Optionally fade out messages after 30 to 60 seconds so the area clears when chat is quiet.

**Each message**
- Badges (moderator, subscriber) as images at the line height, before the name
- Username in Body 7 Semibold or Title 6, message in Body 7
- Emotes as images sized to the line height (28px for Body 7), with the emote name as `alt`
- `overflow-wrap: anywhere`, so a long link or a word spam cannot break the layout
- When chat is merged from several platforms, a small platform icon before the badges, so viewers know where a message came from

**Username colors.** Platforms let users pick any color, so many are unreadable on the plate. Keep the user's hue but move its lightness toward whichever side gives contrast (lighter on dark plates, darker on light plates) until it reaches at least 4.5:1. This matters most when switching aesthetics: the same chat on a light cozy plate needs the opposite correction.

**Emote parsing.** Twitch reports emote positions as Unicode code point offsets, not JavaScript string indexes. Convert the message with `Array.from(text)` before slicing, or every emoji before an emote shifts the emote out of place. Streamers usually also expect third party emote sets (7TV, BTTV, FFZ), which have public APIs per channel; load them once at start and refresh them periodically, not per message.

**Entrance.** A new message fades in and rises with the theme entrance (`.enter`, D2; Base rises Spacing-200, 16px). The messages above it move up with a FLIP transform (measure, then animate `transform`), never by animating `height`, per B7.

**Moderation.** Remove a message from the overlay as soon as it is deleted on the platform, and clear all messages from a user on a timeout or ban. Hide messages from known bots and commands (lines starting with `!`) by default, with a URL parameter to show them.

**Security.** Chat text is untrusted. Insert it with `textContent` or a framework's escaped text binding, never `innerHTML`, and build emotes as image nodes from the platform's emote data, not by replacing text with HTML strings. A browser source runs with network access on the streamer's machine.

**Data**
- Twitch: an anonymous IRC connection (for example `tmi.js` with no token) reads public chat without credentials.
- YouTube: the Live Chat API needs an API key or OAuth and has quota limits. Poll at the interval the API returns, not faster.
- Platforms without a public chat API for overlays: use the provider widget or the platform's own studio tool. Never scrape the platform's pages.
- Provider widgets: if the user already uses StreamElements or Streamlabs chat, style it with that provider's custom CSS rather than rebuilding it.
- Always ship a demo mode (`?demo=1`) that generates realistic messages (B8), with long names, emotes, and long links, so the design can be checked without going live.

## C7. Video player

Two different products share this section. Decide which one is being built.

### Broadcast video (no controls)

For BRB loops, intro clips, and replays inside an overlay.
- Long or full screen video plays better as an OBS Media Source than inside a browser source, because OBS can decode it more efficiently. Use a `<video>` in the overlay only when the clip is small or its timing is tied to overlay logic (an alert, a goal celebration).
- `<video autoplay muted loop playsinline>` for silent loops. Unmute only when the clip is meant to be heard; in OBS, enable "Control audio via OBS" on the browser source so the streamer can mix it.
- For video with transparency, use WebM with VP9 alpha. OBS's browser renders it.
- Preload the file before the scene becomes active, and start from a poster frame so the first frame is never black.
- When a clip ends without looping, fade the element out with `--dur-exit` and `--ease-exit` and remove it.

### Interactive player (landing pages, web apps)

**Controls, in this order:** play/pause, current time / duration, scrubber, volume and mute, captions, playback speed (optional), picture in picture (optional), fullscreen. Icons from B6. Every control is a real `<button>` with an accessible label that changes with its state ("Play" becomes "Pause").

**Scrubber.** Shows played, buffered, and remaining ranges. Draggable with the pointer, operable with arrow keys (5 second steps), and shows the target time while dragging. Render the filled range with `transform: scaleX()`, not `width`.

**Keyboard** when the player has focus: Space or K play/pause, J and L back and forward 10s, left and right arrows 5s, up and down volume, M mute, C captions, F fullscreen. Never take these keys while focus is in a text input elsewhere on the page.

**Autohide.** While playing, controls fade out after 2.5 seconds without pointer movement and come back on pointer move, touch, or focus. Never hide them while paused, while a menu is open, or while any control has keyboard focus.

**States**
- Before play: poster frame with one large play button, and the duration visible
- Buffering: the buffered range on the scrubber plus a slim indeterminate bar along the bottom edge, not a centered spinner (B9)
- Ended: a replay button and, on landing pages, the primary CTA from A2
- Error: what failed and what to do ("This video could not load. Check your connection and try again.") with a retry button

**Landing page rules**
- Autoplaying hero video is always `muted`, `playsinline`, and has a visible pause control (WCAG 2.2.2).
- Under `prefers-reduced-motion`, do not autoplay. Show the poster and the play button.
- Captions via `<track kind="captions">` on any video with speech. Never burn the only captions into the video.
- `preload="metadata"` for videos below the fold, and lazy load the element itself.
- Embeds (YouTube, Vimeo) load behind a facade: a poster image with a play button that swaps in the iframe on click.

## C8. Alerts

Alerts cover follows, subscriptions, gifts, cheers and donations, raids, and members.

**Queue, never overlap.** Events go into a queue and play one at a time. Larger events (raids, large gifts) jump ahead of follows. When many follows arrive at once (a raid or a follow bot), merge them into one alert ("24 new followers") instead of playing 24.

**Duration.** 4 to 8 seconds, scaled to the event size. The entrance and exit use the theme curves (`--ease-enter`, `--ease-exit`); the exit is shorter than the entrance.

**Content.** One line that names the person and the event in Title 6 or Heading 5, plus at most one detail line in Body 8 (the amount, the months subscribed, the message). Donation and sub messages are untrusted text (C6 security) and must pass the platform's or provider's profanity filter before display.

**Placement.** Top center or near the camera, inside the safe area, never over the game's center. Same position for every event type, so viewers learn where to look.

**Sound.** Optional, short, normalized so every alert sound is at the same loudness and sits below the streamer's voice in the mix. Route it through OBS like any other browser audio. Text to speech for donation messages is opt in, runs only after the profanity filter, and is capped in length.

**Per aesthetic.** The alert's shape, entrance, and ornament come from the active theme (D5). Its queue, timing, placement, and filtering never change with the look.

**Test panel.** Ship a way to fire each alert type by hand (in the control dock or with `?demo=1`) so the streamer can check every alert before going live.

## C9. Interactions and live widgets

**Goals and progress bars.** Label (Body 8), current and target value, and a fill rendered with `transform: scaleX()` from the left (`transform-origin: left`). When the value changes, animate the fill with `--ease-enter` over 700ms and count the number up over the same time. When the goal completes, play one short celebration and then show the next goal; do not leave a full bar for hours.

**Countdown timers.** Store the target timestamp and compute the remaining time from `Date.now()` on every frame or second. Never decrement a counter with `setInterval`, which drifts and pauses in hidden tabs. Show `mm:ss` in `--font-mono` or with `font-variant-numeric: tabular-nums` so the digits do not jump. At zero, replace the timer with a line ("Starting now"), never with negative time.

**Polls and predictions.** Options as rows, each with a bar (scaleX) and a percentage. Reorder rows with a FLIP transform when the ranking changes. Show the time left and the total votes.

**Now playing, tickers, and rotating info.** Rotate between at most three messages, each held for at least 8 seconds. A ticker scrolls with a CSS `translateX` animation at a speed a phone viewer can read (about 60px per second at 1080p), never with JavaScript on every frame.

**Chat triggered effects.** Commands or channel point redemptions that trigger an overlay effect go through the same queue as alerts, with a per user cooldown and a global rate limit, so viewers cannot spam the screen.

**Idle motion.** Loops that run all stream long (a live dot, a slow glow on a logo) are allowed only if they are slow (one cycle per 4 seconds or longer), small in area, and far from the camera. Never loop motion next to the streamer's face.

**Flashing.** Nothing on the overlay flashes more than three times in any one second (WCAG 2.3.1), in any aesthetic. Flicker effects (neon, glitch) last a fraction of a second and only on entrance.

**Interactive widgets on web pages** (an embedded poll, a live reaction bar, a demo of the overlay on a landing page) are normal UI: full B9 states, keyboard access, and `prefers-reduced-motion`.

## C10. Data, control, and configuration

**One HTML file per browser source.** `camera.html`, `chat.html`, `alerts.html`, `goal.html`, `starting-soon.html`, all importing the shared `tokens.css`, the theme files, and one script for the event bus. This lets the streamer show, hide, and position each piece in OBS.

```
overlay/
  tokens.css          D2 contract with Base values
  themes/             one file per aesthetic: esports.css, neon.css, ...
  fonts/              every font file the themes use, as woff2
  lib/                event bus, chat client, alert queue, theme loader
  camera.html  chat.html  alerts.html  goal.html  timer.html
  starting-soon.html  brb.html  ending.html
  dock.html           control dock (C10)
  server.js           tiny local server and relay (optional)
```

**Configuration in the URL.** Channel name, theme, demo mode, motion, scale, and which events to show come from query parameters (`chat.html?channel=name&theme=cozy&demo=1`), so one file serves every scene and every streamer. Every source of one stream uses the same `theme` value.

**Serve over localhost, not as local files.** OBS's "Local file" option loads pages from `file://`, where ES modules, `fetch` of local JSON, and same origin features fail. Serve the folder from a tiny local server (`http://localhost:PORT/chat.html`) so every source and the dock share one origin. If the user cannot run a server, ship classic scripts with no modules and no `fetch`.

**OBS runs its own Chromium**, often several versions behind current Chrome. Prefer widely supported CSS (custom properties, grid, transforms, `rgb()` with alpha) over the newest features (`color-mix()`, `@starting-style`, view transitions, container style queries) unless they are confirmed in the user's OBS version. Leave "Browser Source Hardware Acceleration" on in OBS's settings, or every animation costs CPU.

**Secrets.** OAuth tokens and API keys never live in the HTML, the repository, or a URL that could be shown on stream. Keep them in a local config file read by a small local server, or in the provider's own widget settings. Read only chat does not need a token at all.

**Control dock.** When the streamer needs to trigger things by hand (test alerts, start a timer, switch the goal, hide the camera), build a separate page loaded as an OBS custom browser dock. The dock is a normal interface: full B9 states, focus rings, keyboard access, and clear labels, styled with the same theme as the overlay. It talks to the overlays through a small local WebSocket relay (the default, it works whatever OBS does with docks), or through obs-websocket's `BroadcastCustomEvent` when the streamer already uses obs-websocket. Use `BroadcastChannel` only after confirming it reaches the browser sources in the user's setup, since docks and sources do not always share a browser profile. To switch scenes or toggle sources, use obs-websocket (v5) from the dock, never from a viewer facing overlay.

**Theme switching from the dock.** A theme picker in the dock sends `{ type: "theme", value: "neon" }` over the same channel, and every overlay swaps its `data-theme` attribute live. Wait for the new theme's fonts to load before swapping, so no frame shows a fallback font on stream.

**Reconnects.** Every live connection (chat, events, relay) reconnects on its own with exponential backoff (1s, 2s, 4s, capped at 30s) and resumes without reloading the page.

## C11. States on a broadcast

Viewers must never see the overlay's internals.

- **Loading or connecting:** render nothing (or the plate empty and at rest) until data arrives. No skeletons on a broadcast.
- **Empty:** an empty chat or event list collapses or stays hidden. Never "No messages yet". This overrides the B9 empty rule.
- **Error or disconnected:** stay visually calm, keep the last good state on screen, log to the console, and report it in the control dock (C10). Never print an error on the stream.
- **Font loading:** bundle the active theme's font files locally with `font-display: block`, and load them through the theme loader (D2) before the first entrance animation, so text never flashes in a fallback font when a scene goes live.

## C12. Overlay ship requirements

- A source map in the handoff: for each browser source, its file and URL parameters, `x, y, width, height`, FPS (30 or 60, matching the stream), and the OBS options to set
- "Shutdown source when not visible" off for chat and alerts (so history and the queue survive scene changes), and "Refresh browser when scene becomes active" on for timers and intros
- The camera hole's exact position and the camera source's position (C5)
- `?preview=1` and `?demo=1` both working, with realistic demo data (B8)
- Checked over a bright gameplay frame and a dark one, and at 33% scale to simulate a phone viewer
- A one hour soak test in demo mode with no growth in memory or DOM node count
- No layout jump when the longest realistic username, amount, or message appears
- Every animation uses `transform` and `opacity` only, on the active theme's curves (B7, D2)
- No overlay element inside the game's HUD areas or over the camera's face area
- The OBS source order (C2 layer stack) and, for stingers, the transition point in milliseconds
- Every shipped theme checked against D7, and `?theme=` switching tested on every source
- Debugged inside OBS itself, not only in Chrome: start OBS with `--remote-debugging-port=9222` and open `http://localhost:9222` in Chrome to inspect each browser source, and use the source's Interact window to test anything clickable

## C13. Stream package assets

A stream package usually ships static graphics alongside the overlays. Build them from the same tokens and theme so the channel page matches the stream, render them from HTML at exact sizes, and export PNG. Platform sizes change, so confirm against the platform's current guidelines before export.

| Asset | Typical size | Notes |
|---|---|---|
| Offline screen | 1920×1080 | Next stream time and socials, same layout as the Ending scene |
| Twitch profile banner | 1200×480 | Keep text centered; the edges are cropped on small screens |
| Twitch panels | 320px wide | One style for all panels, title in Heading 6, height consistent across the set |
| YouTube channel banner | 2560×1440 | All text and logos inside the centered 1546×423 safe area |
| Emotes | 112×112, also checked at 28×28 | Must read at 28px: thick shapes, no text, no thin lines |
| Sub badges | 72×72, also checked at 18×18 | One simple silhouette per tier, distinguished by more than color |

Emotes and badges are illustrations, not UI: B1 and B2 do not apply to their insides, but the palette and shape language of the active theme do.

---

# PART D — Aesthetic layer

A stream lives on its look, and streamers change looks: a seasonal event, a new game, a subathon, a rebrand. This part lets the same overlay (or landing page) switch aesthetic on request without rebuilding it, while everything that makes it legible, fast, and safe stays fixed.

**Base is the default.** With no look requested, the Base aesthetic is active, and it is Part B exactly. An aesthetic is only applied when the user names one, describes a mood, gives a reference, or asks to change the style. That request is the user's explicit prompt, so the variable rules below may change; the invariants may not.

## D1. What an aesthetic can and cannot change

**Never changes, in any aesthetic**
- The B2 spacing scale and the B1 type scale steps and named styles
- Contrast minimums: on overlays the C3 floor and ratios; on web pages WCAG AA (4.5:1 body text, 3:1 large text, control borders, and focus indicators)
- At most two families (`--font-display` and `--font-text`) plus `--font-mono`. B1's banned fonts stay banned, no italics, nothing heavier than bold (700)
- Chat, body, and caption text always use `--font-text`, which must be a highly legible face. Display fonts are only for Title 6 and larger (24px and up)
- On overlays: plates behind text, strokes of at least 2px, C2 safe areas, the HUD and face areas kept clear
- On web pages: B9 states with a visible focus ring, `prefers-reduced-motion`, the B10 ship requirements, and the 390px check
- Motion mechanics from B7: only `transform` and `opacity`, never a browser default curve, nothing flashing more than three times per second (C9)
- States (B9, C11), security (C6), configuration and data (C10), performance and ship checks (C12), content realism (B8)
- On landing pages: all of Part A, B5 layout, B10, and B11

**Changes with the aesthetic**

| Token group | What may vary |
|---|---|
| Type | Display and text families from the preset, or a vetted choice (D6); display weight; uppercase with letter spacing for short labels (three words or fewer, never for names or chat) |
| Color | Surfaces, text, muted text, stroke, one accent (two only where the preset says so). The B4 dark list binds Base only |
| Shape | Radius (still a Tailwind value), clipped corners, stroke width from 2 to 4px, shadow style |
| Gradients | Base bans them. A preset may allow them only where it says, and never as a smooth, low contrast gradient over a large area, which bands on stream. The B5 hero heading gradient becomes `--text` → `--text-muted` |
| Ornament | Brackets, stickers, pixel notches, rules, patterns, each optional and outside the camera hole |
| Motion | Enter and exit curves, durations (enter 250 to 800ms, exit shorter than enter), entrance direction and distance, stepped timing |
| Icons | Phosphor, Solar, or Iconamoon at a weight that suits the look (regular, bold, fill, duotone; never thin or light on overlays). The pixel preset may use Pixelarticons |
| Voice | Tone and casing of alert lines, scene messages, and labels. The B8 banned filler words still apply |

## D2. Token contract

Every theme sets the same variables. Structural CSS reads only these. A theme is a block scoped to `[data-theme="name"]`.

```css
/* tokens.css: the contract, filled with Base values */
:root, [data-theme="base"] {
  /* Type */
  --font-display: "Geist", system-ui, sans-serif;  /* Headings, Titles 24px and up */
  --font-text: "Geist", system-ui, sans-serif;     /* Body, chat, captions */
  --font-mono: "Geist Mono", ui-monospace, monospace;
  --display-weight: 600;
  --label-case: none;              /* none | uppercase */
  --label-tracking: 0em;           /* up to 0.08em, only with uppercase */

  /* Color */
  --surface-plate: rgb(24 24 24 / 0.94);  /* behind all overlay text */
  --surface-plate-solid: #181818;         /* opaque rings, stinger covers */
  --surface-raised: #272727;              /* elements inside a plate */
  --surface-scene: #000000;               /* full screen scenes */
  --text: #FFFFFF;
  --text-muted: #9B9B9B;
  --accent: #4F8CFF;                      /* replace with the brand color */
  --accent-2: var(--accent);
  --on-accent: #000000;
  --stroke: #313131;

  /* Shape */
  --stroke-width: 2px;
  --radius-plate: 16px;
  --plate-padding: 16px;
  --radius-inner: max(0px, calc(var(--radius-plate) - var(--plate-padding)));
  --plate-clip: none;
  --shadow-plate: none;

  /* Motion */
  --ease-enter: cubic-bezier(0.22, 1, 0.36, 1);
  --ease-exit: cubic-bezier(0.64, 0, 0.78, 0);
  --dur-enter: 500ms;
  --dur-exit: 300ms;
  --enter-x: 0px;
  --enter-y: 16px;
  --enter-scale: 1;
}

@keyframes enter {
  from { opacity: 0; transform: translate(var(--enter-x), var(--enter-y)) scale(var(--enter-scale)); }
  to   { opacity: 1; transform: none; }
}
.enter { animation: enter var(--dur-enter) var(--ease-enter) both; }
```

```js
// lib/theme.js: load the theme's fonts first, then swap, so no frame shows a fallback font
const FONTS = {
  base: ['600 24px "Geist"', '500 20px "Geist"'],
  esports: ['600 24px "Chakra Petch"', '500 20px "Geist"'],
  // one entry per theme, listing each family and weight it uses
};
export async function applyTheme(name) {
  const theme = name in FONTS ? name : "base";
  await Promise.all(FONTS[theme].map((f) => document.fonts.load(f)));
  document.documentElement.dataset.theme = theme;
}
applyTheme(new URLSearchParams(location.search).get("theme"));
```

Declare every theme's `@font-face` rules with local woff2 files. Browsers only download a face when it is used, so unused themes cost nothing.

## D3. Switching aesthetic on request

1. **Read the request.** Map named looks and mood words with D4. A reference image, game, or genre goes through D6.
2. **Write the aesthetic brief** before any code: the preset it starts from, then one line each for mood, type, color, shape, motion, and voice, plus every token that differs from the preset. State it and continue. Ask one question only when the request fits two presets that would look very different (for example "retro" as pixel arcade or as a 70s palette), with those two as the options.
3. **Change only the theme.** Write or edit the theme block. Never rewrite layout, data, or logic to change a look. If the look needs extra markup (corner brackets, stickers), add it once as optional elements that are hidden by default and shown by the theme, so every other theme stays untouched.
4. **Recheck the invariants** with the new values (D7).
5. **Hand off** with the preview URL (`?theme=name&preview=1&demo=1`) and a short list of the tokens that changed.

**Blending.** "Cozy but pixel", "esports with neon": start from one preset and take at most one token group (type, color, shape, or motion) from a second. More than that produces a look with no identity. Recheck contrast after every blend.

**Brand colors win** over a preset's accent, unless the user asks for the preset's colors. A brand accent that fails contrast on the plate becomes a fill (bars, dots, rings) with `--on-accent` text, never a text color.

**Seasonal or event variants** (a holiday, a subathon, a sponsor segment) are a theme that extends the current one and changes one or two groups, usually color and ornament. Switch back by switching the theme, nothing else.

## D4. Mood map

| Words in the request (any language) | Start from |
|---|---|
| minimal, clean, simple, modern, *minimalista, limpio* | `base` |
| competitive, esports, tactical, shooter, HUD, *gamer, competitivo, táctico* | `esports` |
| neon, cyberpunk, synthwave, futuristic, sci fi, *futurista* | `neon` |
| retro, arcade, 8 bit, 16 bit, pixel, *retro, pixelado* | `pixel` |
| cozy, cute, pastel, lofi, chill, soft, *acogedor, tierno, suave* | `cozy` |
| elegant, premium, editorial, luxury, music, podcast, *elegante, lujoso* | `editorial` |
| bold, loud, playful, meme, sticker, *llamativo, divertido* | `brutalist` |
| glass, frosted, sleek, translucent, *cristal, vidrio* | `glass` |

## D5. Presets

Each preset fills the D2 contract. The colors below were checked: body text reaches at least 7:1 on the plate and muted text at least 4.5:1. Brand colors replace `--accent` per D3. `base` is the D2 block itself. The presets are written for overlays first; E5 lists how each one adapts to a normal web page.

### `esports`: tactical HUD
- **Mood:** precise, fast, competitive
- **Type:** display Chakra Petch 600; text Geist; scores and timers in Geist Mono. Labels uppercase, tracking 0.06em
- **Color:** plate `#0E1318`, raised `#18212A`, scene `#070A0D`, text `#F2F5F7`, muted `#8C99A6`, stroke `#24313D`, accent `#00E5A0` with `#04130D` on it
- **Shape:** radius 0, chamfered corners through `--plate-clip: polygon(12px 0, 100% 0, 100% calc(100% - 12px), calc(100% - 12px) 100%, 0 100%, 0 12px)`, 2px stroke
- **Ornament:** corner brackets on the camera and on one key plate; a 4px accent bar as the single accent use
- **Motion:** enter 320ms `cubic-bezier(0.16, 1, 0.3, 1)` from `--enter-x: -24px`, exit 200ms. Alerts may wipe in with a cover element scaling on X
- **Voice:** short and numeric ("NEW FOLLOWER" label, then the name in its own case; "Raid · 48 viewers")
- **Camera:** chamfered ring as an SVG evenodd path (C5), brackets outside it

### `neon`: synthwave and cyber
- **Mood:** nocturnal, electric, futuristic
- **Type:** display Orbitron 600, only at Heading 5 (24px) and larger; text Geist
- **Color:** plate `#120E24`, raised `#1D1738`, scene `#07060F`, text `#F5F3FF`, muted `#A89FD0`, accent `#FF4FD8`, accent 2 `#3BE8FF` (strokes in one, highlights in the other), `#120E24` on either
- **Shape:** radius 8px; stroke is the accent with a tight glow, `box-shadow: 0 0 0 2px var(--accent), 0 0 8px var(--accent)`. The solid 2px line carries the shape when compression eats the glow. Glow blur never exceeds 8px; headings may take `text-shadow: 0 0 6px` in the accent
- **Gradients:** allowed only in full screen scenes, as a horizon with at least three clearly different color stops, and never behind live text
- **Ornament:** a static perspective grid with 2px lines in full screen scenes. Not animated: a moving grid is large area motion (C3)
- **Motion:** entrance flickers opacity three times in the first 150ms with `steps(3)`, then settles on the Base curve over 400ms. Never a continuous flicker
- **Voice:** terse with a light sci fi tone ("Signal from Maya: new follow")
- **Camera:** opaque ring in `--surface-plate-solid` with the glowing stroke on its outer edge, so the corner trick still works

### `pixel`: retro arcade
- **Mood:** nostalgic, playful, crunchy
- **Type:** display Press Start 2P, only at 24px, 48px, or 96px (`text-2xl`, `text-5xl`, `text-8xl`), which are multiples of its 8px grid and stay crisp. Text Geist Mono (or Pixelify Sans when the user wants a full pixel look), never smaller than Body 7
- **Color:** a limited six color palette is the look. Plate `#16162A`, raised `#25253F`, scene `#0B0B16`, text `#F4F4F4`, muted `#A3A3BD`, accent `#FFD23F`, accent 2 `#4FD1E0`, `#16162A` on either. Use no other colors
- **Shape:** radius 0. Notched corners drawn with offset shadows in place of a border: `box-shadow: 0 -4px 0 var(--stroke), 0 4px 0 var(--stroke), -4px 0 0 var(--stroke), 4px 0 0 var(--stroke)` with `--stroke: #F4F4F4`. Every size and position is a multiple of 4px; skip Spacing-25
- **Sprites:** `image-rendering: pixelated`, scaled only by whole numbers (2×, 3×, 4×)
- **Motion:** `steps(4, end)` over 400ms for entrances, distances in multiples of 4px; a bounce is a stepped `translateY`. `?motion=reduced` falls back to a plain opacity step
- **Voice:** arcade system lines in uppercase for labels only ("PLAYER JOINED" above the name). Invent lines; never quote a real game
- **Camera:** notched ring as an SVG evenodd path whose corners step in 4px blocks

### `cozy`: pastel and lofi
- **Mood:** warm, handmade, calm
- **Type:** Nunito for display and text (one family), weights from B1
- **Color:** light plates. Plate `#FFF7EE`, raised `#FBE9D7`, scene `#F3DFCB`, text `#3A2B26`, muted `#7A5E54`, stroke `#5A4038`, accent `#B4462F` with `#FFFFFF` on it. Username colors are clamped darker (C6)
- **Shape:** radius 24px on plates, full pills for tags and badges, 3px stroke, a solid drop shadow `0 4px 0 #5A4038` that makes plates read like stickers over any game
- **Ornament:** small static SVG doodles (stars, leaves, a steaming cup), each under 64px, at plate corners, never near the face
- **Motion:** enter 500ms with a gentle overshoot `cubic-bezier(0.34, 1.56, 0.64, 1)`, `--enter-scale: 0.96`, rise 16px. One sticker may bob on a cycle of 6 seconds or longer
- **Voice:** warm and personal, sentence case ("Thanks for the follow, Maya")
- **Camera:** thick rounded ring in the plate color with the 3px stroke on the outside and one doodle on the frame edge

### `editorial`: magazine and premium
- **Mood:** quiet, confident, expensive
- **Type:** display Instrument Serif 400 (`--display-weight: 400`), only at Heading 4 (30px) and larger, never italic; text Geist; labels uppercase at Caption 6 with tracking 0.08em
- **Color:** plate `#181818`, raised `#272727`, scene `#131209`, text `#F4F1EA`, muted `#A8A296`, stroke `#313131`, accent `#D2B27A` with `#181818` on it
- **Shape:** radius 0 or 4px (pick one), 2px strokes, dividers between rows instead of extra boxes
- **Motion:** slow and mostly opacity: enter 700ms on the Base curve, rise 8px, exit 400ms
- **Voice:** understated ("Maya, now following"). No uppercase except the small labels
- **Camera:** square hole (radius 0, so no corner trick needed) with a 2px stroke and a caption line underneath like a photo credit

### `brutalist`: loud and flat
- **Mood:** bold, funny, unpolished on purpose
- **Type:** Space Grotesk, 700 for display and 500 for text
- **Color:** bright flat plates. Plate `#FFE14D`, raised `#FFFFFF`, scene `#F4F0E6`, text `#111111`, muted `#3D3A2E`, stroke `#111111`, accent `#FF4F7B` used only as a fill with `#111111` text on it, never as a text color
- **Shape:** radius 0 or 8px (pick one), 3px black stroke, hard offset shadow 6px 6px 0 `#111111` drawn by a separate layer behind the plate
- **Motion:** 250ms `cubic-bezier(0.2, 0.8, 0.2, 1)`. Entrance "presses" the plate down: the plate moves from (−6px, −6px) to rest while its shadow layer stays still, so only `transform` animates
- **Voice:** blunt and a little funny but still specific ("Maya followed. Good call.")
- **Camera:** thick black ring with the same offset shadow

### `glass`: frosted and sleek
- **Mood:** light, modern, premium tech
- **Type:** Manrope
- **Color:** plate `rgb(31 31 31 / 0.8)` at the least, which keeps white text above 7:1 even over a white game frame; raised `rgb(255 255 255 / 0.06)`, scene `#181818`, text `#FFFFFF`, muted `#A6A6A6`, accent `#7CC4FF` with `#0B1A26` on it
- **Shape:** radius 24px, 2px stroke `rgb(255 255 255 / 0.14)`, inner highlight `inset 0 2px 0 rgb(255 255 255 / 0.08)`
- **Blur:** over gameplay the glass is faked by the plate above (C0). Real `backdrop-filter` is allowed only in full screen scenes, where the background is drawn inside the same page, and only on plates, never across the whole screen
- **Motion:** Base
- **Camera:** the ring is translucent, so round the camera with an OBS image mask (C5) and draw the glass ring on top

## D6. Custom aesthetics from a reference

When the user gives an image, a game, a film mood, a brand, or a look no preset covers:

1. **Extract** five or six colors from the reference, then adjust lightness until text and muted text pass on the plate. Note the shape language (angles or curves, line weight, corner treatment), the type feel (geometric, condensed, serif, rounded, pixel), and the motion feel (snappy, floaty, mechanical).
2. **Choose fonts** that match the feel, are licensed for streaming and embedding (SIL Open Font License faces are safe), have the weights B1 needs, and are not on B1's banned list. Bundle them locally.
3. **Name the theme** after the look, not the source (`ember`, not the game's title), write it as a full D2 block, and add its fonts to the theme loader.
4. **Evoke, never copy.** Do not reproduce a game's or brand's logos, proprietary fonts, UI assets, character art, or another creator's overlay design. Take the genre's palette, shape, and rhythm, and build original shapes.

## D7. Aesthetic checks

Run these every time a theme is created or changed:

- [ ] Body text 7:1 and muted text 4.5:1 on `--surface-plate`, measured on the solid color and, for translucent plates, over a white frame
- [ ] `--on-accent` reaches 4.5:1 on `--accent`; an accent that fails as text is used only as a fill
- [ ] Display font only at 24px and larger; chat and body in `--font-text` at the C3 floor
- [ ] No banned fonts, no italics, no weight above 700, at most two families plus mono
- [ ] Strokes 2px or thicker; glow blur 8px or less; no smooth gradient across a large area
- [ ] Camera ring opaque where it hides corners, or a mask is specified
- [ ] Every animation still uses only `transform` and `opacity`; no flashing above three per second
- [ ] All fonts for the theme are local and listed in the theme loader
- [ ] Checked over a bright and a dark gameplay frame at 33% scale
- [ ] Switching to Base and back changes nothing but the look

---

# PART E — Redesigning existing pages and apps

A redesign is surgery, not a rebuild. The page already works: it has routes, forms, scripts, analytics, tests, and search rankings. The job is to find what looks generic or broken, move its visual values into tokens, and fix it in place, in an order that gives the most visible improvement for the least risk.

**scan → diagnose → agree → tokenize → fix in priority order → verify**

## E1. Rules of the redesign

- **Keep the stack.** Do not migrate frameworks, styling libraries, or component libraries. With no framework, use plain CSS with custom properties.
- **Do not break what works.** Keep routes and URLs, form field `name`s, element `id`s used by anchors or scripts, `data-*` hooks used by tests or analytics, working ARIA, and the heading hierarchy that search depends on. Before renaming or removing a class, search the scripts for selectors that use it.
- **Diagnose before fixing.** Report every finding first (E8) and let the user veto items. Then fix.
- **Check before adding.** Read the dependency file before importing any library. Never import a package that is not installed; add it explicitly and say so. If the project uses Tailwind, check whether it is v3 or v4 before touching its configuration, since they configure themes differently.
- **Small, reviewable steps.** One priority step (E6) per batch of changes, never the whole site at once, mirroring A6.
- **Never invent a value.** Every font, color, spacing, radius, and curve comes from Part B or the active aesthetic (Part D). If a case is not covered, ask.
- **Copy keeps its meaning.** A copy pass may sharpen wording (A5, B8), but never changes prices, legal text, claims, or facts. Missing facts become marked placeholders (B8).

## E2. Scan

Before judging anything, record:

- Framework, rendering (static, server, client), and the styling method: Tailwind (which version), plain CSS or Sass, CSS modules, CSS in JS, or a component library (shadcn/ui, MUI, Chakra, Bootstrap)
- Where visual values live today: a theme file, CSS variables, a Tailwind config, or scattered literals
- How dark mode works, if it exists (class, `data-*` attribute, or media query)
- The routes and the shared components (nav, footer, buttons, cards, forms)
- The project's own build, lint, and test commands, to run after every batch
- How many distinct fonts, colors, radii, shadows, and z-index values are in use. A quick search shows the scale of the problem:

```bash
# literal colors outside the token files
grep -rnoE "#[0-9a-fA-F]{3,8}\b|rgba?\([^)]*\)|hsla?\([^)]*\)" src | grep -v tokens
# Tailwind arbitrary values that skip the scales
grep -rnoE "\b(text|p[xytrbl]?|m[xytrbl]?|gap|rounded|w|h|tracking|leading)-\[[^]]+\]" src
# fonts, stacking, and motion
grep -rnE "font-family|z-index|transition|animation" src
```

## E3. Audit

Run every area. Each line is a symptom, then the fix, then the rule it resolves to. If the active aesthetic defines a value (a shape, a font, a curve), the aesthetic wins over the default fix.

**Typography**
- Browser default font, or Inter, Roboto, Arial, Open Sans, Helvetica → the theme's `--font-text` (B1)
- Two unrelated typefaces → one family, or the aesthetic's display and text pair (B1, D1)
- Italics → remove; emphasize with weight, size, or color (B1)
- Weights of 800 or more → bold at most. Only 400 and 700 in use → add the medium and semibold the B1 styles need
- Sizes off the scale (`text-[19px]`, `22px`, `1.4rem`) → snap to the closest step below with its line height (B1)
- Text styled with loose sizes and weights → the named B1 styles, defined once
- Paragraphs wider than about 65 characters → cap the measure with `max-width: 65ch`
- Numbers in tables, prices, or stats that shift width → `font-variant-numeric: tabular-nums`
- Headings with Title Case or all caps → sentence case (B8); uppercase only for short labels when the aesthetic allows (D1)
- Orphans, hyphens in copy → `text-wrap: balance` and `pretty`, rewrite the phrase (B1)

**Color and surfaces**
- Off palette backgrounds (`#0a0a0a`, `#121212`, tinted navy) → the theme's surfaces; in Base, the B4 list
- Background gradients, including the purple and blue "AI gradient" → flat surfaces and one accent (B4), unless the aesthetic allows a gradient there (D5)
- Plain hero heading → the B5 text gradient, `--text` → `--text-muted` under an aesthetic
- Several accents, or a neon accent on everything → one accent with one job (C4 applies to pages too)
- Warm and cool grays mixed → one gray family from the theme
- Pure black shadows at low opacity, or shadows implying different light sources → the theme's `--shadow-plate`, one light direction
- A dark section inside a light page, or the reverse, with no reason → one mode per page, or a neighboring surface step
- Empty, flat sections → structure from content: imagery, layering, a pattern the aesthetic allows. Never an ambient gradient

**Layout**
- Everything centered and symmetric → a left aligned header, offset columns, or mixed aspect ratios
- A row of three identical feature cards → a two column zig zag, an asymmetric grid, or a list with real visuals (marketing pages only)
- `height: 100vh` on full screen sections → `min-height: 100dvh`
- No max width → a container of about 1200 to 1440px; hero text capped at 680px (B5)
- Spacing chosen by eye → the B2 scale. Radii chosen by eye → Tailwind radii with the nested formula (B3)
- Equal height cards forced by flex → natural heights, with card buttons pinned to the bottom
- Side by side pricing or comparison lists that start at different heights → fixed height title and price blocks so the lists align
- Icons, play buttons, and button text that look off center → one or two pixels of optical correction
- Crowded marketing sections → one step up the spacing scale. Dense layouts belong to dashboards

**Interaction and states**
- Default easing (`ease`, `linear`, `ease-in-out`) → the theme curves (B7, D2)
- Animated `top`, `left`, `width`, `height` → `transform` and `opacity` (B7)
- Scroll handlers on `window` → `IntersectionObserver` reveals (B7)
- Nav welded to the top, instant menu icon swap, small mobile dropdown → the B7 navigation pattern
- No hover, no pressed feedback, no visible focus ring → the B9 state set; the focus ring uses `--focus-ring` (E4)
- Spinners → skeletons shaped like the content. Blank empty views → composed empty states. `alert()` errors → inline, specific errors (B9)
- Links to `#` → linked or visibly disabled. No current page indicator → mark it (B9)
- No reduced motion handling → B7

**Content**
- Placeholder Latin, "Your headline here" → real draft copy, a blocker (B8)
- Generic names, one face for several people, suspiciously round numbers → B8
- Filler words and vague promises ("streamline", "optimize") → plain, measurable statements (A4, B8)
- Weak CTAs ("Learn more", "Submit") → verb plus outcome (A5). Competing CTAs above the fold → one (A4)
- Proof far from claims, no risk reversal → A4 (marketing pages)
- Cute or loud system messages, passive voice → calm, specific, with the actor named (B8)

**Components**
- Generic cards (border, shadow, white) everywhere → background or spacing alone; cards only where elevation means hierarchy
- A border on one side of a card → all around or none (B4)
- Every section ends in one filled plus one ghost button → one primary, then text links
- Modals for simple actions → inline editing, expanding sections, or a side panel
- A sun and moon toggle as the only theme control → follow the system preference, with the choice in a menu or settings
- A four column footer of links → the main paths plus legal links (B10)
- Badges, avatars, and pills: their shape follows the theme's radius (pills belong to cozy, squares to esports and pixel), not a fixed habit

**Icons and imagery**
- Lucide, Feather, Material Icons or Symbols, or mixed sets → one set from B6, at one stroke weight
- Clichés (a rocket for launch, a shield for security) → a more specific metaphor
- Generic stock photos of smiling teams → real photos or one consistent illustration style
- Missing favicon → a branded one (B10)

**Code**
- Div soup → `nav`, `main`, `section`, `article`, `aside` (B10)
- Inline styles mixed with classes → the project's styling system
- Fixed pixel widths on content → `max-width`, `%`, and `rem` (web pages only; overlays keep pixels, C2)
- `z-index: 9999` and friends → a small named scale in the tokens (base, dropdown, sticky, overlay, modal, toast)
- Dead code, commented blocks, debug logs → remove
- Imports of packages that are not installed → remove or install deliberately
- Missing title, description, `og:image`, generic alt text → B10

**Omissions** (B10): legal links, custom 404, form validation, skip link, cookie consent where required, a way back from every page, and A7 indexing decisions.

## E4. Tokenize

Before changing how anything looks, move the existing values into tokens. This step changes no pixels: screenshots before and after must match. It is what makes every later fix a one line change, and it is what lets a normal website switch aesthetic exactly like an overlay.

**If the project already has a token system** (shadcn/ui variables, an MUI or Chakra theme, a Tailwind theme, Bootstrap variables): keep its names and its value format (hex, HSL channels, or OKLCH). Do not add a second system next to it. Use the D2 contract as the checklist of what every theme must decide, and write each aesthetic as a block that sets the project's own variables.

| D2 and web token | shadcn/ui variable |
|---|---|
| `--surface-page` | `--background` |
| `--text` | `--foreground` |
| `--surface-card` | `--card`, `--popover` |
| `--surface-raised` | `--muted`, `--secondary`, and shadcn's `--accent` (a hover surface, not the brand accent) |
| `--text-muted` | `--muted-foreground` |
| `--accent`, `--on-accent` | `--primary`, `--primary-foreground` |
| `--stroke`, `--stroke-control` | `--border`, `--input` |
| `--focus-ring` | `--ring` |
| `--radius-card` | `--radius` |

**If there is no token system**, add `tokens.css` with the D2 contract and this web layer, then replace literals with variables, file by file:

```css
/* web layer: names a normal page needs, defaulting to the D2 values so every preset works */
:root {
  --surface-page: var(--surface-scene);
  --surface-card: var(--surface-plate-solid);
  --surface-card-raised: var(--surface-raised);
  --radius-card: var(--radius-plate);
  --radius-control: 8px;                 /* buttons and inputs */
  --border-width: 1px;                   /* chunky presets set their --stroke-width */
  --stroke-control: var(--text-muted);   /* input borders need 3:1, muted text always passes */
  --focus-ring: var(--accent);           /* must reach 3:1 against the page */
  --z-dropdown: 10; --z-sticky: 20; --z-overlay: 30; --z-modal: 40; --z-toast: 50;
}

/* Base in light mode; Part B defines only the dark surfaces */
[data-theme="base"][data-mode="light"] {
  --surface-scene: #FFFFFF;
  --surface-plate-solid: #F5F5F5;
  --surface-plate: rgb(245 245 245 / 0.94);
  --surface-raised: #EBEBEB;
  --text: #000000;
  --text-muted: #666666;   /* 5.7:1 on white, 4.8:1 on #EBEBEB */
  --stroke: #E5E5E5;
}
```

**Tailwind v4:** map the tokens to utilities in `@theme inline`. Use different names on the Tailwind side, or the variable refers to itself.

```css
@theme inline {
  --color-page: var(--surface-page);
  --color-card: var(--surface-card);
  --color-fg: var(--text);
  --color-muted: var(--text-muted);
  --color-brand: var(--accent);
  --color-on-brand: var(--on-accent);
  --color-line: var(--stroke);
  --color-ring: var(--focus-ring);
  --font-heading: var(--font-display);
  --font-body: var(--font-text);
  --radius-panel: var(--radius-card);
  --radius-field: var(--radius-control);
  --ease-theme: var(--ease-enter);
}
```

**Tailwind v3:** the same mapping under `theme.extend` in the config (`colors.page: "var(--surface-page)"`, `borderRadius.panel: "var(--radius-card)"`, `fontFamily.heading: "var(--font-display)"`, `transitionTimingFunction.theme: "var(--ease-enter)"`). Opacity modifiers such as `bg-card/80` only work with colors stored as channels, so avoid them on token colors or store the channels.

## E5. Applying an aesthetic to a normal web page

Everything in Part D applies, with these differences from overlays:

- **Legibility:** the C3 overlay floor does not apply; the B1 styles are used as written. Contrast follows WCAG AA, checked on `--surface-page`, `--surface-card`, and `--surface-raised`.
- **Lines:** 1px borders are fine on a page. Base and glass use 1px; the other presets keep their `--stroke-width`, because thick lines are part of their look.
- **Motion:** `prefers-reduced-motion` applies again. Flickers, stepped motion, overshoot, and wipes all fall back to a plain opacity change.
- **Fonts:** use `font-display: swap` with a fallback tuned by `size-adjust` (and `ascent-override` if needed) so the swap does not shift the layout. Preload only the text font of the theme that ships. Overlays use `block` instead (C11).
- **Modes:** each preset is designed in one mode (esports, neon, pixel, editorial, and glass dark; cozy and brutalist light). Offer a light and dark toggle only if every theme the site ships defines both modes, each passing D7. A light neon is a different aesthetic, not a mode.
- **One look or several:** most sites ship one aesthetic, set once on `<html data-theme="name">`. If visitors can switch, set the theme and mode before first paint with a small inline script in `<head>`, so the page never flashes the wrong look:

```html
<script>
  (function () {
    var d = document.documentElement, q = new URLSearchParams(location.search);
    var t = q.get("theme"), m = null;
    try { t = t || localStorage.getItem("theme"); m = localStorage.getItem("mode"); } catch (e) {}
    d.dataset.theme = t || "base";
    d.dataset.mode = m || (matchMedia("(prefers-color-scheme: light)").matches ? "light" : "dark");
  })();
</script>
```

**Per preset on a web page**

| Preset | Adaptation |
|---|---|
| `base` | Part B as written, dark or light |
| `esports` | Chamfered cards and buttons through `clip-path`. A clip also cuts off the focus outline, so clipped controls draw focus inside: `box-shadow: inset 0 0 0 2px var(--focus-ring)`. Uppercase only on nav items, buttons, and labels. Hover grows a 4px accent bar with `scaleX` |
| `neon` | Dark only. Glow (8px at most) on hover and focus of controls, not on resting text blocks. The horizon gradient may sit behind the hero only, with heading contrast checked at its lightest point. The flicker plays once, on the hero heading, at load |
| `pixel` | Press Start 2P for headings at 48px on desktop and 24px under 640px wide. Paragraphs in Geist, since long mono or pixel text is tiring to read; mono for labels and data. Buttons press down with a stepped `translateY(4px)` |
| `cozy` | Pill buttons, 24px cards with the 3px stroke and solid shadow. Overshoot only on small elements (buttons, badges, toasts); section reveals use the Base curve, because a whole section bouncing feels unsteady. Muted text is close to the limit on the page (4.6:1), so keep it off tinted backgrounds |
| `editorial` | Serif display for Heading 1 to 4, body measure at 65ch, dividers between list items, large images with Caption 2 credits, slow 700ms reveals |
| `brutalist` | Buttons sit on a still shadow layer; on `:active` the button moves `translate(6px, 6px)` onto it. The accent fails 3:1 on the page (2.8:1), so `--focus-ring` is `#111111`. Accent only as a fill |
| `glass` | Real `backdrop-filter: blur(16px)` works on a page, for the nav and for cards over photography. Give it real content to blur (images, never a background gradient), add `@supports not (backdrop-filter: blur(1px))` with a solid surface, check contrast against the lightest part of the image behind, and keep blurred elements few and out of long scrolling lists |

## E6. Fix priority

Ordered for the most visible improvement at the least risk. Each step is one reviewable batch.

0. **Tokenize** (E4). No visual change; verify screenshots match.
1. **Fonts**
2. **Color and surfaces**, including removing background gradients
3. **Hover, active, and focus states**
4. **Layout and spacing**: container, grid, spacing scale, radii
5. **Motion**: theme curves, reveals, navigation
6. **Generic components** replaced
7. **Loading, empty, and error states**
8. **Copy pass**
9. **Type scale polish**

When the user asked for an aesthetic, steps 1, 2, and 5 are done by writing the theme (D3) right after step 0; then continue from step 3.

## E7. Verify

After every batch, not only at the end:

- The project's build, lint, and tests pass
- Screenshots before and after of every changed route at 390px and 1440px, in every shipped theme and mode
- A keyboard pass: every control reachable, focus always visible, no trap in menus or dialogs
- Forms still validate and submit; links, anchors, and script hooks still work; no new console errors
- D7 for each theme, with the web contrast rules from E5
- No layout shift from fonts or images (cumulative layout shift under 0.1)

## E8. Redesign output format

Return the diagnosis before changing anything:

```
Diagnosis: <site or page>
Stack: <framework, styling method, component library, Tailwind version>
Tokens today: <where values live, or "scattered literals">
Requested look: <aesthetic and mode, or Base>

| # | Area | Finding | Where | Fix | Rule | Risk |
|---|------|---------|-------|-----|------|------|
| 1 | Type | Inter on all text | app/layout.tsx:8 | Theme --font-text | B1 | Low |
| 2 | Color | Purple gradient hero background | Hero.tsx:14 | Flat --surface-page | B4 | Low |
| 3 | States | Buttons have no focus ring | Button.tsx:22 | --focus-ring outline | B9 | Low |

Plan: E6 steps 0 to 9, one batch each. Reply with any row numbers to skip.
```

Then apply one step at a time, and after each step report what changed, the files touched, and the E7 results.

## E9. Redesigning an existing overlay

Same flow, different audit. Scan the browser sources, the OBS source list, and any provider widget (StreamElements, Streamlabs) in use. Audit against C2 to C12 and D7 instead of E3: canvas and safe areas, legibility after compression, plates, the camera ring, chat security and pruning, the alert queue, broadcast states, and the configuration. Provider widgets are styled only through the CSS, HTML, and fields their editor exposes; keep their field names and event handlers intact, and move their colors and fonts into the same tokens so the widget follows the theme.

---

# Output format

**For a stream overlay**, return these in order before writing code:

1. **Canvas** — size, platform, software, and any assumptions from C1
2. **Aesthetic brief** — the preset or custom theme and its six lines (D3)
3. **Scene list** — each scene with the elements it contains (C2)
4. **Layout map** — a rough ASCII diagram per scene, with every element's position and size in pixels, the safe area, and the HUD and face areas marked
5. **Source map** — one row per browser source: file, URL parameters, position and size, and its place in the layer stack (C2, C12)
6. **Data and control** — where chat and events come from, what the control dock does, and which secrets are needed and where they live (C10)

Then build in this order: `tokens.css` and the theme → camera frame → chat → alerts → goals and timers → full screen scenes → stinger → control dock.

**For an aesthetic change** on something already built, return only:

1. **Aesthetic brief** (D3)
2. **Token diff** — each variable that changes, old value → new value, plus any optional ornament markup it turns on
3. **D7 results**
4. **Preview URL** with `?theme=`

Then edit the theme files only. Layout, data, and logic stay untouched.

**For a redesign** of an existing website, app, component, or overlay, return the E8 diagnosis first and wait for vetoes, then apply the E6 steps one batch at a time with E7 results after each.

**For a landing page**, return these in order before writing code:

1. **Page outline** — sections and their order
2. **Hero copy** — headline, subheadline, CTA, proof line
3. **Benefits** — three to five outcome driven bullets
4. **How it works** — three steps
5. **FAQ** — six to twelve questions and answers
6. **SEO / AEO** — index or noindex recommendation, plus title and meta if indexed
7. **Layout recommendation** — A, B, C, or D, and why

Then build section by section per A6.

---

# Quick checklist

**Strategy**
- [ ] One offer, one audience, one primary action
- [ ] No competing CTAs above the fold
- [ ] Specific numbers instead of vague verbs
- [ ] At least one risk reversal
- [ ] Proof sits next to the claim it supports
- [ ] Layout type chosen deliberately

**Visual**
- [ ] Single approved typeface (or the active aesthetic's pair, D1), no italics, no ultra bold
- [ ] No hyphens in copy, no orphaned words
- [ ] Every font size lands on a Tailwind scale step
- [ ] Every text element uses a named text style (Heading, Title, Body, Button, Caption)
- [ ] Every spacing value comes from the spacing table
- [ ] Nested radii follow the formula
- [ ] No single sided card borders, no background gradients (unless the active aesthetic allows them, D5)
- [ ] Hero heading and subheading capped at 680px with meaningful line breaks
- [ ] Icons from Phosphor, Solar, or Iconamoon
- [ ] Every transition uses the B7 base curve (or the active theme curves), scroll reveals use IntersectionObserver
- [ ] Tagline reveal section present, minimum two lines, words activate one at a time on scroll
- [ ] No invented prices, stats, or testimonials; missing facts use marked placeholders
- [ ] Checked at 390px with no overflow

**Content and ship**
- [ ] Real draft copy, believable names and numbers, no banned filler words
- [ ] Hover, active, focus, loading, empty, and error states all present
- [ ] No dead links, current nav item indicated
- [ ] 404, legal links, form validation, favicon, meta tags, alt text

**Overlays** (Part C)
- [ ] Fixed canvas size, transparent page background, no scrollbars
- [ ] All styling reads D2 tokens; no literal colors, fonts, or curves in structural CSS
- [ ] Persistent elements inside the safe area, clear of the game HUD and the camera's face area
- [ ] No text below 18px on a 1080p canvas; chat in Body 7, glance info in Body 8; 1440p via `?scale=`, never stretched
- [ ] All text on solid plates, no `backdrop-filter` over gameplay, strokes at least 2px
- [ ] Camera hole and camera source positions stated in pixels; ring opaque or mask specified
- [ ] Layer stack stated; cut out cameras have their tag in the under layer
- [ ] Chat capped and pruned, untrusted text never set with `innerHTML`, deleted messages removed, emote offsets by code point
- [ ] Alerts queued one at a time, bursts merged, test triggers available
- [ ] Progress fills use `scaleX`, timers compute from a target timestamp
- [ ] No loading, empty, or error states visible to viewers; reconnects with backoff
- [ ] Fonts bundled locally and loaded before the first animation
- [ ] `?demo=1` and `?preview=1` work; checked at 33% scale and after a one hour soak
- [ ] Served from localhost, tested inside OBS with remote debugging
- [ ] No tokens or keys in HTML, the repo, or URLs
- [ ] Nothing flashes more than three times per second

**Aesthetics** (Part D)
- [ ] Aesthetic brief written before code; Base used when no look was requested
- [ ] Theme fills every D2 variable; switching themes touches no layout or logic
- [ ] At most one token group borrowed when blending; brand accent applied and checked
- [ ] D7 checks pass for every shipped theme
- [ ] Custom themes evoke the reference without copying logos, fonts, or assets

**Redesign** (Part E)
- [ ] Stack, token location, dark mode method, and project commands recorded before judging
- [ ] Diagnosis reported with file locations before any change; vetoed rows skipped
- [ ] Tokenized first, with screenshots matching before and after
- [ ] Existing token system reused, not duplicated; Tailwind version checked
- [ ] Routes, form names, ids, data hooks, ARIA, and heading hierarchy preserved
- [ ] Fixes applied in E6 order, one batch at a time, build and tests passing after each
- [ ] Every shipped theme and mode passes AA contrast and has a visible focus ring
- [ ] No theme flash on load; no layout shift from font swaps

**Video player** (C7)
- [ ] Every control is a labeled button; keyboard shortcuts work when the player has focus
- [ ] Controls autohide only while playing, never while paused or focused
- [ ] Muted autoplay with a visible pause control; no autoplay under reduced motion
- [ ] Captions track on any video with speech; embeds behind a facade

---

## Credits

The no invented facts rule and reduced motion support for the tagline reveal were suggested by [@allen-baler](https://github.com/allen-baler) in [#1](https://github.com/elayadesign/ai-design-skills/pull/1).

Parts of this skill were adapted from [taste-skill](https://github.com/Leonxlnx/taste-skill) by Leon Lin ([@LexnLin](https://x.com/LexnLin)), MIT licensed. Its redesign audit structure, content realism checks, and motion and navigation ideas informed the matching sections here, which have since been rewritten.

Part E builds on [redesign-existing-projects](https://github.com/elayadesign/redesign-skill), MIT licensed: its scan, diagnose, and fix flow, its audit areas, and its fix priority were rewritten here to share this file's values, the aesthetic layer, and the overlay rules.

<details>
<summary>taste-skill license</summary>

```
MIT License

Copyright (c) 2026 Leonxlnx

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
</details>
