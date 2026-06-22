# Email template prompt pack — start here

This folder gives you **5 ready-to-use prompts** — one per design direction (A–E) from the
Bonjour Battle showcase. You don't need any coding or design knowledge. You **copy a prompt,
paste it into an AI assistant** (Claude, ChatGPT, Gemini, etc.), and it builds the email for you.

Each prompt also explains **what to consider** and **why**, so you learn a little about good
email/UI design while you use it.

> 🧭 **New here? Read this page first**, then open the template file you want:
> - [Template A — Editorial Light](template-A-editorial-light.md)
> - [Template B — Gradient Premium](template-B-gradient-premium.md)
> - [Template C — Minimal Centered](template-C-minimal-centered.md)
> - [Template D — Dark Editorial](template-D-dark-editorial.md)
> - [Template E — Event Ticket](template-E-event-ticket.md)

---

## How to use a prompt (3 steps)

1. **Open** the template file you like (links above). Find the box titled **"📋 The prompt — copy everything in this box."**
2. **Copy** the whole box and **paste it** into your AI assistant. Press send.
3. The AI returns a single HTML file. **Save it as `email.html`** and open it in your browser to preview. To send it, paste the HTML into your email tool (Mailchimp, Brevo, Zoho, etc.) using its "code/HTML" or "import HTML" option.

**Want a change?** Just ask in plain words: *"Make the button green,"* *"Use my logo at this link,"*
*"Change the prize to Rs 1,00,000,"* *"Make the headline bigger on mobile."* You don't edit code — you describe what you want.

---

## A 60-second glossary (so the prompts make sense)

| Word | What it means, plainly |
|------|------------------------|
| **Hero** | The big eye-catching area at the top (image or bold headline). |
| **Eyebrow** | The tiny label above a headline (here: *"Bonjour Battle · Season 1"*). |
| **CTA** | "Call To Action" — the main button you want people to click. |
| **Hex color** | A color written as `#41009A`. The `#` plus 6 characters = one exact color. |
| **Inline CSS** | Styling written directly on each element. Email needs this (explained below). |
| **Responsive** | The design re-flows to look good on a phone as well as a computer. |
| **Above the fold** | What people see before scrolling. Put the important stuff here. |
| **Alt text** | Words shown if an image fails to load. Important for email + accessibility. |
| **Visual hierarchy** | Making the most important thing look the most important (size, color, position). |
| **Whitespace** | Empty breathing room around things. More space = calmer, more premium. |

---

## The shared brand kit (every template uses this)

Give this to the AI as-is, or swap in your own brand. The prompts already include it, but here it is in one place:

**Brand:** Lingotran — *Bonjour Battle, Season 1*

**Colors**

| Role | Hex | Used for |
|------|-----|----------|
| Deep plum (darkest) | `#1A0B2E` | Footer background, darkest text |
| Brand purple (primary) | `#41009A` | Buttons, links, headings accent |
| Violet (bright accent) | `#7C4DFF` | Gradients, highlights |
| Coral (warm accent) | `#FF6B4A` | Eyebrow labels, small accents |
| Cream (page background) | `#E7E4DF` | The area around the email card |
| Soft purple tint | `#F0E6FF` | Highlight boxes (prize, step numbers) |
| Body text | `#444444` | Paragraphs |
| Muted text | `#666666` | Secondary/quiet text |

**Typography:** Nunito (a friendly, rounded sans-serif). Fallback: Helvetica, Arial, sans-serif.
Headlines are heavy (800), body text is medium (500).

**Logo:** `https://lingotran.com/media/logo.png`

**The content (same message in every design)**
- Eyebrow: **Bonjour Battle · Season 1**
- Headline: **You're in. Now let's begin.**
- Sub-text: *The French assessment course is open. Log in and finish your first lessons before assessment night on 24 June.*
- Button: **Log in and start learning →** → `https://learn.lingotran.com/bonjour-battle`
- Prize pool: **Rs 50,000** + a certificate for every student who completes the assessment.
- Details: **When** 24 June · 7:30 PM · **Format** Online · free to enter · **Level** Beginners welcome
- What to do next: 1) Log in and open the Bonjour Battle course. 2) Finish your lessons before 23 June. 3) Show up on assessment night, 24 June.
- Footer: Lingotran · info@lingotran.com · 96060 81499 · *View in browser* · *Unsubscribe* · © 2026 Lingotran Private Limited.

---

## Why email design is different from a website (read this once)

This is the single most useful thing to understand. **An email is not a web page.** Email apps
(especially Outlook) ignore a lot of modern code, so emails are built with older, sturdier techniques:

1. **Layout uses invisible tables, not modern CSS.** It looks dated, but it's the only thing that
   survives every inbox. *(The AI handles this — you don't have to.)*
2. **All styling is "inline"** (attached to each element) because many inboxes strip out a separate
   style section.
3. **Width ~600px.** The safe, classic width that fits every email app and phone.
4. **Real, hosted images** (with `https://` links and **alt text**), because email can't generate
   images from code reliably.
5. **One clear button.** Built "bulletproof" so it shows even when images are blocked.
6. **Dark mode + images-off** are realities — design so the message still reads with no images and
   on a dark background.

Every prompt in this pack already tells the AI to follow these rules, so your result is **actually
sendable**, not just pretty in a browser.

---

## Universal checklist (applies to all 5 designs)

Before you send any email built from these prompts, check:

- [ ] **One job per email** — is the main action (the button) obvious within 3 seconds?
- [ ] **Reads top-to-bottom** — headline → why it matters → button → details.
- [ ] **Works with images off** — the message still makes sense (text isn't trapped inside an image).
- [ ] **Readable on a phone** — text ≥14px, button easy to tap, no sideways scrolling.
- [ ] **Good color contrast** — dark text on light, or light text on dark. Nothing faint.
- [ ] **Every image has alt text** and the logo links to your site.
- [ ] **Links work** and go to the right place (test the button!).
- [ ] **Footer has** sender name, contact, *unsubscribe*, and *view in browser* (legally expected).
- [ ] **Subject line + preheader** set (the short text shown next to the subject in the inbox).
- [ ] **Send yourself a test** to Gmail, Outlook, and a phone before the real send.

---

*Part of the [Bonjour Battle email showcase](../index.html). Sendable HTML lives in [`/emails`](../emails); design-tool originals in [`/source`](../source).*
