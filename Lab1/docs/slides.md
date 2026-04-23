---

marp: true
theme: default
paginate: true
size: 16:9
header: "Econ 30 -- Lab 1"
footer: "Stanford University | Spring 2026"
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

# Introduction to Cursor

## Econ 30 -- Lab 1

### Samira Gholami

Spring 2026

---

# Today Section

- Intorduction and Logistics
- Build a mini research project from scratch using Cursor:

You will work on one of your ideas and by the end of this session you will have: 

- A project folder structure
- A synthetic dataset (if applies to your project)
- An OLS regression results
- Related figures and tables
- A written research memo

---

# Agenda


| Part | Topic                                | Time   |
| ---- | ------------------------------------ | ------ |
| 0    | Orientation & Setup                  | 8 min  |
| 1    | Project Scaffolding (Agent mode)     | 7 min  |
| 2    | Designing the Analysis (Plan mode)   | 10 min |
| 3    | Building & Running Code (Agent mode) | 20 min |
| 4    | Writing a Research Memo              | 8 min  |
| 5    | Wrap-Up & Cheat Sheet                | 7 min  |


---

# Part 1: Logistics & Introduction

**Introductions** -- please share: your name, major, year, and one research question you hope to work on.

**About Lab Sessions:**
- These sessions are opportunities to learn tools and make progress on your projects
- Consider them a focused hour on your project -- I'll help you figure it out
- Please bring your laptops and be ready to engage

**Getting Help:**
- I'm here to help you push on your project, along with Lukas
- If you feel stuck or unsure how to proceed, always feel free to email me
- Issues on Canvas (submissions / peer reviews) -- also feel free to email me

---

# Part 2

## Cursor

---

# Why Cursor?

It's great tool that can switch from conversation to AI agent, to question to coding and etc. 

Let's start from learning about the environment of Cursor.

# The Chat Panel

The **Chat panel** is on the right side of Cursor.

Open it with `**Ctrl+L`**

This is where you talk to the AI. Everything starts here.

At the top of the chat you will see:

- A **mode toggle** (Ask / Plan / Agent)
- A **model selector** dropdown

---

# Three Modes


| Mode      | What It Does                         | When to Use It                         |
| --------- | ------------------------------------ | -------------------------------------- |
| **Ask**   | Read-only Q&A                        | "What does this function do?"          |
| **Plan**  | AI proposes a plan; you review first | "How should I structure this project?" |
| **Agent** | AI reads, writes, and runs code      | "Build me a scatter plot"              |


Think of it as a spectrum:

**Ask** = just talking  --  **Plan** = thinking together  --  **Agent** = doing

---

# Model Selection

The dropdown in chat lets you choose which AI model to use.


| Model                   | Strengths                            |
| ----------------------- | ------------------------------------ |
| Claude Opus / o3        | Best reasoning, complex planning     |
| Claude Sonnet / GPT-4.1 | Fast, great for straightforward code |


**Rule of thumb:**

- Strong model for **planning** (thinking is hard)
- Fast model for **execution** (typing is easy)

---

# Extensions

Make sure you have the **Python** extension installed:

1. Open Extensions sidebar: `**Ctrl+Shift+X`**
2. Search for **"Python"**
3. Install the one by **Microsoft** (if not already installed)

Other useful extensions: R, Jupyter, Rainbow CSV, Markdown Preview

---

# The Key Mindset

> Everything you do for this class -- code, notes, outlines, reading summaries -- should happen inside Cursor.

Cursor is not just a coding tool. It is a **text editor** with superpowers.

If you are typing text into a file, do it in Cursor.

---

# Setup Check

Before we begin:

1. Open Cursor
2. **File > Open Folder** -- open your empty `Lab1` folder
3. Open the Chat panel (`Ctrl+L`)
4. Confirm you are in **Agent** mode

Everyone ready?

---

# Part 1

## Project Scaffolding (7 min)

---

# Your First Prompt

Switch to **Agent** mode. Copy-paste this into chat:

```
Set up a project folder structure for an empirical
economics research project.
Create the following folders: data/, code/, figures/,
output/, docs/
Also create a README.md that briefly describes the project:
"Returns to Education: analyzing the relationship
between schooling and wages."
```

Watch Cursor create your entire project structure.

---

# What Just Happened?

You told the AI **what** you wanted, and it figured out **how** to do it.

You should now see in the Explorer sidebar:

- `data/`
- `code/`
- `figures/`
- `output/`
- `docs/`
- `README.md`

**Lesson:** Agent mode can create files and folders. Good prompts get good results.

---

# Part 2

## Designing the Analysis (10 min)

---

# Switch to Plan Mode

Change the mode toggle from **Agent** to **Plan**.

In Plan mode, the AI will **propose a plan** but will **not change any files**.

This is where you think before you code.

This is also where you would use a **strong model** (Opus / o3) -- planning requires deep reasoning.

---

# The Planning Prompt

Paste this into chat (in **Plan** mode):

