# Marcia Collins — A Life Well Lived

> *"In every stroke of the pen, a prayer."*

A personal memoir website honouring the life and legacy of **Marcia Collins** (born 2 October 1936, London) — master calligrapher, woman of faith, devoted mother and grandmother, whose quiet influence has touched many lives over nine decades.

This website was created as a gift for Marcia on the occasion of her 90th year, presented at *An Evening of Memories, October 2026.*

---

## About This Site

A single-file, self-contained HTML memoir website built Mobile-First, fully responsive, and deploy-ready with no build step required. All 16 photographs are embedded directly as base64 — no external image hosting needed.

The site draws directly from **Marcia's own memoir**, recorded in her own words at *An Evening of Memories, 3 October 2026*, and presents her life across six chapters.

---

## The Six Chapters

### Part I — Roots & Origins
*From a premature birth in wartime London to a childhood in the fields of Essex*

| Section | Detail |
|---------|--------|
| Born into a World on the Edge of Storm | Charing Cross Hospital, 2 October 1936 — 4 pounds, fitting along a doctor's forearm |
| Those Dark Curly Locks | Marcia as a toddler in her pram, c.1937 |
| Mother & Child — A Garden, c.1937 | A hand-tinted photograph behind ornate glass — Marcia's mother holding her |
| Mayesbrook, 1939 | Aged three, already blonde as she described in her memoir — six months before the war |
| The Chair Left Behind | The unexploded bomb, the hurried departure, the chair she never got back |
| A Childhood Rooted in Field & Sky | Hornchurch, Essex, 1940 — hide-and-seek, hedgerows, and the seeds of a lifelong eye for beauty |

---

### Part II — Youth & Formation
*Wartime injury, Manchester, the scholarship, and twenty-one dresses*

| Section | Detail |
|---------|--------|
| A Child Who Needed Her Father | The infected finger, the rising temperature, the ward sister's daily report — and Dad recalled from France |
| Manchester, Grandma & Victory | Euston Station, Pendlebury Hospital, Grandma's canal, the bull at the door, and the 1945 street party |
| The Scholarship & Twenty-One Dresses | Romford County High School, the sewing machine rescue, and a lifetime of making things with her hands |

---

### Part III — Love & Family
*The cinema, the fountain, the wedding, and a life built at number 22*

| Section | Detail |
|---------|--------|
| Last to Fill the Row | Tony — met at the cinema, introduced by a family friend, last to fill the row |
| Tuesdays, Saturdays & a Fountain | The zoo, the borrowed company, and the proposal that wasn't quite a proposal — Southampton |
| 8th of May, 1965 — At Last | The Old Bailey, the long wait, and finally the wedding day |
| The Honeymoon | A week at Land's End — sunrise and sunset over the Atlantic |
| The Family She Built | Three generations gathered around Marcia and Tony |
| Number 22, Butterfield Road | The front door where they stood with their two daughters — where Marcia still lives today |
| A New Life Arrives | A newborn held with careful, certain hands — pure joy |
| Marcia — In Her Prime | A portrait, c.1970s–80s — the quiet confidence of a woman who knows exactly who she is |
| That Laugh — That Man | Tony writing, Marcia laughing — two people entirely sufficient to each other |
| Beside Still Waters | Tony's arms around Marcia by a river — a summer afternoon, entirely at peace |
| The Family Portrait | A formal black and white portrait, c. early 1970s |
| A Formal Evening | Black tie, floor-length gowns, chrysanthemums — an evening dressed for properly |

---

### Part IV — Trials & Turning Points
*Six words. No bitterness. Just grace.*

| Section | Detail |
|---------|--------|
| When Things Do Not Work Out | "Alas, my marriage proved to be a failure." — the Old Bailey, the long wait |
| Luckily, Father Had a Good Job | That single word BUT — a whole philosophy of life |

---

### Part V — Giving Back
*A cheque, a hospice, and a life of quiet service*

| Section | Detail |
|---------|--------|
| Three Hundred and Fifty Pounds | HSBC cheque, £350 to Countess Mountbatten House from Southampton Pops Orchestra, 16 May 2005 |

