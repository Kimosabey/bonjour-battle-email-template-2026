# Template D — Dark Editorial

> 🆕 First time? Read the [prompt pack intro](README.md) first — it explains how to use these and what the words mean.

## At a glance

**The feel:** Dramatic, premium, "after dark." A deep plum-to-purple background with glowing accents.
High contrast and confident.

**Best for:** Premium launches, evening/event invites, gaming or "season" themes, anything that wants
to feel exclusive and modern. Also a natural match for readers in dark mode.

**One-line description:** *A dark purple card with white headlines, a glowing gradient button, and
soft purple-tinted boxes — the moody counterpart to Template A.*

## What it looks like, top to bottom

1. **Logo on a white chip**, top-left (so it stays visible against the dark background).
2. **Coral eyebrow**, a white **headline** with the second line in bright violet, then a soft-white
   paragraph.
3. A **hero banner** — a violet→purple gradient rectangle with floating translucent circles.
4. A **glowing gradient button** (purple→violet) that looks like it's lit up.
5. A **prize box** with a faint translucent fill and a glowing purple border.
6. **Detail rows** (When / Format / Level) divided by faint light lines.
7. **"What to do next"** — three numbered steps in glowing circles.
8. An even **darker footer** at the bottom.

---

## 📋 The prompt — copy everything in this box

```text
You are an expert email developer. Build me ONE complete, ready-to-send HTML email file called
"Dark Editorial". It must look polished in Gmail, Apple Mail, and Outlook, and on mobile phones.

DESIGN DIRECTION — "Dark Editorial":
Dramatic and premium, with a dark plum-to-purple background and light text. High contrast, a glowing
gradient button, and subtle glowing accents. It should feel like an exclusive, after-dark invitation.
It is the dark-mode sibling of a clean white editorial layout.

BRAND KIT:
- Font: Nunito (load from Google Fonts), falling back to Helvetica, Arial, sans-serif.
  Headlines weight 800, body weight 500.
- Colors: background gradient from #1A0B2E to #241046; brand purple #41009A; violet #7C4DFF;
  bright violet for accents #9B6BFF; coral #FF6B4A; page background #1A0B2E (deep plum).
  Text: white #FFFFFF for headlines, soft light lavender (about rgba white 78%) for body, muted
  lavender #B5A9CE in the footer.
- Logo image: https://lingotran.com/media/logo.png (alt text "Lingotran").

LAYOUT (top to bottom), inside a rounded card filled with a 160-degree gradient from #1A0B2E to
#241046, max width 600px, centered on a deep-plum page:
1. The logo placed on a small WHITE rounded chip (so it stays visible on the dark card), top-left.
2. Coral uppercase eyebrow "BONJOUR BATTLE · SEASON 1".
3. A large bold WHITE headline: "You're in." line break "Now let's begin." with the second line in
   bright violet #9B6BFF.
4. A short paragraph in soft translucent white: "The French assessment course is open. Log in and
   finish your first lessons before assessment night on 24 June." (bold the "24 June" in solid white).
5. A hero banner (~190px tall, rounded) filled with a 135-degree gradient from #7C4DFF to #41009A,
   with two faint translucent circles for depth and a label "Hero image · replace with hosted 1200×600".
6. A full-width "bulletproof" button with a gradient from #41009A to #7C4DFF, white text, rounded 8px,
   and a soft purple glow shadow, text "Log in and start learning →", linking to
   https://learn.lingotran.com/bonjour-battle. Under it a small muted line:
   "Takes a minute to begin · the course closes 23 June".
7. A prize box: a faint translucent white fill with a glowing purple border (about #7C4DFF at ~45%),
   rounded. Inside: tiny coral label "PRIZE POOL", large bold WHITE "Rs 50,000", then a soft-white line
   "Plus a certificate for every student who completes the assessment."
8. Three detail rows, label on the left and value on the right, divided by faint light hairlines:
   When = "24 June · 7:30 PM"; Format = "Online · free to enter"; Level = "Beginners welcome".
   Labels in muted lavender, values in solid white.
9. A "WHAT TO DO NEXT" label in bright violet, then three numbered steps in small glowing
   purple-tinted circles: 1) Log in and open the Bonjour Battle course. 2) Finish your lessons before
   23 June. 3) Show up on assessment night, 24 June.
10. A darker footer panel (slightly darker than the card, e.g. black at ~25%): "Lingotran", then
    "info@lingotran.com · 96060 81499", then links "View in browser · Unsubscribe", then
    "© 2026 Lingotran Private Limited. You received this because you registered for Bonjour Battle Season 1."

TECHNICAL RULES (important — this is an EMAIL, not a web page):
- Use table-based layout (not flexbox/grid) so it survives Outlook.
- Outlook ignores CSS gradients: set SOLID fallbacks — card falls back to solid #1A0B2E, the hero and
  button fall back to solid #41009A — so nothing turns white/blank in Outlook.
- DARK-MODE CAUTION: some email apps auto-invert colors. Keep text defined as light on a dark
  background and avoid relying on transparency for legibility; ensure the white logo chip stays light.
- Put ALL styling inline (keep a <style> block for the font + mobile tweaks).
- Max content width 600px; center the card on the page.
- Responsive: under ~480px, reduce side padding and font sizes. No sideways scrolling.
- Every image needs alt text. The logo links to https://lingotran.com.
- Add a hidden preheader: "You're in — the French course is open. Start before 24 June."
- Strong contrast (this matters more on dark), tap-friendly spacing. Output ONE complete HTML file,
  no explanation around it.
```