```
I want to analyze the returns to education using
individual-level data. Plan a Python analysis that:
1. Generates a synthetic dataset of 2,000 individuals
   with: years of education (8-20), years of experience
   (0-30), a gender indicator, and log hourly wages
   following a Mincer equation with a gender wage gap
2. Produces summary statistics
3. Runs an OLS regression of log wages on education,
   experience, experience-squared, and gender
4. Creates two figures: (a) a scatter of education vs.
   wages with a fitted line, (b) a bar chart of the
   gender wage gap
Save data to data/, scripts to code/, figures to
figures/, regression output to output/
```

---

# Read the Plan

The AI will produce a structured plan. Take a moment to:

- **Read it carefully.** Does the approach make sense?
- **Ask follow-up questions** in chat (still in Plan mode)
- **Discuss with your neighbor.** What would you change?

Notice: **no files were created or changed.** Plan mode is read-only.

This mirrors real research workflow: **plan first, code second.**

---

# Part 3

## Building & Running Code (20 min)

---

# Execute the Plan

Switch back to **Agent** mode. Type:

```
Go ahead and implement the plan.
Write clean, well-structured Python code.
```

Cursor will:

- Create `code/generate_data.py`
- Create `code/analysis.py`
- Generate `data/wages.csv`
- Save figures to `figures/`
- Save regression results to `output/`

Watch it work!

---

# Exercise A: Inline Editing

While code is generated, try `**Ctrl+K**` (inline edit):

1. Open a generated `.py` file
2. **Select** a few lines of code (e.g., plotting code)
3. Press `**Ctrl+K`**
4. Type: `Add a title and axis labels, use a colorblind-friendly palette`
5. Press Enter

This is how you make **quick, targeted changes** without going to the chat panel.

---

# Exercise B: Ask Mode for Learning

Switch to **Ask** mode. Highlight the regression code and type:

```
Explain what this regression is doing
and interpret the coefficients.
```

The AI will explain the code **without changing anything**.

This is how you use Cursor to **learn**, not just produce.

---

# Exercise C: The Terminal

Open the built-in terminal: `**Ctrl+`*`*

Run your scripts:

```
python code/generate_data.py
python code/analysis.py
```

The terminal is built into Cursor -- **no need to switch apps.**

---

# Exercise D: Debugging

If a script throws an error:

1. **Copy** the full error traceback
2. Switch to **Agent** mode
3. **Paste** the error and say: `Fix this error`
4. Cursor will diagnose and fix the issue

Errors are not failures -- they are prompts for the next iteration.

---

# Checkpoint

You should now have:

- `data/wages.csv` -- your dataset
- `figures/education_vs_wages.png` -- scatter plot
- `figures/gender_wage_gap.png` -- bar chart
- `output/regression_results.txt` -- OLS output

Raise your hand if anything is missing.

---

# Part 4

## Writing in Cursor (8 min)

---

# Cursor Is Not Just for Code

You should use Cursor for **everything**: prose, notes, memos, outlines.

Switch to **Agent** mode and paste:

```
Write a short 1-page research memo in docs/memo.md
summarizing:
- The research question (returns to education)
- The data (describe the synthetic dataset)
- Key findings from the regression (reference the
  coefficients)
- Embed the two figures from figures/
Keep it concise and professional.
```

---

# Edit and Preview

After the memo is generated:

1. **Open** `docs/memo.md`
2. **Manually edit** a sentence -- add your name, rephrase something
3. Preview the rendered Markdown: `**Ctrl+Shift+V`**

Cursor is a full-featured text editor. The AI assists you, but **you are in control.**

---

# Part 5

## Wrap-Up (7 min)

---

# What You Learned Today


| Feature        | How to Access    | When to Use                   |
| -------------- | ---------------- | ----------------------------- |
| Ask Mode       | Mode toggle      | Understanding, learning       |
| Plan Mode      | Mode toggle      | Project design, before coding |
| Agent Mode     | Mode toggle      | Building, generating, fixing  |
| Inline Edit    | `Ctrl+K`         | Quick targeted code changes   |
| Model Selector | Dropdown in chat | Match model to task           |
| Terminal       | `Ctrl+``         | Running scripts               |
| Extensions     | `Ctrl+Shift+X`   | Language support              |


---

# Final Exercise

Use **Agent** mode to create your personal reference:

```
Create a file called docs/cursor_cheatsheet.md with
a quick-reference guide to the Cursor features I
used today: modes, keyboard shortcuts, and tips for
using AI effectively in research.
```

You now have a cheat sheet to take home.

---

# After the Lab

- **Use Cursor for all Econ 30 work.** Problem sets, reading notes, data analysis.
- **Experiment with prompts.** Better instructions produce better output.
- **Use Plan mode before big tasks.** Think before you code.
- **Use Ask mode to learn.** Highlight code and ask "Explain this."
- **Refer to your cheat sheet** whenever you forget a feature.

---

# Happy Coding!

## Open the lab handout: `docs/lab_handout.md`

Questions? Raise your hand or ask in Cursor chat.