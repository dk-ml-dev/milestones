# Deepu Kushwaha — Resume Site

A single-page static resume (`index.html`). No build step, no dependencies — Vercel will detect it as a static project automatically.

## Deploy with Vercel CLI (fastest)

1. Install the CLI (one-time): `npm i -g vercel`
2. From inside this folder, run: `vercel`
3. Follow the prompts (log in / link project). For a production URL immediately, run: `vercel --prod`

## Deploy via GitHub (recommended for updates)

1. Push this folder to a new GitHub repo:
   ```
   git init
   git add .
   git commit -m "Initial resume site"
   git branch -M main
   git remote add origin <your-repo-url>
   git push -u origin main
   ```
2. Go to https://vercel.com/new, import that repo.
3. Framework preset: choose **Other** (it's plain static HTML) — leave build command and output directory blank.
4. Click **Deploy**. Every future push to `main` will auto-redeploy.

## Notes

- `index.html` is the whole site — edit it directly for any content changes.
- The "Print / Save as PDF" button in the top bar still works after deployment (it uses `window.print()`), and is hidden automatically when printing.
- `vercel.json` just adds clean URLs and basic caching headers — safe to delete if you want Vercel's defaults.
- To use a custom domain, add it under Project Settings → Domains after the first deploy.
