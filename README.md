# Chamila website (taste-skill redesign)

Open `index.html` through a small local server (the page uses JavaScript modules, which browsers block from a double-clicked file):

    cd chamila-website
    python3 -m http.server 8000
    # then open http://localhost:8000

Or upload the whole folder to Netlify Drop, Cloudflare Pages or GitHub Pages; it works there as is.

## Things to change before going live
- **WhatsApp number:** in `index.html`, near the bottom, set `const WHATSAPP = '';` to your number with country code and no + (for example `94771234567`). Left empty, WhatsApp asks the customer to pick a contact.
- **Prices:** the prices are placeholders I set. Change them in the range tiles and the order list (each row's `data-price` and the text beside it).
- **Domain:** once you have one, add `<link rel="canonical" href="https://your-domain/">` in the head.

The design system in `assets/` comes from taste-skill (MIT licence, see `assets/LICENSE-taste-skill.txt`).
