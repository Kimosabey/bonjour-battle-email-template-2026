# Template E — Event Ticket

> 🆕 First time? Read the [prompt pack intro](README.md) first — it explains how to use these and what the words mean.

## At a glance

**The feel:** Playful and tangible. The email is shaped like a real event ticket — complete with a
dashed "tear here" perforation and little notch cut-outs on the sides.

**Best for:** Events, webinars, competitions, "your pass / your spot is confirmed" emails — when you
want the message to feel like something you *hold*.

**One-line description:** *A white ticket with a purple top stub ("Your entry pass"), then a dashed
perforation with side notches, then a ticket-stub strip of details.*

## What it looks like, top to bottom

1. A **purple top strip** ("the stub header") with the logo on a white chip and the words
   **"Your entry pass"** on the right.
2. The familiar **eyebrow + headline + paragraph**.
3. A **hero banner** (gradient placeholder).
4. The **purple button**.
5. A **prize box** (coral left bar on soft purple).
6. **The signature touch:** a **dashed perforation line** with two little **notch circles** cut into
   the left and right edges — exactly like tearing a ticket stub.
7. Below the tear, a **3-column "stub" strip** of details (When / Format / Level).
8. **"What to do next"** — three numbered steps.
9. **Footer** on deep plum.

---

## 📋 The prompt — copy everything in this box

```text
You are an expert email developer. Build me ONE complete, ready-to-send HTML email file called
"Event Ticket". It must look polished in Gmail, Apple Mail, and Outlook, and on mobile phones.

DESIGN DIRECTION — "Event Ticket":
Playful and tangible — the email is styled like a real event ticket. The signature elements are a
purple "entry pass" header strip at the top and a dashed PERFORATION line across the middle with two
small notch circles cut into the left and right edges (like a tear-off ticket stub). Below the tear is
a ticket-stub strip of event details.

BRAND KIT:
- Font: Nunito (load from Google Fonts), falling back to Helvetica, Arial, sans-serif.
  Headlines weight 800, body weight 500.
- Colors: deep plum #1A0B2E, brand purple #41009A, violet #7C4DFF, coral #FF6B4A,
  cream page background #E7E4DF, soft purple tint #F0E6FF, body text #444444, muted text #666666.
- Logo image: https://lingotran.com/media/logo.png (alt text "Lingotran").

LAYOUT (top to bottom), inside a white rounded card, max width 600px, centered on a cream #E7E4DF page:
1. A purple #41009A header strip spanning the full width: on the LEFT the logo on a small white
   rounded chip; on the RIGHT, small uppercase light-purple text "YOUR ENTRY PASS" (two lines).
2. Coral uppercase eyebrow "BONJOUR BATTLE · SEASON 1".
3. Headline in deep plum: "You're in." line break "Now let's begin." with the second line in brand
   purple #41009A. Then a short paragraph: "The French assessment course is open. Log in and finish
   your first lessons before assessment night on 24 June." (bold the "24 June").
4. A hero banner (~170px tall, rounded) filled with a 135-degree gradient from #41009A to #7C4DFF,
   with faint translucent circles and a label "Hero image · replace with hosted 1200×600".
5. A full-width "bulletproof" button: brand purple #41009A, white text, rounded 8px,
   "Log in and start learning →", linking to https://learn.lingotran.com/bonjour-battle. Under it a
   small muted line "Takes a minute to begin · the course closes 23 June".
6. A prize box: soft purple #F0E6FF background with a 4px coral #FF6B4A bar on the left edge, rounded
   on the right. Inside: tiny coral "PRIZE POOL", bold "Rs 50,000", then "Plus a certificate for every
   student who completes the assessment."
7. THE SIGNATURE PERFORATION: a horizontal dashed line across the ticket, with a small circle the SAME
   COLOR AS THE PAGE BACKGROUND (#E7E4DF) notched into the left edge and another into the right edge, so
   it looks like a tear-off line on a physical ticket.
8. Below the tear, a ticket-stub detail strip: 3 columns separated by thin vertical dividers, each with
   a small label and value: When = "24 June · 7:30 PM"; Format = "Online · free to enter";
   Level = "Beginners welcome". On screens under ~480px, stack the 3 columns into one (with thin
   horizontal dividers between them instead of vertical ones).
9. A "WHAT TO DO NEXT" label, then three numbered steps in small purple-tinted circles: 1) Log in and
   open the Bonjour Battle course. 2) Finish your lessons before 23 June. 3) Show up on assessment
   night, 24 June.
10. Footer on deep-plum #1A0B2E, light text: "Lingotran", then "info@lingotran.com · 96060 81499",
    then links "View in browser · Unsubscribe", then "© 2026 Lingotran Private Limited. You received
    this because you registered for Bonjour Battle Season 1."

TECHNICAL RULES (important — this is an EMAIL, not a web page):
- Use table-based layout (not flexbox/grid) so it survives Outlook.
- The perforation notch circles work by using small circle shapes filled with the page background color
  (#E7E4DF) positioned at the card's left and right edges. Keep a simpler fallback (a plain dashed line)
  in case an email app can't position the notches — the design must still look fine without them.
- Put ALL styling inline (keep a <style> block for the font + mobile tweaks).
- Max content width 600px; center the card on the cream background.
- Responsive: under ~480px, reduce side padding/font sizes and stack the 3-column detail strip into one
  column. No sideways scrolling.
- Every image needs alt text. The logo links to https://lingotran.com.
- Add a hidden preheader: "Your entry pass is ready — start the French course before 24 June."
- Strong contrast, tap-friendly spacing. Output ONE complete HTML file, no explanation around it.
```

