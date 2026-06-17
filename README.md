# Anirudh Soman — Portfolio Site

A single-page Product Manager portfolio site — built from Anirudh's resume, but framed as case studies (problem / approach / impact) and personal projects rather than a plain CV.

No build step — plain HTML/CSS/JS, no backend, no dependencies.

Live at **[anirudhsoman.in](https://anirudhsoman.in)**.

## 1. Preview it locally

Just open `index.html` in your browser — double-click the file, or right-click → Open With → your browser. No server needed.

## 2. How deployment works

This site auto-deploys — there's no manual upload step anymore.

- Code lives on GitHub: `https://github.com/anirudh28197/portfolio` (branch `main`)
- Netlify is connected to that repo and rebuilds the live site automatically on every push
- The custom domain `anirudhsoman.in` is pointed at Netlify via Netlify DNS (nameservers were changed at GoDaddy), with free auto-renewing SSL

So shipping a change is just:

```
git add .
git commit -m "describe the change"
git push
```

Netlify picks it up within a minute or two — check the **"Deploys"** tab on the site's Netlify dashboard to watch progress or see build logs if something looks off.

## 3. Updating content

Everything is in one file: `index.html`. Each section is clearly commented (`<!-- HERO -->`, `<!-- CASE STUDIES -->`, `<!-- PERSONAL PROJECTS -->`, `<!-- SKILLS -->`, etc.) — find the section, edit the text, save.

Each case study under `<!-- CASE STUDIES -->` follows the same pattern: a number/category tag, a title, then three blocks — **Problem Faced**, **How I Solved It**, **Impact**. Copy that pattern for any new case study you add.

- Colors/spacing: `style.css` — the accent color is one line near the top (`--accent: #2dd4bf;`), change it there to re-theme the whole site.
- Animations/interactions: `script.js`.

After editing, commit and push (see above) to go live.

## 4. If something goes wrong with the domain/SSL

- Domain/DNS settings: GoDaddy → My Products → `anirudhsoman.in` → DNS (nameservers should be `dns1-4.p05.nsone.net`)
- Netlify-side domain config: Netlify site → Site configuration → Domain management
- SSL is automatic (Let's Encrypt via Netlify) and renews on its own — nothing to maintain manually
