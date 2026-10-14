# AMAZON CAFE Website

A responsive, single-page website for AMAZON CAFE, Sherpur Sadar, Sherpur, Bangladesh.
Contact: khansaarrahman7@gmail.com

## Files
- `index.html` - the whole site (HTML, CSS and JavaScript in one file)
- `README.md` - this guide

## How to view
Unzip and open `index.html` in any browser. No build step or install needed.
Fonts (Google Fonts) need internet; offline, the site uses Georgia and system fonts.

## How to edit content
Open `index.html` in a text editor and find the block marked `// ===== EDITABLE CONTENT =====` near the bottom.

- `EMAIL` - the address that receives orders and contact messages
- `MENU` - each item is `[category, name, description, price in ৳, emoji]`
- `OFFERS` - each offer is `[emoji, title, description, "Price | Valid date"]`
- `GALLERY` (`GAL`) - `[emoji, caption]`
- `REVS` - `[customer name, stars 1-5, comment]`

All menu items, prices, offers and reviews are SAMPLES. Replace them with real,
confirmed information before publishing. Do not show offers or discounts that
are not real.

Other things to update by hand:
- Opening hours (Contact section, "Opening hours: add yours here.")
- Colors: change the variables at the top of the `<style>` block (`--gold`, `--bg`, `--cream`, etc.)

## Adding real photos
The site currently uses emoji and drawn illustrations instead of photos.
To use your own photos:
1. Put images in an `images/` folder next to `index.html`.
2. For a menu card, replace the emoji `<span>` in the card template with
   `<img src="images/latte.jpg" alt="Latte" style="width:100%;height:100%;object-fit:cover">`.
3. Do the same for the gallery buttons and the About section.

## How orders work
"Order Now" buttons and the contact form open the visitor's email app with a
pre-filled message to the EMAIL address. There is no server or payment system.
For online ordering later, connect a service such as a form backend or WhatsApp link.

## Hosting
Upload the folder to any static host (Netlify, Vercel, GitHub Pages, Cloudflare Pages).

## Features
Animated canvas background (beans, particles, waves, glow), animated SVG coffee cup
with steam, sticky navigation with mobile menu, category filters, offer cards,
gallery with lightbox, review cards, and reduced-motion support.
