# Anirudh Soman — Portfolio Site

A single-page Product Manager portfolio site — built from Anirudh's resume, but framed as case studies (problem / approach / impact) and personal projects rather than a plain CV.

No build step — plain HTML/CSS/JS, no backend, no dependencies.

## 1. Preview it locally

Just open `index.html` in your browser — double-click the file, or right-click → Open With → your browser. No server needed.

## 2. Deploy to Netlify (free)

1. Go to [netlify.com](https://www.netlify.com) and sign up for a free account (you can use your Google or email account).
2. Once logged in, you'll land on your **Sites** page. Look for a box that says **"Add new site"** → click it → choose **"Deploy manually"**.
3. A page appears with a dashed drop-zone that says **"Drag and drop your site output folder here"**.
4. Open Finder, find this `portfolio` folder, and drag the whole folder onto that drop-zone.
5. Netlify uploads it and gives you a live URL right away, like `https://random-name-123.netlify.app`. That's your site — open it to check.

## 3. Give it a nicer URL

1. On your new site's page in Netlify, click **"Site configuration"** in the left sidebar.
2. Click **"Change site name"**.
3. Enter something like `anirudh-soman` and save. Your site is now at `https://anirudh-soman.netlify.app` (or similar — Netlify will tell you if that name is taken and suggest you try another).

## 4. Updating content later

Everything is in one file: `index.html`. Each section is clearly commented (`<!-- HERO -->`, `<!-- CASE STUDIES -->`, `<!-- PERSONAL PROJECTS -->`, `<!-- SKILLS -->`, etc.) — find the section, edit the text, save.

Each case study under `<!-- CASE STUDIES -->` follows the same pattern: a number/category tag, a title, then three blocks — **Problem Faced**, **How I Solved It**, **Impact**. Copy that pattern for any new case study you add.

- Colors/spacing: `style.css` — the accent color is one line near the top (`--accent: #2dd4bf;`), change it there to re-theme the whole site.
- Animations/interactions: `script.js`.

After editing, redeploy by dragging the `portfolio` folder onto your site's **"Deploys"** tab in Netlify (same drag-and-drop as step 2).

## 5. Later, if you want it (optional)

- **Custom domain**: if you buy a domain (e.g. `anirudhsoman.com`), Netlify's **"Domain management"** page walks you through pointing it at this site.
- **Auto-deploy on every change**: connecting this folder to a GitHub repo and linking that repo in Netlify means edits go live automatically without re-dragging the folder. Worth doing later if you start updating the site often — ask and we can set it up.