---

### Part VI — Her Legacy
*What she left in every stitch*

| Section | Detail |
|---------|--------|
| What She Left in Every Stitch | Twenty-one dresses made by hand for granddaughter Paula's holiday |
| A Circle Completed | Born at 4 pounds — decades later, she made a nightdress for a grandson born at the same weight |
| Closing Dedication | Ecclesiastes 9:10 — "Whatever your hand finds to do, do it with all your might" |

---

## Technical Specifications

| Property | Value |
|----------|-------|
| Architecture | Single-file HTML — no framework, no build step |
| Responsive | Mobile-First CSS with `@media (min-width: 900px)` breakpoints |
| Images | 16 photographs embedded as base64 (JPEG + PNG) |
| File size | ~15 MB |
| Fonts | Google Fonts — Playfair Display, EB Garamond, Inter |
| JavaScript | None |
| Dependencies | None (Google Fonts loaded via CDN) |
| Hosting | GitHub Pages |

---

## Files

```
/
├── index.html        ← Complete website (single self-contained file, ~15 MB)
└── README.md         ← This file
```

---

## How to View Locally

Open `index.html` in any modern web browser — no server or installation required.

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

1. Create a new GitHub repository named `marcia-collins-memoir`
2. Upload `index.html` and `README.md` to the root
3. Go to **Settings → Pages**
4. Under *Source*, select **Deploy from branch → main → / (root)**
5. Click **Save**

Live URL:
```
https://<your-github-username>.github.io/marcia-collins-memoir/
```

Deployment takes 1–2 minutes.

---

## Updating the Site

All content lives inside `index.html`. To update:

| What to change | Where in the HTML |
|----------------|-------------------|
| Any text | Find the section by its heading, edit the `<p>` tags |
| A photograph | Replace the `src="data:image/..."` with a new base64 string |
| A caption | Find the `fullbleed-img-caption` or `img-caption` near the image |
| Placeholder text (✏️ markers) | Search for `✏️` — placeholders await Marcia's own words |
| Colour palette | `:root` CSS variables at the top of `<style>` |

### Pending placeholders (marked ✏️ in the site)

These sections are awaiting confirmation from Marcia:

1. **Family gathering** — names of all family members and occasion
2. **New arrival, c.1970s** — who the baby is and the year
3. **Tony & Marcia at dinner** — occasion and year
4. **Tony & Marcia by the river** — location and year
5. **Formal family portrait** — names and year
6. **Formal evening** — occasion, names, and year
7. **HSBC cheque (Part V)** — Marcia's own story in her words

---

## Design

### Colour Palette

```css
:root {
  --cream:      #F7F3ED;   /* page background */
  --cream-mid:  #EDE7DC;   /* section alternates */
  --cream-dark: #D9CFBF;   /* borders */
  --ink:        #1C1813;   /* primary text & dark panels */
  --ink-mid:    #4A4035;   /* body text */
  --ink-light:  #8A7F72;   /* captions & labels */
  --gold:       #B8935A;   /* accent */
  --gold-light: #D4B483;   /* borders on gold panels */
  --gold-pale:  #F0E4CC;   /* quote card backgrounds */
  --white:      #FDFAF6;   /* text panels */
}
```

### Typography

| Role | Font |
|------|------|
| Headings & titles | Playfair Display (serif) |
| Body & quotes | EB Garamond (serif) |
| Labels & navigation | Inter (sans-serif) |

---

## Credits

| Role | Name |
|------|------|
| Subject | Marcia Collins |
| Memoir text | Marcia Collins — *An Evening of Memories, October 2026* |
| Website concept & build | Ambrose Cheng |
| Built with | Claude (Anthropic) |
| Photography | The Collins family |
| Hosting | GitHub Pages |

---

## Licence

This website is created for personal and family use in honour of Marcia Collins. All content — text, photographs, and design — belongs to the Collins family. Please do not reproduce or distribute without permission.

---

*"Whatever your hand finds to do, do it with all your might."*
— Ecclesiastes 9:10

*An Evening of Memories · October 2026*
