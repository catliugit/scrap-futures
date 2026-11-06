# Scrap Futures — live site package

This is a static website ready to deploy.

## Quickest way to make it live

### Option 1: Netlify (easiest)
1. Go to https://app.netlify.com/drop
2. Drag the entire `Scrap_Futures_Live_Site` folder into the page, or upload the ZIP after extracting it.
3. Netlify will instantly publish the site and give you a public URL.
4. Optional: click **Domain settings** to connect your own domain.

### Option 2: Vercel
1. Create a free Vercel account.
2. Create a new project.
3. Upload this folder.
4. Because this is a static site, no build command is required.
5. Deploy.

### Option 3: GitHub Pages
1. Create a GitHub repo.
2. Upload `index.html`.
3. In repo settings, enable GitHub Pages from the main branch.
4. Your site will get a live URL.

## Suggested domain names
- scrapfutures.com
- scrapfutures.co
- getscrapfutures.com
- scrapfutures.io

## Notes
- This site is self-contained in a single HTML file.
- No backend is required.
- The calculator is front-end only and for demo purposes.
- Before deploying, set CONTACT_EMAIL near the top of the <script> in index.html so the "Email the founder" button works.
