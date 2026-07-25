# 🚀 Deployment Guide - Yusuf Kedir Portfolio

This guide shows you how to:

1. Push your portfolio to GitHub
2. Deploy for free using **GitHub Pages** and **Netlify**

---

## Step 1: Push to GitHub

Open **Terminal** or **Git Bash** in your project folder and run:

```bash
# Initialize git repository
git init

# Add all files
git add .

# Create first commit
git commit -m "Initial commit - Yusuf Kedir Portfolio"

# Create a new GitHub repository
gh repo create yusuf-kedir-portfolio --public --source=. --remote=origin --push

# Or if you already created a repo on GitHub manually:
# git branch -M main
# git remote add origin https://github.com/yu12suf/yusuf-kedir-portfolio.git
# git push -u origin main
```

---

## Step 2: Deploy with GitHub Pages (Free - Easy)

### Method A: GitHub Pages (No custom domain)

1. Go to your repository on GitHub: `https://github.com/yu12suf/yusuf-kedir-portfolio`
2. Click **Settings** → **Pages** (in left sidebar)
3. Under "Source", select **Deploy from a branch**
4. Select branch: `main`, folder: `/ (root)`
5. Click **Save**
6. Wait 1-2 minutes, then your site will be live at:
   ```
   https://yu12suf.github.io/yusuf-kedir-portfolio/
   ```

---

## Step 3: Deploy with Netlify (Free - Better)

Netlify gives you a professional URL and is faster.

### Option A: Deploy from GitHub (Recommended)

1. Go to [https://app.netlify.com](https://app.netlify.com)
2. Click **Sign up** (use GitHub to login)
3. Click **Add new site** → **Import an existing project**
4. Select your GitHub repo: `yu12suf/yusuf-kedir-portfolio`
5. Deploy settings:
   - **Branch**: `main`
   - **Publish directory**: `/` (leave empty - it's the root)
   - Leave everything else default
6. Click **Deploy site**
7. Your site will be live at a random Netlify URL like:
   ```
   https://your-site-name.netlify.app
   ```

### Option B: Drag & Drop (No GitHub needed)

1. Go to [https://app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag and drop your **PortfolioWebsite** folder onto the browser
3. Your site is deployed instantly!

---

## Step 4: Custom Domain (Optional)

### For GitHub Pages:

1. Buy domain from Namecheap, GoDaddy, etc.
2. In GitHub repo Settings → Pages, enter your custom domain
3. Update DNS records at your domain provider (add CNAME)

### For Netlify:

1. Go to your site dashboard → **Domain settings**
2. Click **Add custom domain**
3. Follow Netlify's DNS instructions (much easier than GitHub)

---

## Step 5: Auto-Updates

### For GitHub Pages:

Every time you push to main branch, GitHub automatically redeploys:

```bash
git add .
git commit -m "Updated portfolio content"
git push
```

### For Netlify:

Same - just push to GitHub and Netlify automatically redeploys.

---

## Quick Summary

```
1. git init
2. git add .
3. git commit -m "Initial commit"
4. git branch -M main
5. gh repo create yusuf-kedir-portfolio --public --source=. --remote=origin --push
6. Go to Netlify.com → Import from GitHub → Deploy
```

**Your live portfolio URL:** `https://yu12suf.github.io/yusuf-kedir-portfolio/`
