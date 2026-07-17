# Dog's Station — Ordering App

This is your ordering app, packaged as a normal website project so it can
be deployed to Vercel and connected to dogsstation.com.au.

It's already fully self-contained — all orders, schedule, and settings
are read from and written to your Google Sheet, so it works the same
here as it did inside Claude.ai.

---

## Option A — Easiest: deploy from GitHub (recommended)

1. **Create a free GitHub account** at github.com if you don't have one.
2. **Create a new repository** (e.g. "dogs-station"), then upload all the
   files in this folder to it (GitHub's website has an "upload files"
   button — you can drag the whole folder in, no command line needed).
3. **Go to vercel.com** and sign up / log in (you can sign in with your
   GitHub account directly, which makes step 4 easier).
4. Click **"Add New" → "Project"**, then select the GitHub repo you just
   created. Vercel will auto-detect it's a Vite app — just click **Deploy**.
5. Within about a minute, Vercel gives you a live link like
   `dogs-station.vercel.app` — that's your app, live on the internet.

## Option B — No GitHub: deploy from your computer (Vercel CLI)

If you'd rather not use GitHub, you can deploy straight from this folder:

1. Install [Node.js](https://nodejs.org) if you don't already have it
   (just click the big green "LTS" download button and install it).
2. Open a terminal in this folder and run:
   ```
   npm install -g vercel
   vercel
   ```
3. Follow the prompts (press Enter to accept the defaults). It will log
   in, ask a few questions, then deploy and give you a live link.

---

## Connecting dogsstation.com.au

Once your project is deployed and you can see it working on the
`*.vercel.app` link:

1. In your Vercel project, go to **Settings → Domains**.
2. Type in `dogsstation.com.au` and click **Add**.
3. Vercel will show you either:
   - A **CNAME record** to add, or
   - Two **A records** (IP addresses) to add
4. Go to wherever you bought the domain (your registrar), find
   **DNS settings** for dogsstation.com.au, and add exactly what Vercel
   showed you.
5. DNS changes can take anywhere from a few minutes to a few hours to
   activate. Vercel will show a green checkmark next to your domain once
   it's live.

Once that checkmark is green, `dogsstation.com.au` will show your
ordering app directly — no more `/vercel.app` link needed.

---

## If anything doesn't work

Come back and tell me exactly what step you're on and what you're
seeing (a screenshot helps a lot), and we'll sort it out from there.
