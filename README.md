# Recognition Pretest — Erlangen

This folder is a complete, standalone static site — copy it into the root of its own
GitHub repo and enable GitHub Pages (Settings → Pages → Deploy from `main` branch).
No build step, no dependencies.

**Before deploying:**
1. Set `notifyEmails` and `emailjs` in `config.js` — see the main project's
   `email-relay/DEPLOY.md` for how to get those values.
2. Add the 317 image files listed in `images/REQUIRED_IMAGES.txt` into `images/`, then
   run `python3 check_images.py sites/erlangen` from the main project root to confirm
   nothing's missing.
3. Optionally add `images/instructions_example.png` to replace the placeholder on the
   instructions screen.
4. Test locally first: `python3 -m http.server 8000` in this folder, then open
   `http://localhost:8000`.

This site was generated from the main project's `src/`. If you need to change
shared wording, styling, or logic, edit it there and regenerate — see the root
`README.md`.
