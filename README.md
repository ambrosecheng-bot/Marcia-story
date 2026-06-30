# Marcia Collins — A Life Well Lived

> *"In every stroke of the pen, a prayer."*

A personal memoir website honouring the life and legacy of **Marcia Collins** (born 1936) — master calligrapher, woman of faith, and teacher whose quiet influence has touched many lives over nine decades.

https://ambrosecheng-bot.github.io/Marcia-story/

---

## About This Site

This is a single-file, self-contained HTML website created to record and present the life story of Marcia Collins. It is designed to be simple to host, easy to maintain, and beautiful to read — a lasting digital memorial that can be shared with family, friends, and all who have been touched by her life.

The site is structured around six chapters of her life:

| Chapter | Title |
|---------|-------|
| Part I | Roots & Origins |
| Part II | Youth & Formation |
| Part III | Love & Family |
| Part IV | Trials & Turning Points |
| Part V | The Art of Calligraphy |
| Part VI | Her Legacy |

---

## Files

```
/
├── index.html        ← The complete website (single file, self-contained)
└── README.md         ← This file
```

> **Note:** The portrait photograph is embedded directly inside `index.html` as a base64-encoded image, so the site requires no external image files or assets to run.

---

## How to View Locally

Simply open `index.html` in any modern web browser — no server, no dependencies, no installation required.

```bash
# macOS
open index.html

# Windows
start index.html

# Linux
xdg-open index.html
```

---

## How to Deploy on GitHub Pages

1. **Create a new GitHub repository** (e.g. `marcia-collins-memoir`)
2. **Upload both files** — `index.html` and `README.md` — to the root of the repository
3. Go to **Settings → Pages**
4. Under *Source*, select **Deploy from a branch**
5. Choose **main** branch and **/ (root)** folder
6. Click **Save**

Your site will be live at:
```
https://<your-github-username>.github.io/marcia-collins-memoir/
```

GitHub Pages deployment typically takes 1–2 minutes.

---

## How to Rename the File

GitHub Pages expects the main file to be named `index.html`. If your file is currently named `marcia_memoir.html`, rename it before uploading:

```bash
mv marcia_memoir.html index.html
```

---

## Customisation Guide

All content can be edited directly inside `index.html` using any text editor (Notepad, TextEdit, VS Code, etc.).

| What to change | Where to find it in the HTML |
|----------------|------------------------------|
| Site title in browser tab | `<title>` tag |
| Name in navigation bar | `.nav-logo` text |
| Main headline | `<h1 class="hero-title">` |
| Subtitle / description | `<p class="hero-desc">` |
| Birth year & meta data | `.meta-value` spans |
| Quote card text | `.quote-body` and `.quote-attr` |
| Portrait photo | Replace the `src="data:image/png;base64,..."` with a new base64 image or a file path |
| Chapter names | `.ch-title` spans in the footer strip |
| Colour palette | `:root` CSS variables at the top of `<style>` |

### Colour Variables

```css
:root {
  --cream:      #F7F3ED;   /* page background */
  --ink:        #1C1813;   /* primary text */
  --gold:       #B8935A;   /* accent colour */
  --white:      #FDFAF6;   /* card / text panel background */
}
```

---

## Replacing the Portrait Photo

To use a local image file instead of the embedded base64 image:

1. Place your photo (e.g. `marcia.jpg`) in the same folder as `index.html`
2. In `index.html`, find the `<img>` tag inside `.hero-photo`
3. Replace the long `src="data:image/png;base64,..."` with:

```html
<img src="marcia.jpg" alt="Marcia Collins" />
```

---

## Technology

- Pure HTML5 + CSS3 — no JavaScript frameworks, no dependencies
- Fonts loaded from Google Fonts: [Playfair Display](https://fonts.google.com/specimen/Playfair+Display) + [EB Garamond](https://fonts.google.com/specimen/EB+Garamond) + [Inter](https://fonts.google.com/specimen/Inter)
- Portrait image embedded as base64 (no external image hosting required)
- Fully responsive layout (desktop-first; mobile optimisation can be added)

---

## Credits

- **Subject:** Marcia Collins — Master Calligrapher
- **Website concept & design:** Ambrose Cheng
- **Built with:** Claude (Anthropic)
- **Hosted on:** GitHub Pages

---

## Licence

This website is created for personal and family use. All content — text, images, and design — belongs to the Collins family. Please do not reproduce or distribute without permission.

---

*"Whatever your hand finds to do, do it with all your might."*
— Ecclesiastes 9:10
