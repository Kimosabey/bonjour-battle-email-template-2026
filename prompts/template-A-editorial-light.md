# Template A — Editorial Light

> 🆕 First time? Read the [prompt pack intro](README.md) first — it explains how to use these and what the words mean.

## At a glance

**The feel:** Clean, calm, white, magazine-like. A thin coral line across the very top is the only
flourish. Lets the words breathe.

**Best for:** Newsletters, course updates, "you're in" confirmations — anything where you want to
look trustworthy and content-first rather than flashy.

**One-line description:** *A white card with a coral top stripe, a left-aligned logo, a bold
headline, a colorful hero banner, one purple button, and tidy detail rows.*

## What it looks like, top to bottom

1. A thin **coral stripe** (3px) across the top edge.
2. **Logo**, top-left.
3. **Coral eyebrow** ("Bonjour Battle · Season 1"), then a big dark **headline** with the second
   line in purple, then a short paragraph.
4. A **hero banner** — a purple→violet gradient rectangle (stands in for a real photo).
5. The **purple button** (full width) with a small reassuring line under it.
6. A **prize box**: soft purple background with a purple bar down its left edge.
7. **Detail rows** (When / Format / Level) — label on the left, answer on the right, thin lines between.
8. **"What to do next"** — three numbered steps.
9. **Footer** on a deep-plum background.

---

## 📋 The prompt — copy everything in this box

```text
You are an expert email developer. Build me ONE complete, ready-to-send HTML email
file called "Editorial Light". It must look polished in Gmail, Apple Mail, and Outlook,
and on mobile phones.

DESIGN DIRECTION — "Editorial Light":
Clean, white, calm, magazine-style. Content-first with generous whitespace. The only
decorative touch is a thin 3px coral line across the very top of the email.

BRAND KIT:
- Font: Nunito (load from Google Fonts), falling back to Helvetica, Arial, sans-serif.
  Headlines weight 800, body weight 500.
- Colors: deep plum #1A0B2E, brand purple #41009A, violet #7C4DFF, coral #FF6B4A,
  cream page background #E7E4DF, soft purple tint #F0E6FF, body text #444444, muted text #666666.
- Logo image: https://lingotran.com/media/logo.png (alt text "Lingotran").

LAYOUT (top to bottom), inside a white rounded card, max width 600px, centered on a cream page:
1. A 3px-tall coral (#FF6B4A) bar spanning the full top.
2. Logo, left-aligned, about 148px wide.
3. Coral uppercase eyebrow "BONJOUR BATTLE · SEASON 1" (small, bold, letter-spaced).
4. Headline in deep plum, very bold: "You're in." then a line break, then "Now let's begin."
   with "Now let's begin." in brand purple #41009A.
5. A short paragraph: "The French assessment course is open. Log in and finish your first
   lessons before assessment night on 24 June." (bold the "24 June").
6. A hero banner rectangle (~200px tall, rounded corners) filled with a 135-degree gradient
   from #41009A to #7C4DFF. Put a label inside it: "Hero image · replace with hosted 1200×600".
   (This is a placeholder for a real photo the user will host later.)
7. A full-width button: background brand purple #41009A, white text, rounded 8px, comfortable
   padding, text "Log in and start learning →", linking to
   https://learn.lingotran.com/bonjour-battle. Make it a "bulletproof" button that still shows
   if images are off. Under it, a small muted line: "Takes a minute to begin · the course closes 23 June".
8. A prize box: soft purple #F0E6FF background, with a 4px brand-purple bar on its LEFT edge,
   rounded on the right. Inside: tiny coral label "PRIZE POOL", then large bold "Rs 50,000",
   then "Plus a certificate for every student who completes the assessment."
9. Three detail rows, each with the label on the left and the value on the right, separated by
   thin hairlines: When = "24 June · 7:30 PM"; Format = "Online · free to enter";
   Level = "Beginners welcome".
10. A "WHAT TO DO NEXT" section with three numbered steps (small purple-tinted circles with the
    number inside): 1) Log in and open the Bonjour Battle course. 2) Finish your lessons before
    23 June. 3) Show up on assessment night, 24 June.
11. Footer on a deep-plum #1A0B2E background, light text: the word "Lingotran", then
    "info@lingotran.com · 96060 81499", then links "View in browser · Unsubscribe", then
    "© 2026 Lingotran Private Limited. You received this because you registered for Bonjour Battle Season 1."

TECHNICAL RULES (important — this is an EMAIL, not a web page):
- Use table-based layout (not flexbox/grid) so it survives Outlook.
- Put ALL styling inline on the elements (also keep a <style> block for the font + mobile tweaks).
- Max content width 600px; center the card on the cream background.
- Make it responsive: on screens under ~480px, reduce side padding and font sizes slightly so
  nothing is cramped and there is no sideways scrolling.
- Every image needs alt text. The logo links to https://lingotran.com.
- Add a hidden preheader text near the top: "You're in — the French course is open. Start before 24 June."
- Keep good color contrast and tap-friendly spacing. Output ONE complete HTML file I can copy, with
  no explanation around it.
```