---

## What makes this design work (the UI/UX considerations)

- **A metaphor makes it memorable.** Shaping the email like a ticket instantly communicates "this is
  your pass / you're confirmed" before anyone reads a word. Visual metaphors are a powerful shortcut.
- **The "Your entry pass" stub sets context** in the inbox preview — it frames the whole message.
- **The perforation is delight, not decoration for its own sake.** It reinforces the metaphor and
  visually *separates* the "message" half from the "details stub" half — form following meaning.
- **Graceful fallback matters.** Fancy touches like notch cut-outs can fail in strict email apps, so the
  prompt insists the design still looks good as a plain dashed line if the notches don't render. *Never
  let a nice-to-have flourish break the core layout.*
- **Stub = scannable facts.** The 3-column strip below the tear behaves like the detachable part of a
  real ticket — the at-a-glance "when/where/what."
- **Mobile re-flow.** On phones the 3 columns stack, and vertical dividers become horizontal — a small
  but important detail so it never looks squished.

## Why these choices

| Choice | Why it's there |
|--------|----------------|
| Purple "entry pass" header strip | Sets the ticket metaphor and confirmation tone immediately. |
| Dashed perforation + side notches | The signature delight that makes it unmistakably a "ticket." |
| Details placed below the tear | Mirrors a real stub — the part you'd keep — so it reads naturally. |
| Plain-line fallback for the tear | Keeps the email robust across inboxes that can't do the cut-outs. |
| Same content, different container | Proves the same message can feel like an "event" with the right framing. |

## Make it yours (just ask the AI in plain words)

- *"Add a fake barcode or a QR-code placeholder at the bottom of the stub."*
- *"Put a seat/ticket number like 'PASS #001' in the top strip."*
- *"Make the perforation vertical, splitting the ticket into left and right."*
- *"Change the entry-pass strip color to coral."*
- *"Add a calendar 'Add to Calendar' link near the When detail."*

## Before you send (in addition to the [universal checklist](README.md#universal-checklist-applies-to-all-5-designs))

- [ ] Check the **perforation notches** render in your main inboxes — if not, confirm the plain dashed
      line still looks clean (it should).
- [ ] The notch circles must match your **page background color** exactly, or the "cut-out" illusion breaks.
- [ ] On a **phone**, confirm the 3-column stub has stacked neatly and dividers switched to horizontal.
- [ ] In **dark mode**, make sure the white ticket and the notch color still read as a ticket (add a faint border if needed).

---

*Template E of 5 · [Back to the prompt pack](README.md) · [See it live](../index.html)*
