# Invitation letter — clickable demos

A shareable digital invitation. Open the link → an invitation letter opens →
press inside to open the attached PDF document.

## ✨ Live link

Once GitHub Pages is enabled (see below), the invitation is live at:

**https://gracethy1405-wq.github.io/Invitation-Letter/**

Send that link to anyone — it opens straight away in their browser, no login or install needed.

## The pages

| File | Style | Document opens |
|------|-------|----------------|
| `index.html` | **Main invitation** — animated background, envelope reveal, confetti, live countdown, RSVP, add-to-calendar | In-page PDF viewer (desktop) / new tab (mobile) |
| `envelope.html` | Wax-sealed envelope → formal letter (cream + gold) | New browser tab |
| `ticket.html` | Event "admit one" pass with barcode (dark, modern) | New browser tab |
| `modern.html` | Split-screen card with big date block (light, clean) | In-page viewer |

`index.html` is what the live link shows. A working sample `invitation.pdf` is included so everything runs out of the box.

## Enable the live link (GitHub Pages)

1. The repo must be **public** for free GitHub Pages (the published page is public either way).
2. Repo **Settings → Pages**.
3. Under **Build and deployment**, set **Source = Deploy from a branch**, **Branch = `main` / `(root)`**, then **Save**.
4. Wait ~1 minute, then open the live link above.

## Make it yours

1. **Swap the document.** Replace `invitation.pdf` with your own file (keep the name, or change `DOC_URL` in `index.html`). To use a Google Doc, point the link at your share URL instead.
2. **Edit the wording.** Open `index.html` and change the title, date, venue and body text near the top of `<body>`. Update the `EVENT` and `TARGET` values in the script so the calendar link and countdown match your real date.
3. **Recolour.** Change the colour variables in the `:root { ... }` block at the top of `<style>`.
