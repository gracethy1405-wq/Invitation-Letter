# Invitation letter — clickable demos

Three self-contained invitation pages. Each one is the same flow:

**press the link → an invitation letter opens → press inside to open the PDF / document**

No build step, no server. Just double-click an `.html` file to open it in your browser.

## The three creative layouts

| File | Style | How the document opens |
|------|-------|------------------------|
| `envelope.html` | Wax-sealed envelope that flips open into a formal letter (cream + gold) | Opens the PDF in a **new browser tab** |
| `ticket.html` | Event "admit one" pass with perforated stub + barcode (dark, modern) | Opens the PDF in a **new tab** |
| `modern.html` | Split-screen card with a big date block (light, clean) | Opens the PDF **inside the page** in a built-in viewer, with a Download button |

A working sample `invitation.pdf` is included so all three run out of the box.

## Make it yours

1. **Swap the document.** Replace `invitation.pdf` in this folder with your own file (keep the name, or change the `href` / `openDoc(...)` path in the HTML — search the file for `invitation.pdf`).
   - To point at a **Google Doc** instead, change the link to your share URL, e.g.
     `href="https://docs.google.com/document/d/XXXX/edit"`.
2. **Edit the wording.** Open the `.html` in any text editor and change the title, date, time, venue, and body text — they're plain text near the top of the `<body>`.
3. **Recolour.** Each file has a `:root { ... }` block at the top of `<style>`; change the colour variables there.

## Sending it to guests

- **Email a single file:** attach the `.html` *and* the `.pdf`, or zip the folder.
- **Host a real link:** drop this folder on any static host (GitHub Pages, Netlify, your web server) and share the URL to `envelope.html` (or whichever layout you like).

> Tip: the `modern.html` in-page viewer needs the PDF served over `http(s)` to embed; opened as a local `file://`, some browsers block the embedded frame — use `envelope.html`/`ticket.html` (new-tab) for pure local/offline use.
