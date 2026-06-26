# How to publish the study hub for your classmates

The site is just static files (web pages + audio). You publish it once and get a public link to paste in your class chat. Two routes — the first is the fastest.

## Fastest route — Netlify Drop (about 1 minute, no account needed)

1. Unzip **Economics-Prep-Site.zip** so you have a normal folder of files.
2. Go to **https://app.netlify.com/drop** in your browser.
3. Drag that **whole folder** onto the page.
4. Wait a few seconds — you get a public link like `https://random-name.netlify.app`.
5. Paste that link in your class chat. Anyone who opens it sees the hub, plays the podcasts, and takes the quizzes.

That's it. (Optional: make a free Netlify account to rename the link to something nicer and keep it permanent.)

## The Vercel route (you chose this — needs a quick sign-in)

Vercel can't be deployed for you from here because it needs your own login. Easiest Vercel path:

1. Create a free account at **https://vercel.com** (sign in with Google/GitHub).
2. Install the tool: open a terminal and run `npm i -g vercel` (needs Node.js installed).
3. Unzip the site, `cd` into the folder, and run `vercel`. Follow the prompts (it emails you a login code).
4. It returns a public `https://your-project.vercel.app` link to share.

If you don't already use a terminal, the Netlify Drop route above is much simpler and gives the same result.

## Good to know

- The link is **public** — anyone with it can view (perfect for classmates, but don't post it somewhere you don't want it found).
- `index.html` is the front page, so the bare link opens the hub automatically.
- To **update** it later (e.g. after we add anything), just re-drag the folder onto Netlify Drop, or run `vercel` again.
- Keep all files together — each day page loads its own podcast file by name.

## GitHub Pages route (free, lives under your GitHub)

All in the browser — no command line needed.

1. Unzip **Economics-Prep-Site.zip** to a plain folder.
2. On github.com: **+ → New repository**. Name it (e.g. `econ-prep`), make it **Public**, create it.
3. **Add file → Upload files** → drag in ALL files from the folder (`index.html`, every `Day-*.html`, every `Day-*.mp3`) → **Commit changes**.
4. **Settings → Pages** → Source: **Deploy from a branch**, Branch: **main**, folder **/ (root)** → **Save**.
5. Wait ~1 minute, refresh, and copy the link: `https://<your-username>.github.io/econ-prep/`. Open it on your phone and bookmark it.

Notes:
- The repo must be **public** for free Pages, so the link is public (fine for classmates).
- `index.html` is the front page, so the bare link opens the hub. File names are case-sensitive on GitHub — ours already match.
- To update later, upload the changed files again; Pages redeploys automatically.
