# Shivay Tours & Travels — v14

This version is rebuilt around the supplied mobile reference: dark navy/gold palette, temple + mountain hero, one primary Book a Vehicle action, Local/Temple/Family trips, and a two-category fleet that stays closed until the customer taps Sedan or 7 Seater.

## Run locally
1. Extract the ZIP and open the `Shivay_Tours_Travels` folder in VS Code.
2. Open Terminal in that exact folder (the folder containing `package.json`).
3. Run `npm install` once.
4. Run `npm start` or double-click `start.bat` on Windows.
5. Open the localhost URL printed by the terminal (normally `http://localhost:3000`).
6. Admin: `http://localhost:3000/admin.html`.

Do not use VS Code Live Server for the booking flow; the Node backend must be running.

## Fleet image sources
Sedan and Innova images use Wikimedia Commons remote image URLs so the site displays real vehicle photographs instead of illustration/sticker assets. Ertiga uses the supplied high-resolution local photographs in `images/ertiga/`.

The hero visual is based on the user's supplied Shivay Tours & Travels reference image so the mobile composition matches the requested look.

## Production notes
Before public launch, replace the demo/admin credentials in `.env`, configure a production database and HTTPS, and verify the WhatsApp business number. Remote vehicle images should ideally be downloaded/licensed and stored locally for production reliability.


## V15 visual fixes
- The hero reference artwork is rendered as a single source image so the logo, title, trust badges, central Book a Vehicle CTA and vehicle lineup are not duplicated by HTML overlays.
- The extra top-right Book a Vehicle artwork was removed from the hero image; the central CTA is the only visible Book a Vehicle button.
- Hero artwork was upscaled to 3840px wide with high-quality resampling and mild sharpening for cleaner mobile/desktop presentation.
- The bottom CTA now uses one reference artwork only; duplicate HTML text/WhatsApp layers were removed. A transparent clickable hotspot remains over the WhatsApp area.
- The menu remains functional through the transparent hamburger hotspot in the hero.

## V16 layout changes
- Made for Real Travel card compacted and its overlapping outline removed.
- Our Fleet moved above Why Shivay.
- Why Shivay changed to clean point-style notes instead of four cards.
- Bottom Let's Plan / WhatsApp CTA strip removed.
- Hamburger menu is vertical and includes a Close Menu button.
