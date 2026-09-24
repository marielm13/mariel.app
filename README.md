# marielmontuori.com — deploy guide

Plain static site: one `index.html`, no build step.

## Before launch (search index.html for "[")
- Photo: add `photo.jpg` here and swap the placeholder (see the PHOTO comment)
- Flagship AI case study: fill in or delete the card (see the FLAGSHIP comment)
- The AI Gap: add the three post titles and LinkedIn URLs (see the POSTS comment)

## Deploy on Vercel (about 15 minutes, one time)
1. Create a free account at vercel.com (the Hobby plan is fine for a personal site).
2. Easiest route: go to vercel.com/new, choose to deploy without Git, and drag this folder in.
   Better long-term route: put this folder in a GitHub repo and import it, so every
   edit you push redeploys automatically.
3. Framework preset: "Other". No build command, no output directory.
4. Vercel gives you a *.vercel.app link. Check it on desktop and phone.

## Custom domain
1. Buy the domain (e.g. at Cloudflare Registrar or Namecheap).
2. In Vercel: Project > Settings > Domains > add the domain and the www version.
3. Vercel shows the DNS records to add at your registrar. SSL is automatic.

## Updating later
Edit index.html (or ask Claude Code to), then redeploy: push to GitHub or re-upload the folder.
