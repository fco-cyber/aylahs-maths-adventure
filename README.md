# 🧮 Aylah's Maths Adventure

A friendly, colourful **Grade 4 maths practice app** — built to help a 9-year-old learn
place value, number lines, skip counting and Australian money, at her own pace, on her own.

It's a single self-contained web app (no build step, no accounts, no tracking) that runs in
any modern browser and can be **installed on a tablet or phone** to work **offline**.

**Live site:** `https://fco-cyber.github.io/aylahs-maths-adventure/`
*(the address becomes active once you finish the steps in “Put it online” below)*

---

## ✨ What's inside

Eight activities, each with self-checking, gentle hints, rewards (⭐ + badges) and an
Australian read-aloud voice:

- **Place Value Builder** — build 4-digit numbers and watch the value, words and blocks update
- **Say the Number** — practise reading numbers out loud
- **Expanded Form** — break numbers apart (9000 + 600 + 50 + 3) and put them back together
- **Rename Numbers** — e.g. 9,653 = 96 hundreds and 53 ones
- **Biggest & Smallest** — the playing-card game
- **Skip Counting** — a rolling odometer, counting by 10s / 100s / 1000s
- **Number Line** — *read it*, *estimate*, *count to it*, and *watch the jumps*
- **Money** — count Australian coins and notes, and work out change

Four themes to choose from (🌈 Rainbow · 🐾 Pets · 🪐 Space · 🐬 Ocean) and a **Voice
settings** panel to control talking speed, pitch and the pause between parts.

---

## 🚀 Put it online (GitHub Pages)

This deploys the **same way** as `fco-cyber.github.io/playing-with-numbers` — a GitHub Pages
*project site* served straight from the repository. No workflow or build step needed.

### 1. Create the repository
1. On GitHub, click **New repository**.
2. Name it **`aylahs-maths-adventure`** (any name works — it becomes part of the web address).
3. Choose **Public**, then **Create repository**.

### 2. Add these files
**Easiest (browser):** on the new repo page choose **uploading an existing file**, then drag in
**everything inside this folder** (keep the `icons` folder together) and **Commit changes**.

**Or with Git:**
```bash
cd aylahs-maths-adventure
git init
git add .
git commit -m "Aylah's Maths Adventure"
git branch -M main
git remote add origin https://github.com/fco-cyber/aylahs-maths-adventure.git
git push -u origin main
```

### 3. Turn on Pages
1. In the repo, go to **Settings → Pages**.
2. Under **Build and deployment → Source**, choose **Deploy from a branch**.
3. Set **Branch** to **`main`** and the folder to **`/ (root)`**, then **Save**.
4. Wait about a minute, then open:
   **`https://fco-cyber.github.io/aylahs-maths-adventure/`**

That's it. 🎉 Every time you push a change to `main`, the site updates automatically.

---

## 📲 Install it on a tablet or phone

Once the site is live, open the address above in the browser and add it as an app:

- **iPad / iPhone (Safari):** Share button → **Add to Home Screen**
- **Android / Chrome:** menu (⋮) → **Install app** / **Add to Home screen**

It then opens full-screen with its own icon and **works without internet** after the first visit.

---

## 💻 Run it on your own computer

- **Quickest:** double-click `index.html`. Everything works except the “install / offline”
  feature (browsers only allow that over a web address, not a local file).
- **Full experience:** from this folder run a tiny local server and open the address it prints:
  ```bash
  python3 -m http.server 8000
  ```
  then visit `http://localhost:8000/`.

---

## 📁 What's in this folder

```
aylahs-maths-adventure/
├── index.html              ← the whole app
├── manifest.webmanifest    ← makes it installable (name, icons, colours)
├── service-worker.js       ← offline caching
├── favicon.png             ← browser-tab icon
├── icons/                  ← app icons (home-screen, etc.)
├── .nojekyll               ← tells GitHub Pages to serve files as-is
├── LICENSE
└── README.md
```

---

## 🛠️ Notes

- Built with plain HTML, CSS and JavaScript — no frameworks, no build tools, nothing to install.
- Fonts (Fredoka + Nunito) load from Google Fonts on the first visit and are then cached for
  offline use; if they can't load, the app falls back to friendly rounded system fonts.
- Progress (stars, badges, chosen theme and voice settings) is saved on the device.
- Aligned to the Victorian / Australian Curriculum Grade 4 number strand.

---

Made with ❤️ for Aylah • Grade 4 Maths • Melbourne, Australia 🇦🇺
