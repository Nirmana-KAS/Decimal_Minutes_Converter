<div align="center">

# ⏱️ Decimal Minutes Converter

**Divide 450 by any value and instantly see the answer as minutes and seconds.**

A tiny, fast, zero-dependency web calculator: one HTML file, no build step, no tracking.

[![Live Demo](https://img.shields.io/badge/demo-live-brightgreen?style=for-the-badge&logo=vercel)](https://YOUR-PROJECT.vercel.app)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](#)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](#)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](LICENSE)

</div>

---

## 📖 About

The page runs one fixed equation:

```
decimal minutes = 450 ÷ your value
```

It then turns the decimal-minute result into a readable **minutes + seconds** answer, so you never have to do the `× 60` conversion by hand.

> **Example:** 450 ÷ 500 = 0.9 decimal minutes = **0 minutes 54 seconds**

## ✨ Features

- ⚡ **Instant results**: type a value, press **Calculate** (or Enter)
- 🔢 **Decimal → minutes & seconds** conversion, rounded to the nearest second
- 🧾 **Full working shown**: decimal minutes (6 d.p.) and total seconds
- 🛡️ **Input validation**: only numbers greater than zero are accepted
- 🌙 **Dark, clean UI** that works on phones, tablets and desktops
- ♿ **Accessible**: labelled fields, live result region, error alerts
- 📦 **Zero dependencies**: a single self-contained HTML file (~4 KB)

## 🚀 Live Demo

👉 **https://YOUR-PROJECT.vercel.app** *(replace after your first Vercel deploy)*

## 🖼️ Screenshots

| Desktop | Mobile |
|:---:|:---:|
| ![Desktop screenshot](docs/screenshot-desktop.png) | ![Mobile screenshot](docs/screenshot-mobile.png) |

*Add your screenshots to a `docs/` folder with the names above.*

## 🧮 How It Works

| Step | Formula | Example (value = 500) |
|---|---|---|
| 1. Divide | `450 ÷ value` | `0.9` decimal minutes |
| 2. To seconds | `round(decimal × 60)` | `54` total seconds |
| 3. Split | `minutes = ⌊s ÷ 60⌋`, `seconds = s mod 60` | `0 min 54 s` |

## 🛠️ Usage

### Run locally

No install needed. Either:

- Double-click `decimal_minutes_converter.html` to open it in your browser, **or**
- Serve the folder locally:

```bash
npx serve .
# then open http://localhost:3000
```

### Use the calculator

1. Enter your value in **Second value** (must be greater than 0).
2. Press **Calculate**.
3. Read the result in minutes and seconds, with the full working below it.

## ☁️ Deploy to Vercel (free)

1. Push this folder to a new GitHub repository.
2. Sign in at [vercel.com](https://vercel.com) with GitHub (Hobby plan is free).
3. Click **Add New… → Project** and **Import** this repository.
4. Keep the defaults:
   - **Framework Preset:** `Other`
   - **Build Command:** *(leave empty)*
   - **Output Directory:** *(leave empty, root)*
5. Click **Deploy**. Your site is live at `https://<project-name>.vercel.app`.

Every later push to the `main` branch redeploys automatically.

`vercel.json` serves `decimal_minutes_converter.html` at the site root (`/`) and adds basic security headers.

## 📁 Project Structure

```
Decimal_Minutes_Converter/
├── decimal_minutes_converter.html   # The calculator (HTML + CSS + JS)
├── vercel.json                      # Vercel config (root rewrite + headers)
├── README.md
├── LICENSE
└── .gitignore
```

## 🤝 Contributing

Issues and pull requests are welcome. For larger changes, please open an issue first to discuss what you'd like to change.

## 📄 License

Released under the [MIT License](LICENSE) © 2026 Shehan Nirmana.

<div align="center">

Made with ❤️ by **Shehan Nirmana**

</div>
