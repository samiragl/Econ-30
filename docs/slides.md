# Econ 30 Lab: HTML capstone page + Cursor + Vercel

**TA prep deck** (Markdown source — edit here, then sync to `slides.html` if you maintain both)

---

## Slide 1 — Title

**Preparing the web capstone assignment**

HTML page · Cursor (including Plan Mode) · Vercel hosting

Stanford Econ 30 · Lab prep for TAs

---

## Slide 2 — Why this assignment

**One public URL = anyone can open your project**

- Communicate context, literature, and your research question clearly.
- Practice packaging work for non-specialists (a useful skill beyond this class).
- Learn a simple **publish** step: local file → hosted page.

---

## Slide 3 — What students turn in

**Deliverables (from the assignment)**

1. A simple **`index.html`** webpage with:
   - **Project title**
   - **Student name**
   - **Description**: context, literature, research question
   - **One interactive element** (placeholder or figure is OK if the full interaction is not ready)
2. A **live link** (page hosted on **Vercel**, publicly accessible)

**Important:** They may use **Cursor** as a collaborator; **Plan Mode** is recommended for breaking the work into steps.

---

## Slide 4 — What HTML is (in one minute)

**HyperText Markup Language = structure + content**

- **Structure:** `html`, `head`, `body`, headings, sections, paragraphs.
- **Embedded media:** images, links to papers or data.
- **“Interactive” in the assignment sense:** anything that responds or invites action—button, collapsible section, form, chart placeholder, etc.

You are **not** teaching a full web course; you are mapping these ideas to **their** capstone page.

---

## Slide 5 — Minimum viable page layout

**Suggested regions (wireframe)**

```
[ Project title + name ]
[ Context / motivation     ]
[ Literature (short)       ]
[ Research question        ]
[ Interactive / figure     ]
[ Optional: links, footer  ]
```

**Typical tags:** `h1`–`h3`, `p`, `section`, `figure`, `img`, `a`, `details`/`summary`, or a simple `button`.

---

## Slide 6 — Interactive element (keep it small)

**Acceptable examples**

- **`details` / `summary`:** expandable “Methods” or “Data” blurb.
- **Placeholder:** “Chart will go here” inside a bordered `div` or `figure`.
- **Simple form** that does not need a server yet (assignment is static HTML).
- **Button + short script** (optional) for a minimal demo—only if you want to show JS.

**Message:** A **placeholder** satisfies the requirement if the real interaction is still in progress.

---

## Slide 7 — Working with Cursor (workflow)

**Sketch → describe → build → check → deploy**

1. Rough **sketch** (on paper or in chat): sections and order.
2. **Prompt** with **content** (what to say) **and** **design** (layout, fonts, colors, vibe).
3. Cursor proposes **structure and code**; student **reviews** and edits.
4. **Open** `index.html` in a browser locally.
5. **Host** on Vercel; share URL.

**You (intent)** → **Cursor (plan + code)** → **You (review + test)** → **Vercel (publish)**

---

## Slide 8 — Plan Mode

**When to use it**

- First time combining **HTML + deploy**.
- Several steps at once (structure, style, placeholder interaction, Vercel prep).

**Example ask:** “Break this into steps: (1) semantic HTML skeleton, (2) simple CSS for readability, (3) one interactive placeholder, (4) checklist for deploying a static site to Vercel.”

Students implement **step by step** instead of one vague “make my website” request.

---

## Slide 9 — Prompts: weak vs strong (part 1)

**Weak**

> “Make my website for my capstone.”

**Why it fails:** No sections, no audience, no design, no file structure.

**Stronger (shape)**

> “Create a single-file **`index.html`** for my economics capstone. Sections: title and my name; motivation; 3–5 sentence literature summary; research question in bold; one `details`/`summary` block for extra detail. Design: clean academic look, max width ~720px, readable system fonts, plenty of whitespace.”

---

## Slide 10 — Prompts: fill-in for their project

**They should paste (and customize) something like:**

- **Content:** Working title; name; 1 paragraph context; 2–4 key references (names or links); precise research question.
- **Design:** Single column vs two columns; color preferences; formal vs friendly tone; optional image paths if they have figures.
- **Tech constraints:** “Single `index.html`” vs “folder with `index.html` + `styles.css` + images/” (both are fine if deployment instructions match).

**TA tip:** Ask them to attach a **rough outline** in the same message as the design preferences.

---

## Slide 11 — Before Vercel: local check

**Static site = no server required for this homework**

- Open **`index.html`** in Chrome / Edge / Firefox (double-click or “Open with”).
- Fix **broken image paths** (often wrong relative path).
- File name matters: typically **`index.html`** (lowercase) at the folder Vercel treats as root.

If it looks wrong locally, hosting will not fix it.

---

## Slide 12 — Hosting on Vercel (pick one primary path)

**Goal:** a **production URL** anyone can open.

**Common path A — Git + Vercel**

- Push project to GitHub (or similar).
- Vercel: New Project → import repo → framework preset **Other** / static if asked.
- Ensure project **root** contains `index.html` (or configure root directory).

**Common path B — Vercel drop / dashboard upload** (if available in your workflow)

- Use whatever the course documentation standardizes; **one** path reduces confusion.

**Redeploy:** after changes, push again (Git path) or trigger redeploy from dashboard.

---

## Slide 13 — Common pitfalls

| Issue | What to check |
|--------|----------------|
| Blank site | Wrong root folder; `index.html` missing or misnamed |
| Images broken | Paths relative to `index.html` |
| Old version live | Did they push / redeploy after edits? |
| Cursor over-scoped | Remind: static page + one interactive **or** placeholder |

---

## Slide 14 — Live session: optional co-build

**Recommended:** 10–20 minutes building **one toy example** together (fake title, placeholder figure—not 30 different capstones).

- Use a **scripted prompt** you prepared in advance.
- Students **mirror** the same prompt or **watch then repeat** in lab—state which you expect.
- **Backup:** short recording + a known-good deployed URL if Vercel or logins fail live.

---

## Slide 15 — Worksheet (student-facing)

**My initial prompt (draft)**

**Content I will include:**  
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

**Design I want (layout, fonts, colors, tone):**  
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

**Plan Mode steps I will ask for:**  
1. _ _ _ _ _ _ _ _ _ _  
2. _ _ _ _ _ _ _ _ _ _  
3. _ _ _ _ _ _ _ _ _ _

---

## Slide 16 — Summary & office hours

**Checklist for students**

- [ ] `index.html` with title, name, description (context, literature, RQ), interactive or placeholder  
- [ ] Tested locally in a browser  
- [ ] Deployed; **public URL** submitted  

**Useful OH prompts**

- “Paste your **Cursor plan**.”  
- “Paste your **Vercel** deploy log or screenshot.”  
- “Does your URL work on **phone** / incognito?”

**End**

---

**Deck locations**

- **Reveal (recommended for presenting):** [`slides/index.html`](../slides/index.html) — see [`slides/README.md`](../slides/README.md) for print/PDF and optional Vercel hosting.
- **Print-friendly single file:** [`docs/slides.html`](slides.html) (scroll or browser Print).
- **Locked outline:** [`docs/deck-outline.md`](deck-outline.md)
- **Vercel script (~2–3 min):** [`docs/vercel-walkthrough-script.md`](vercel-walkthrough-script.md)
- **Live co-build prompt:** [`docs/live-cobuild-prompt.md`](live-cobuild-prompt.md)
