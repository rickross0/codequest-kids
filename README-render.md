# Deploy CodeQuest on Render.com (Step-by-Step)

This guide shows you exactly how to deploy **CodeQuest** on Render.com.

---

## ✅ Recommended Method: Using Git + Render (Easiest & Free)

### Step 1: Prepare Your Files

Make sure you have these files in a folder:

- `index.html` ← (this is your game)
- `render.yaml` ← (already created for you)
- `README.md`

> We already renamed `codequest.html` → `index.html` for you.

### Step 2: Create a GitHub Repository (Required for Render)

1. Go to [https://github.com/new](https://github.com/new)
2. Repository name: `codequest` (or anything you like)
3. Keep it **Public** (or Private — both work)
4. **Do NOT** initialize with README (we'll push existing files)
5. Click **Create repository**

### Step 3: Upload Your Files to GitHub

#### Option A: Using Git (Recommended)

Open your terminal in the folder containing the files:

```bash
# 1. Initialize git
git init

# 2. Add files
git add .

# 3. Commit
git commit -m "Initial CodeQuest game"

# 4. Connect to GitHub (replace YOUR_USERNAME and REPO_NAME)
git remote add origin https://github.com/YOUR_USERNAME/codequest.git

# 5. Push to GitHub
git branch -M main
git push -u origin main
```

#### Option B: Upload Manually (No Git)

1. Go to your new GitHub repo
2. Click **Add file** → **Upload files**
3. Drag and drop:
   - `index.html`
   - `render.yaml`
   - `README.md`
4. Commit the changes

### Step 4: Deploy on Render.com

1. Go to [https://dashboard.render.com](https://dashboard.render.com)
2. Sign in (free account works)
3. Click **+ New** → **Static Site**
4. Click **Connect** next to GitHub
5. Select your `codequest` repository
6. Render will auto-detect settings:
   - **Name**: `codequest-kids` (you can change this)
   - **Environment**: Static Site
   - **Build Command**: (leave empty)
   - **Publish Directory**: `.` (or leave as `/`)
7. Click **Create Static Site**

Render will now build and deploy your game!

### Step 5: Your Game is Live!

After deployment finishes:
- You'll get a URL like: `https://codequest-kids.onrender.com`
- Click the link to play!
- Every time you push to GitHub, Render will automatically redeploy.

---

## Alternative: Direct File Upload (Quick Test)

Render doesn't have a simple "drag and drop" like Netlify, but you can:

1. Create a new Static Site
2. Instead of connecting Git, use **"Deploy from existing files"** (not always available)
3. Or just use the Git method above — it's cleaner and better for updates.

**Recommendation**: Use the Git method.

---

## Custom Domain (Optional)

After deployment:
1. Go to your service on Render
2. Go to **Settings** → **Custom Domains**
3. Add your domain (Render gives you free SSL)

---

## Troubleshooting

**Game not loading?**
- Make sure `index.html` is in the root
- Check the deploy logs on Render

**Want to update the game later?**
- Just edit `index.html`
- Commit and push to GitHub
- Render will automatically redeploy

---

## Files You Need

| File            | Purpose                     |
|-----------------|-----------------------------|
| `index.html`    | The full game               |
| `render.yaml`   | Tells Render it's static    |

You're all set!

Once deployed, share the Render URL with your kids — they can play from any device. 🎮

Need help? Paste the URL Render gives you and I can help you customize it further.
