# Live co-build — scripted Cursor prompt (toy capstone)

Use this in section after slides **7–8** (Cursor + Plan Mode). Build a **fake** page so students see workflow without merging 30 different capstones.

---

## Setup (you say aloud)

“Watch the screen. I’m creating a **sample** project named **Econ 30 Sample Capstone**—you’ll replace this with your real title later. I’ll use **Plan Mode** first, then accept the plan and implement step one.”

---

## Plan Mode — first message (paste into Cursor)

```text
I am a TA demo for an undergraduate economics class. Help me build a single static webpage for a TOY capstone (not real research).

Use Plan Mode: list concrete steps first, then we'll implement.

Requirements for index.html:
- Title: "Econ 30 Sample Capstone"
- Author line: "Jane Doe (demo)"
- Sections with placeholder text: Motivation; Short literature summary (3 sentences); Research question in bold
- One interactive-style element that works without a backend: use HTML details/summary titled "Extra detail" with 2 short paragraphs inside
- Clean academic layout: max-width ~720px, centered, readable system fonts, comfortable spacing
- Single file index.html with minimal embedded CSS in a style tag (no build tools)

Do NOT invent real citations or statistics—use obvious placeholders like "Author (Year)" and "X% (illustrative only)."
```

---

## After the plan appears

1. Confirm steps match: skeleton → styles → details/summary → optional polish.  
2. Ask Cursor to **implement step 1 only**, then **open `index.html` in the browser** and narrate what you see.  
3. Iterate for remaining steps or accept full file if time is short.

---

## Fallback if time or network fails

- Show a **prerecorded** 3-minute clip of the same flow.  
- Display a **known-good** deployed URL (your rehearsal deploy) and walk through the HTML in the editor for 2 minutes.

---

## Optional — mirror vs watch

**Mirror:** “Paste the same Plan Mode message when I say go—don’t customize yet.”  
**Watch then repeat:** “Take notes; you’ll do this in lab with your real content.”

State which mode you chose at the start of the activity.