---

## What makes this design work (the UI/UX considerations)

- **Visual hierarchy through size + color, not decoration.** The headline is the biggest, darkest
  thing; the purple second line pulls the eye; the button is the only solid color block. Your eye
  naturally goes headline → button. *This is the core skill: make the most important thing look most important.*
- **Whitespace = trust.** The generous padding and the airy white card read as calm and credible.
  Cramped emails feel like spam.
- **One accent color, used sparingly.** Coral appears only in the top stripe and the tiny labels.
  A little accent pops; a lot of accent becomes noise.
- **A single, obvious CTA.** One full-width purple button, repeated nowhere else, so there's zero
  confusion about what to click.
- **Scannability.** Labels-on-left / values-on-right rows and numbered steps let people *skim* and
  still get the key facts (when, where, what to do).
- **Readable type.** Body text around 15–17px with relaxed line spacing — comfortable on a phone.
- **Email-safe construction.** Tables + inline CSS so Outlook doesn't break the layout; a bulletproof
  button so the call-to-action survives even with images turned off.
- **Accessibility.** Strong contrast (dark text on white, white text on purple), alt text on images,
  and real text (not text baked into a picture) so screen readers and "images-off" inboxes still work.

## Why these choices

| Choice | Why it's there |
|--------|----------------|
| White background, thin coral line | Signals "editorial / official," not promotional. The line adds brand color without clutter. |
| Purple only on the button + one headline word | Trains the eye: purple = "this is actionable / important." |
| Hero as a gradient placeholder | Lets you ship now and drop in a real hosted photo later without redesigning. |
| Prize in a tinted box with a side bar | A "callout" pattern — separates the reward from body text so it gets noticed. |
| Numbered steps | People skip paragraphs but follow numbers. Reduces "what do I do now?" friction. |
| Dark footer | Visually closes the email and groups the legal/contact bits away from the message. |

## Make it yours (just ask the AI in plain words)

- *"Swap the gradient hero for my real photo at [link], keep it 600×300."*
- *"Change coral to my brand's accent color [hex]."*
- *"Make the headline say [your headline]."*
- *"Add a second small text link under the button to the full schedule."*
- *"Give me a plain-text version too, for inboxes that block HTML."*

## Before you send (in addition to the [universal checklist](README.md#universal-checklist-applies-to-all-5-designs))

- [ ] Replace the gradient hero with a **real hosted image** (or keep it — it looks fine as-is).
- [ ] Confirm the thin coral line shows on top (some inboxes clip the very top — keep it 3px+).
- [ ] Check the white card edges on **dark mode** — add a subtle border if it disappears on dark backgrounds.

---

*Template A of 5 · [Back to the prompt pack](README.md) · [See it live](../index.html)*
