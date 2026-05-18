# Rondane 2026 — Countdown 🏔️

A live countdown to **01.07.2026** — the day 7 friends hike to Rondeslottet in Dovre.

The number recalculates every time the page loads, so it always shows the correct number of days left.

**The Crew:** Andreas · Kjetil · Geir · Sondre · HC · Knut · Ole Martin

---

## How to host this for free on GitHub Pages (5 minutes)

You'll get a public URL like `https://<your-username>.github.io/rondane-2026/` that you can paste into Facebook.

### 1. Create a new GitHub repo

1. Go to <https://github.com/new>
2. Repo name: `rondane-2026` (or anything you like)
3. Set it to **Public** (required for free GitHub Pages)
4. Click **Create repository**

### 2. Upload the files

In the new empty repo, click **"uploading an existing file"** (or **Add file → Upload files**), then drag in **everything from this `site/` folder**:

- `index.html`
- `preview.png`
- `.nojekyll`
- `README.md` (optional)

Click **Commit changes**.

### 3. Turn on GitHub Pages

1. In the repo, go to **Settings** → **Pages** (left sidebar)
2. Under **Source**, pick **Deploy from a branch**
3. Branch: **`main`** · Folder: **`/ (root)`**
4. Click **Save**

Wait ~1 minute. Refresh the Pages settings page — at the top you'll see your live URL:

```
https://<your-username>.github.io/rondane-2026/
```

That's your countdown.

---

## Posting on Facebook

Two ways, do both for max effect:

### A) Live link in a post
1. Paste your `https://<your-username>.github.io/rondane-2026/` URL into a Facebook post.
2. Facebook auto-generates a preview card using `preview.png` (already wired up via `og:image` tags in `index.html`).
3. Add a caption like:
   > 44 dager til Rondane! 🏔️ Følg nedtellingen → [link]

### B) Just the image
If you only want a static post (no clickable link), upload `preview.png` directly. Re-post a fresh screenshot as the trip nears for the updated number.

### Force Facebook to refresh the preview
If FB caches the wrong image, paste your URL into the **Facebook Sharing Debugger** and click **Scrape Again**:
<https://developers.facebook.com/tools/debug/>

---

## Editing the page

Open `index.html` in any editor. Things you might want to change:

| What | Where |
|---|---|
| Trip date | Look for `2026-07-01T08:00:00` in the `<script>` near the bottom |
| Names | Search for `Andreas · Kjetil` in the `<div class="names">` block |
| Title / page meta | Top of file: `<title>` and `og:title` |
| Number color | CSS variable `--accent` and `--warm` at the top of the `<style>` block |
| Any cartoon character | Each hiker is inside a `<!-- HIKER N: ... -->` block in the SVG |

---

## Files in this folder

```
site/
├── index.html      ← the countdown page (open this in a browser to preview)
├── preview.png     ← Facebook/social card image (1400×900)
├── .nojekyll       ← tells GitHub Pages not to run Jekyll on these files
└── README.md       ← this file
```

That's it — happy hiking! 🥾
