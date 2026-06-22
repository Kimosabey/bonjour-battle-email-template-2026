# Template B — Gradient Premium

> 🆕 First time? Read the [prompt pack intro](README.md) first — it explains how to use these and what the words mean.

## At a glance

**The feel:** Bold, premium, branded. A big purple gradient header makes it feel like a product
launch or a "you're invited" moment.

**Best for:** Announcements, launches, VIP/registration confirmations — when you want energy and a
strong brand presence the instant the email opens.

**One-line description:** *A large purple→violet gradient header with the logo and headline on it,
then a clean white body with a wide prize band and a 3-column detail grid.*

## What it looks like, top to bottom

1. A **big gradient header** (deep purple to violet, diagonal) filling the whole top — logo on a
   white chip, coral eyebrow, large **white headline**, short white sub-text. Soft translucent
   circles float in the background for depth.
2. The **purple button** (full width).
3. A **wide prize band**: the prize amount on the left, a one-line description on the right.
4. A **3-column detail grid** (When / Format / Level) that looks like neat tiles — and stacks into
   one column on a phone.
5. **"What to do next"** — three numbered steps.
6. **Footer** on deep plum.

---

## 📋 The prompt — copy everything in this box

```text
You are an expert email developer. Build me ONE complete, ready-to-send HTML email file
called "Gradient Premium". It must look polished in Gmail, Apple Mail, and Outlook, and on
mobile phones.

DESIGN DIRECTION — "Gradient Premium":
Bold, premium, and brand-forward. The signature element is a large diagonal purple gradient
header that the logo and headline sit ON TOP of (white text over the gradient). The body below
is clean and white. It should feel like a confident product launch.

BRAND KIT:
- Font: Nunito (load from Google Fonts), falling back to Helvetica, Arial, sans-serif.
  Headlines weight 800, body weight 500.
- Colors: deep plum #1A0B2E, brand purple #41009A, violet #7C4DFF, coral #FF6B4A,
  cream page background #E7E4DF, soft purple tint #F0E6FF, body text #444444, muted text #666666.
- Logo image: https://lingotran.com/media/logo.png (alt text "Lingotran").

LAYOUT (top to bottom), inside a white rounded card, max width 600px, centered on a cream page:
1. A large header block (about 38px of padding) filled with a 150-degree gradient from #41009A
   to #5A18C4 to #7C4DFF. On top of it, in this order: the logo on a small white rounded chip;
   a coral-tinted uppercase eyebrow "BONJOUR BATTLE · SEASON 1" (use a soft coral like #FFCBB9 so
   it reads on the gradient); a large bold WHITE headline "You're in. Now let's begin."; a short
   white paragraph (slightly transparent white) "The French assessment course is open. Finish your
   first lessons before assessment night on 24 June." Add 2 large, very faint translucent circles
   in the header background for subtle depth (one white, one coral).
2. A full-width "bulletproof" button: brand purple #41009A background, white text, rounded 8px,
   text "Log in and start learning →", linking to https://learn.lingotran.com/bonjour-battle.
   Under it a small muted line: "Takes a minute · the course closes 23 June".
3. A wide prize band: soft purple #F0E6FF background with a 4px coral #FF6B4A bar on the left edge,
   rounded on the right. On the LEFT: tiny coral label "PRIZE POOL" and large bold "Rs 50,000".
   On the RIGHT: "+ a certificate for every student who completes the assessment." On a phone these
   stack vertically.
4. A 3-column detail grid that looks like joined tiles (thin light dividers between them), each
   white with a small label and value: When = "24 June · 7:30 PM"; Format = "Online · free to
   enter"; Level = "Beginners welcome". On screens under ~480px, stack the three into one column.
5. A "WHAT TO DO NEXT" section with three numbered steps (small purple-tinted circles with the
   number inside): 1) Log in and open the Bonjour Battle course. 2) Finish your lessons before
   23 June. 3) Show up on assessment night, 24 June.
6. Footer on a deep-plum #1A0B2E background, light text: "Lingotran", then
   "info@lingotran.com · 96060 81499", then links "View in browser · Unsubscribe", then
   "© 2026 Lingotran Private Limited. You received this because you registered for Bonjour Battle Season 1."

TECHNICAL RULES (important — this is an EMAIL, not a web page):
- Use table-based layout (not flexbox/grid) so it survives Outlook.
- IMPORTANT: Outlook ignores CSS gradients. For the gradient header, ALSO set a solid #41009A
  background color as a fallback (and ideally a VML/Outlook fallback) so Outlook shows solid purple,
  never a white/blank header. White text must stay readable on that solid purple.
- Put ALL styling inline (keep a <style> block for the font + mobile tweaks).
- Max content width 600px; center the card on the cream background.
- Responsive: under ~480px, reduce side padding/font sizes, and stack the prize band and the
  3-column grid into single columns. No sideways scrolling.
- Every image needs alt text. The logo links to https://lingotran.com.
- Add a hidden preheader: "You're in — the French course is open. Start before 24 June."
- Strong contrast, tap-friendly spacing. Output ONE complete HTML file, no explanation around it.
```

---

## What makes this design work (the UI/UX considerations)

- **Immediate brand impact.** A full-bleed gradient header is the first thing the eye lands on, so
  the brand "owns" the top of the inbox preview. Great for launches; a bit much for quiet newsletters.
- **Contrast does the hierarchy.** White text on a saturated gradient is naturally high-contrast and
  commanding — the headline can't be missed.
- **The body calms down.** After the loud header, the white body with simple tiles keeps the
  information easy to read. Loud-then-calm is a deliberate rhythm.
- **Tiles = scannable facts.** A 3-up grid signals "three quick facts" and invites a glance rather
  than a read.
- **Outlook gradient fallback is the #1 risk.** Outlook ignores CSS gradients; without a solid-color
  fallback you'd get white text on a white header = invisible. The prompt forces a solid fallback.
- **Mobile stacking.** Multi-column layouts must collapse to a single column on phones or they get
  squished — the prompt makes the prize band and grid stack.

## Why these choices

| Choice | Why it's there |
|--------|----------------|
| Gradient header with text on top | Maximum brand presence and a "premium launch" mood in the first second. |
| Soft coral eyebrow (`#FFCBB9`) | Plain coral can vibrate against purple; a softer tint stays legible and elegant. |
| Wide prize band (side-by-side) | Treats the reward like a banner headline — more prominent than a small box. |
| Joined tiles for details | Reads as a compact "spec strip," modern and product-like. |
| Solid-purple Outlook fallback | Guarantees the hero never breaks in the inbox with the largest desktop user base. |

## Make it yours (just ask the AI in plain words)

- *"Make the gradient go from [hex] to [hex]."*
- *"Put a real hero image behind the header instead of a gradient, with a dark overlay so white text stays readable."*
- *"Move the prize band above the button."*
- *"Add a fourth detail tile for 'Language: French'."*
- *"Tone it down — smaller header, less saturated gradient."*

## Before you send (in addition to the [universal checklist](README.md#universal-checklist-applies-to-all-5-designs))

- [ ] **Test in Outlook specifically** — confirm the header shows solid purple (not white) and the
      white headline is readable.
- [ ] Check the header on **dark mode** — gradients can shift; make sure text contrast holds.
- [ ] If you add a real header photo, **darken it** behind the text or the white words may vanish.

---

*Template B of 5 · [Back to the prompt pack](README.md) · [See it live](../index.html)*
