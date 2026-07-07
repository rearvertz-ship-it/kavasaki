# kavasaki.is-a.dev — contact page

Minimal contact page with a message form (via Formspree), TikTok and Instagram links.

## Quick start

### 1. Push to GitHub

```bash
# Create a repo named kavasaki (or whatever you like) on GitHub.
# Then:
git init
git add .
git commit -m "initial"
git remote add origin https://github.com/rearvertz-ship-it/kavasaki.git
git branch -M main
git push -u origin main
```

### 2. Enable GitHub Pages

1. Go to your repo **Settings → Pages**
2. Under **Branch**, select `main` and `/ (root)`
3. Click **Save**
4. Your site will be live at `https://rearvertz-ship-it.github.io/kavasaki` (or `rearvertz-ship-it.github.io` if the repo is named `rearvertz-ship-it.github.io`)

### 3. ✓ Formspree already configured

Messages go to **rearvertz@gmail.com**. Free tier: 50 submissions/month.

### 4. Claim `kavasaki.is-a.dev` (two PRs)

**PR 1 — Register the domain**
1. Fork [is-a-dev/register](https://github.com/is-a-dev/register)
2. In your fork, go to `domains/` and create `kavasaki.json`
3. Paste the contents of [`domains/kavasaki.json`](domains/kavasaki.json)
4. Open a pull request back to `is-a-dev/register`

**PR 2 — Verify domain ownership (while waiting for PR 1)**
1. Go to GitHub **Settings → Pages → Add a domain** and enter `kavasaki.is-a.dev`
2. Copy the TXT verification string they give you
3. In your fork of `is-a-dev/register`, create `domains/_github-pages-challenge-rearvertz-ship-it.kavasaki.json`
4. Paste the contents of [`domains/_github-pages-challenge-rearvertz-ship-it.kavasaki.json`](domains/_github-pages-challenge-rearvertz-ship-it.kavasaki.json)
5. Open a second PR to `is-a-dev/register`

**After both PRs merge:**
1. Go to GitHub **Settings → Pages → Custom domain** and enter `kavasaki.is-a.dev`
2. Click **Verify** (the TXT record should resolve now)
3. Check **Enforce HTTPS**
4. Done — your page is live at `https://kavasaki.is-a.dev`

### 5. (Optional) Free professional email

- **Zoho Mail** — free mailbox with your own domain (5GB). Set up MX records at your DNS provider.
- **Cloudflare Email Routing** — forwards emails to your existing Gmail, no storage limits.
- **iCloud+ Custom Domain** — free if you already have iCloud+.

## Files

| File | Purpose |
|------|---------|
| `index.html` | The contact page (avatar, form, social links) |
| `domains/kavasaki.json` | is-a.dev registration — submit to `is-a-dev/register` |
| `domains/_github-pages-challenge-rearvertz-ship-it.kavasaki.json` | GitHub Pages domain verification — submit to `is-a-dev/register` |
| `README.md` | This file |
