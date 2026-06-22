# Template C — Minimal Centered

> 🆕 First time? Read the [prompt pack intro](README.md) first — it explains how to use these and what the words mean.

## At a glance

**The feel:** Quiet, elegant, typographic. Everything is centered on a warm cream card with lots of
empty space. The giant prize number is the star.

**Best for:** Boutique / premium brands, single-message emails, save-the-dates, "thank you" notes —
when less is more and you want one idea to land beautifully.

**One-line description:** *A centered, cream-colored card where a huge "Rs 50,000" is the hero,
framed by thin hairlines and one neat button.*

## What it looks like, top to bottom

1. **Logo, centered.**
2. A centered **eyebrow** with thin horizontal lines on either side of it (like a divider with a label).
3. A centered **headline**, second line in purple.
4. The **giant prize number** — "Rs 50,000" set very large in purple — the visual centerpiece.
5. A centered **button** (just as wide as its text, not full width).
6. A centered **3-column detail strip** with thin vertical dividers.
7. **"What to do next"** shown as one tidy centered line with dot separators (not numbered blocks).
8. **Footer** on deep plum, centered.

---

## 📋 The prompt — copy everything in this box

```text
You are an expert email developer. Build me ONE complete, ready-to-send HTML email file called
"Minimal Centered". It must look polished in Gmail, Apple Mail, and Outlook, and on mobile phones.

DESIGN DIRECTION — "Minimal Centered":
Quiet, elegant, and typographic. Everything is centered with generous whitespace on a warm cream
card. The single biggest element is the prize amount, treated as a large display number. Restraint
is the point — minimal decoration.

BRAND KIT:
- Font: Nunito (load from Google Fonts), falling back to Helvetica, Arial, sans-serif.
  Headlines weight 800, body weight 500.
- Colors: deep plum #1A0B2E, brand purple #41009A, violet #7C4DFF, coral #FF6B4A,
  warm cream card #FAF6F0, page background #E7E4DF, body text #444444, muted text #666666,
  hairline lines a soft tan like #ECE0D0.
- Logo image: https://lingotran.com/media/logo.png (alt text "Lingotran").

LAYOUT (top to bottom), inside a cream #FAF6F0 rounded card with a subtle border, max width 600px,
centered on a #E7E4DF page. EVERYTHING is center-aligned:
1. Logo, centered, about 150px wide.
2. A centered eyebrow row: a thin tan hairline, then the coral uppercase label
   "BONJOUR BATTLE · SEASON 1", then another thin tan hairline (label sits between two short lines).
3. A centered headline in deep plum: "You're in." line break "Now let's begin." with the second
   line in brand purple #41009A.
4. A short centered paragraph (max ~400px wide so the lines aren't too long): "The French assessment
   course is open. Finish your first lessons before assessment night on 24 June."
5. THE HERO: a centered "PRIZE POOL" mini-label, then "Rs 50,000" set VERY large (display size, very
   bold) in brand purple, then a short centered line "Plus a certificate for every student who
   completes the assessment."
6. A centered button (inline-block, sized to its text with comfortable padding — NOT full width):
   brand purple #41009A background, white text, rounded 8px, "Log in and start learning →", linking
   to https://learn.lingotran.com/bonjour-battle. Under it a small muted centered line:
   "Takes a minute · the course closes 23 June". Make it a bulletproof button.
7. A centered 3-column detail strip with a thin tan line above and below it and thin vertical dividers
   between columns, each centered: When = "24 June · 7:30 PM"; Format = "Online · free entry";
   Level = "Beginners welcome". On screens under ~480px, stack into one column.
8. A "WHAT TO DO NEXT" mini-label, then ONE centered line listing the three steps separated by dots:
   "Log in and open the course  ·  Finish your lessons by 23 June  ·  Show up on assessment night".
9. Footer on deep-plum #1A0B2E, centered, light text: "Lingotran", then
   "info@lingotran.com · 96060 81499", then links "View in browser · Unsubscribe", then
   "© 2026 Lingotran Private Limited. You registered for Bonjour Battle Season 1."

TECHNICAL RULES (important — this is an EMAIL, not a web page):
- Use table-based layout (not flexbox/grid) so it survives Outlook; center with align="center".
- Put ALL styling inline (keep a <style> block for the font + mobile tweaks).
- Max content width 600px; center the card on the page.
- Responsive: under ~480px, reduce padding/font sizes (the big prize number should scale DOWN so it
  never overflows the screen) and stack the 3-column strip into one column. No sideways scrolling.
- Every image needs alt text. The logo links to https://lingotran.com.
- Add a hidden preheader: "You're in — Rs 50,000 prize pool. Start the French course before 24 June."
- Strong contrast, tap-friendly spacing. Output ONE complete HTML file, no explanation around it.
```

---

## What makes this design work (the UI/UX considerations)

- **One hero, on purpose.** By making the prize number enormous and everything else small, the design
  says "this is the one thing to remember." Minimalism only works when you choose a single focal point.
- **Centering creates ceremony.** Centered layouts feel formal and calm (think invitations). They're
  less "scannable" than left-aligned, so they suit *short* messages — which this is.
- **Hairlines instead of boxes.** Thin lines separate sections without adding visual weight, keeping
  the airy feel. Boxes would make it feel busier.
- **Whitespace is the design.** The empty space around the prize is what makes it feel premium. Resist
  the urge to fill it.
- **The button is sized to its words.** A compact centered button feels refined; a full-width bar would
  feel heavier and break the delicate mood.
- **Watch line length.** Centered paragraphs are capped to ~400px so lines stay short and readable —
  long centered lines are tiring to read.
- **The big number must scale on mobile.** A giant display number can overflow a phone screen, so the
  prompt explicitly shrinks it on small screens.

## Why these choices

| Choice | Why it's there |
|--------|----------------|
| Cream card (`#FAF6F0`) not pure white | Warmer, softer, more "boutique" than stark white. |
| Prize as a giant display number | Turns the reward into the memorable hero with zero clutter. |
| Hairlines + centered text | Maximum elegance, minimum noise — fits a single, calm message. |
| Steps on one dotted line | Keeps the minimal rhythm; numbered blocks would add visual weight. |
| Compact centered button | Refined and intentional, in keeping with the restrained mood. |

## Make it yours (just ask the AI in plain words)

- *"Make the prize number even bigger and add a subtle shadow."*
- *"Use white instead of cream for the card."*
- *"Add a small centered photo above the headline."*
- *"Left-align everything instead of centering"* (if you find centered hard to scan).
- *"Add a thin divider line above the footer."*

## Before you send (in addition to the [universal checklist](README.md#universal-checklist-applies-to-all-5-designs))

- [ ] On a **phone**, confirm "Rs 50,000" fits on one line and doesn't overflow.
- [ ] Make sure centered text blocks aren't too wide (short lines read better when centered).
- [ ] Cream-on-cream can wash out in **dark mode** — verify the card still looks distinct, or add a faint border.

---

*Template C of 5 · [Back to the prompt pack](README.md) · [See it live](../index.html)*
