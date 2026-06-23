# 🚀 Deploy CodeQuest (Super Easy!)

CodeQuest is a **single HTML file** — no build step, no server, nothing complicated.

## Fastest Ways to Deploy (Free)

### 1. Netlify Drop (Recommended - 30 seconds)
1. Go to: https://netlify.com/drop
2. Drag `codequest.html` from your computer onto the page
3. Done! You get a free `.netlify.app` URL instantly
4. Share the link with friends/kids!

### 2. Vercel (Also very fast)
1. Go to https://vercel.com
2. Sign in with GitHub
3. Click "Add New Project"
4. Upload or connect a repo containing `codequest.html`
5. Deploy

### 3. GitHub Pages
1. Create a new GitHub repository
2. Upload `codequest.html` (rename it to `index.html` if you want)
3. Go to **Settings → Pages**
4. Under "Source", choose "Deploy from a branch"
5. Select your main branch + root folder
6. Save — your site will be live at `https://yourusername.github.io/reponame`

### 4. Cloudflare Pages
1. Go to https://pages.cloudflare.com
2. Connect your GitHub repo or upload the file
3. Deploy

## Local Testing First

Before deploying, always test locally:
```bash
# Option 1: Just double-click codequest.html
# Option 2: Use a simple server
python3 -m http.server 8000
# Then open http://localhost:8000/codequest.html
```

## Making It Even Better (Optional)

### Add a Custom Domain
- Netlify / Vercel / Cloudflare all support free custom domains

### Make It Mobile Friendly
Already works great on phones and tablets!

### Enable Real Multiplayer (Advanced)
Want real-time leaderboards with friends?
- Host the HTML file
- Use services like:
  - Supabase (free)
  - Firebase (free tier)
  - Or simply use the built-in share code system

## Tips for Teachers / Parents

- Deploy once → share the link with the whole class
- Progress is stored in the browser (per device)
- Use the "Share Progress" feature so kids can compete with friends
- Print certificates directly from the game

---

**Your game is 100% ready to deploy right now.**

Just drag `codequest.html` to Netlify Drop and you're live!