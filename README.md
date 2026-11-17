# Exclusive Real Estate Roadshow

A private invitation for the Golden Palm Real Estate roadshow with Royal Development Holding.

## Run

```bash
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

The guest desk is at [http://localhost:3000/admin](http://localhost:3000/admin). The desk password stays in `.env.local` (`ADMIN_PASSWORD` and `SESSION_SECRET`) and is not published here.

GitHub Pages serves `index.html` at the site root. That file is the public invitation. This readme is for running the project on a computer.

## What the desk controls

Venue, date, Gulf Standard Time, map pin, WhatsApp, phone, email, the public link used by the QR code, photographs, and the invitation copy. Guest replies are stored in `data/roadshow.db`. The desk can search, filter attendance, remove a mistaken reply, and export Excel.

The evening is set to 6:00–9:00 PM GST until you replace it with the exact time.

WhatsApp and the enquiry lines stay hidden until a number or email is saved.

To let phones on the same network open the invitation:

```bash
npm run dev -- -H 0.0.0.0
```

Then set the public invitation link in the desk to that address so the QR code points at it.

## Photographs

The opening and closing images are contemporary residential photographs for the invitation. Replace `public/images/hero.jpg` and `public/images/closing.jpg`, or point the desk at another `/images/` file or https link.

The Royal Development Holding and Golden Palm Real Estate marks are the supplied logos, unchanged.
