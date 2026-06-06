# ktripathy-site

Personal academic website. Single-file static site, no build step.

## Run locally
Open index.html in a browser. Or:
```bash
python -m http.server 8000   # then visit http://localhost:8000
```

## Deploy on GitHub Pages
```bash
git init && git add . && git commit -m "initial site"
gh repo create ktripa.github.io --public --source=. --push
# or push to any repo, then Settings > Pages > Deploy from branch > main
```
If the repo is named `ktripa.github.io`, the site goes live at https://ktripa.github.io.

## Claude Code workflow for this project
```bash
cd ktripathy-site
claude                        # start a session in this folder
```
First prompts to try, one tab per session:
1. "Read CLAUDE.md and index.html. Replace the photo placeholder with assets/photo.jpg and refine the Home tab spacing."
2. "Build out the Research tab: 3 cards from my PNAS, WRR, and GRL papers. I will paste figure captions."
3. "Add EDDI-14 and EDDI-28 to the Software tab. Precompute fields in Python to JSON, load via fetch."

## Roadmap
- [ ] Add real photo (assets/photo.jpg)
- [ ] Research tab: real figures + captions
- [ ] Blog: markdown-based posts
- [ ] Software: EDDI, ESI, SESR, SMVI from precomputed JSON (GLEAM subset)
- [ ] FlashCAT link + pip install instructions
