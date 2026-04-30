# Vercel walkthrough — spoken script (~2–3 minutes)

**Audience:** students who already have a working `index.html` opened locally.  
**Path:** GitHub repository → Vercel import (static site). Adjust wording if your course uses a different primary path.

---

## 0:00–0:20 — Goal

“By the end of this, you’ll have a **public link** that opens your page in any browser—same idea as sharing a Google Doc link, but it’s your HTML. We’ll use **Vercel** and assume your files are in a **GitHub** repo.”

---

## 0:20–0:55 — GitHub prep

“First, make sure your project folder contains **`index.html`** at the **root** of what you’re deploying—the same place Vercel will look when it builds. If you use images or a CSS file, keep paths **relative** to `index.html`, and commit everything. Push to GitHub so the repo is up to date.”

---

## 0:55–1:45 — Vercel import

“Log into **vercel.com**, click **Add New… → Project**, then **Import** your GitHub repository. If this is your first time, authorize GitHub when asked. When Vercel asks for framework settings, choose **Other** or the static option—there’s no React or Next required here. Don’t change the root unless your `index.html` lives in a subfolder on purpose; for this class, root is simplest.”

---

## 1:45–2:30 — Deploy and test

“Click **Deploy**. When the build finishes, open the **production URL** Vercel shows you. Check on your phone or in an **incognito** window so you’re not fooled by cache. If something’s wrong—blank page, missing images—compare what’s **online** to what works **locally**; usually it’s the wrong folder, a typo in `index.html`, or a broken relative path.”

---

## 2:30–3:00 — After you change files

“Whenever you edit your page, **commit and push** to GitHub again. Vercel will create a **new deployment**; use the production URL from the latest deploy. That’s what you submit for the assignment.”

---

**TA note:** If live demo fails, show a prerecorded screen capture of these steps and keep this script as the canonical order.