---

## What makes this design work (the UI/UX considerations)

- **Dark backgrounds raise the stakes.** Light text on dark reads as premium, focused, and modern —
  but only if contrast is high. Faint grey text on dark is the most common dark-design mistake; here
  headlines are pure white.
- **Glow = hierarchy.** The button's soft shadow and the prize box's glowing border draw the eye to the
  two things that matter most, without adding more color.
- **The white logo chip is a deliberate fix.** Most logos are dark and vanish on dark backgrounds;
  putting it on a small white chip keeps it crisp. *A classic dark-UI consideration.*
- **Bright violet as the spotlight accent.** A single brighter hue (`#9B6BFF`) on the headline's second
  line and step numbers gives life against the deep plum.
- **Dark mode double-handling.** Ironically, dark designs can break in inboxes that *auto-invert* colors.
  The prompt tells the AI to define colors explicitly and avoid relying on transparency for legibility.
- **Outlook fallbacks are critical here.** If the gradient card fails to a white background in Outlook,
  the white text disappears — so solid dark fallbacks are non-negotiable.

## Why these choices

| Choice | Why it's there |
|--------|----------------|
| Plum→purple gradient card | Creates depth and a premium "after-dark" mood vs. a flat black. |
| White logo on a chip | Guarantees the brand mark stays visible on the dark field. |
| Glowing button + bordered prize | Light/glow replaces extra color as the way to signal importance. |
| Bright violet accents | One lively hue keeps the dark palette from feeling flat or gloomy. |
| Darker footer | Adds a sense of "floor" and groups the legal/contact info. |

## Make it yours (just ask the AI in plain words)

- *"Make the card pure black instead of plum."*
- *"Increase the button glow / remove the glow for a flatter look."*
- *"Use my brand's accent color for the headline's second line and step numbers."*
- *"Add a real hero photo with a dark gradient overlay so white text stays readable."*
- *"Give me a light version of this same layout"* (→ that's essentially Template A).

## Before you send (in addition to the [universal checklist](README.md#universal-checklist-applies-to-all-5-designs))

- [ ] **Test dark mode in Gmail and Apple Mail** — confirm colors don't auto-invert into something ugly.
- [ ] **Test Outlook** — confirm the card is solid dark (not white) and white text is visible.
- [ ] Check the **logo chip** stays white/light everywhere; a dark logo on a dark card is invisible.
- [ ] Make sure body text isn't too faint — bump up transparency if it's hard to read on a phone outdoors.

---

*Template D of 5 · [Back to the prompt pack](README.md) · [See it live](../index.html)*
