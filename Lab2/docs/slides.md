---

marp: true
theme: default
paginate: true
size: 16:9
header: "Econ 30 -- Lab 2"
style: |
  section {
    font-family: 'Segoe UI', 'Helvetica Neue', Arial, sans-serif;
  }
  h1 {
    color: #1a1a1a;
    border-bottom: 3px solid #8C1515;
    padding-bottom: 8px;
  }
  h2 {
    color: #2e2e2e;
  }
  code {
    background: #f0f0f0;
    border-radius: 4px;
    padding: 2px 6px;
  }
  table {
    font-size: 0.85em;
  }
  blockquote {
    border-left: 4px solid #8C1515;
    color: #555;
    font-style: italic;
  }
  section.title {
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
  section.title h1 {
    border-bottom: none;
    font-size: 2.5em;
  }
  section.title h2 {
    font-weight: normal;
    color: #666;
  }
  section.section-break {
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    background: #f8f8f8;
  }
  section.section-break h1 {
    font-size: 2em;
    border-bottom: none;
  }
  section.section-break h2 {
    font-weight: normal;
    color: #8C1515;
  }
---

<!-- _class: title -->
<!-- _paginate: false -->

# Building a Knowledge Base

## Econ 30 -- Lab 2

### Samira Gholami

Spring 2026

---
# Any questions / feedback?
 
- Was everyone able to install Cursor and activate the student account?


- Let me show you quickly something about usage.


----

# Today

We will learn how to:

- Organize readings and notes systematically
- Use Cursor to summarize and extract ideas
- Build a connected knowledge base
- Retrieve and reuse information

---
# Step 1: Create Folder Structure

First, create a folder named `knowledge base` in your project root.
Download the cursorrule file from Canvas (under section)

Then create the following structure:

```bash
knowledge-base/
  raw/
  cursorrule
```

---

# Step 2: Add Materials to `raw/`

In `knowledge-base/raw/`, from your reading list add:

- PDFs
- articles and reports
- class notes and reflections

If you have many files, organize with subfolders:
- `articles/`
- `papers/`
- `notes/`


---
# Step 3: Let's review `cursorrules`

Open `knowledge-base/` in Cursor. Let's take 5 minutes to read cursorrule. 

- Whenever you ask the agent to do something, it first reads the `cursorrule` file  
- The file tells the agent how to behave and structure its output  
- You can modify it or create your own — this is just a template  

---

# Step 4: Trying Cursorrule

Ask Cursor in the agent mode:

```text
There are some new papers in Raw folder. set everything up as described in .cursorrules.
```

Check:
- structure and properties are correct
- tags use `[[...]]`
Feel free to add your comments for one paper.

---

# Check your Summary and Concept folders

```markdown
---
title:
sources:
related: []
last_updated:
tags: []
add_property:
---

## Summary
3-4 sentence explanation

## My Comment

```
---

# Step 5: Install and Open Obsidian

Choose "Open folder as vault" and select `Wiki/`.

Then:
- read notes
- edit summaries and concepts
- verify links between files


---

# Step 6: Cross-Reference Ideas

Use links like:

```markdown
[[concept-name]]
```

Examples:
- In a summary: `This paper supports [[inclusive-institutions]] and [[state-capacity]].`
- In a concept note: `Related summaries: [[2025-nobel-economics]], [[acemoglu-2001-colonial-origins]].`
- In index: `Institutions -> Growth -> [[inclusive-institutions]]`

---

# Step 7: Create `index.md` (Fast Retrieval)

Add one line per idea:

```markdown
- Technology and inequality → [[tech_inequality]]
- AI and jobs → [[automation_substitution]]
- Development and institutions → [[inclusive_institutions]]
```

Who this is useful for:
- for those with many readings: prevents getting lost
- for research writing: quickly find where ideas came from
- for exam review: scan main ideas fast before deep reading
- for AI support: better retrieval from organized notes

Key idea: **Scan first, then read deeply.**

---

# Step 8: Keep Compounding (Most Important)

When you have a useful idea (from class, reading, or discussion), ask:

```text
Turn this into a concept note and save it in concepts/
```

Why:
- turns temporary thoughts into permanent knowledge
- makes your system better over time

Key idea: **Don't lose good thoughts - save them.**

---

# Have a Great Weekend




