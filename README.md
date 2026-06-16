# Dr. Shefali Maydeo — Portfolio

A creative, single-page portfolio website for **Dr. Shefali Maydeo**, an
Occupational Therapist, Trainer and Center Head based in Mumbai, India, who
supports adults with intellectual and developmental disabilities through skill
development, vocational training and community inclusion.

> *"Creating pathways for independence and meaningful participation in society."*

## ✨ Highlights

- **Warm, healing aesthetic** — a custom palette of sage teal, warm coral and
  gold, with organic blob backgrounds and a hand-drawn feel.
- **Fully self-contained** — pure HTML, CSS and vanilla JavaScript. No build
  step, no frameworks, no external image dependencies. All artwork is inline SVG.
- **Sections**: Hero · About · Experience timeline · Skills · Education ·
  Credentials & community · Contact.
- **Interactive touches** — scroll progress bar, scroll-reveal animations,
  animated stat counters, active-section nav highlighting, a rotating monogram
  portrait and an infinite values marquee.
- **Accessible & responsive** — semantic HTML, skip link, keyboard-friendly
  mobile menu, visible focus styles, strong colour contrast, and full
  `prefers-reduced-motion` support. (Accessibility felt especially fitting for a
  disability-inclusion professional.)

## 📁 Structure

```
.
├── index.html            # All page content
├── assets/
│   ├── css/style.css      # Styling, layout, animations, responsive rules
│   ├── js/main.js         # Nav, scroll reveal, counters, progress bar
│   └── favicon.svg        # Monogram favicon
├── .nojekyll              # Lets GitHub Pages serve files as-is
└── README.md
```

## 🚀 View it locally

It's a static site — just open `index.html` in a browser, or serve the folder:

```bash
# Python 3
python3 -m http.server 8000
# then visit http://localhost:8000
```

## 🌐 Deploy on GitHub Pages

1. Push this branch to GitHub.
2. In the repository, go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select this branch and the **`/ (root)`** folder, then **Save**.
5. Your site goes live at `https://<username>.github.io/<repo>/`.

## 🚂 Deploy on Railway

This repo ships ready for [Railway](https://railway.com). A tiny, dependency-free
static server (`server.js`) serves the site and binds to Railway's `$PORT`;
`railway.json` pins the build/start config.

**From the Railway dashboard (recommended):**

1. Go to [railway.com/new](https://railway.com/new) → **Deploy from GitHub repo**.
2. Pick this repository and set the branch to **`shefali`**.
3. Railway auto-detects Node (via `package.json`), builds with Nixpacks, and runs
   `node server.js` (from `railway.json`). No extra settings needed.
4. Open the service → **Settings → Networking → Generate Domain** to get a public URL.

**From the Railway CLI (local machine):**

```bash
npm i -g @railway/cli
railway login
railway init            # create a new project
railway up              # build & deploy the current directory
railway domain          # generate a public URL
```

> `$PORT` is provided by Railway automatically — no env vars are required.

## ✏️ Customising

- **Content** lives in `index.html` (text is easy to find by section).
- **Colours, fonts and spacing** are CSS custom properties at the top of
  `assets/css/style.css` (`:root { ... }`).
- To swap the monogram for a real photo, replace the `.portrait__inner` block in
  `index.html` with an `<img>` and adjust the `.portrait` styles.

## 📇 Contact

- **Email:** maydeo.shefali@gmail.com
- **Phone:** +91 90226 42431
- **LinkedIn:** [in/shefali-maydeo](https://www.linkedin.com/in/shefali-maydeo)
- **Location:** Mumbai, India

---

Built from Dr. Shefali Maydeo's professional résumé. Fonts: *Fraunces* &amp;
*DM Sans* via Google Fonts.
