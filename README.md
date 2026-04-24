# 🚀 Deploying "The Daily Pulse" to GitHub Pages

## Quick Setup (5 minutes)

### Step 1: Create a GitHub Repository
1. Go to [github.com/new](https://github.com/new)
2. Name it: `the-daily-pulse`
3. Set it to **Public**
4. Click **Create repository**

### Step 2: Upload the Site Files
Option A — **Drag & Drop (easiest):**
1. Download the `the-daily-pulse.zip` file
2. Unzip it
3. In your new GitHub repo, click **"uploading an existing file"**
4. Drag all the files from the `site/` folder into the upload area
5. Click **Commit changes**

Option B — **Git command line:**
```bash
git clone https://github.com/YOUR_USERNAME/the-daily-pulse.git
cd the-daily-pulse
# Copy all files from the site/ folder here
git add .
git commit -m "Initial blog setup"
git push origin main
```

### Step 3: Enable GitHub Pages
1. Go to your repo → **Settings** → **Pages**
2. Under "Source", select **Deploy from a branch**
3. Branch: **main**, folder: **/ (root)**
4. Click **Save**
5. Wait 1-2 minutes — your site will be live at:
   `https://YOUR_USERNAME.github.io/the-daily-pulse/`

### Step 4: Update RSS Feed URLs
Once you know your GitHub username, find & replace `YOUR_GITHUB_USERNAME` in `feed.xml` with your actual username.

### Step 5: Submit RSS to NewsBreak
1. Go to [creators.newsbreak.com](https://creators.newsbreak.com)
2. Sign up as a Creator
3. Submit your RSS feed URL: `https://YOUR_USERNAME.github.io/the-daily-pulse/feed.xml`

---

## Adding New Posts

1. Create a new `.html` file in `posts/`
2. Add a card to `index.html`
3. Add an `<item>` to `feed.xml` (NewsBreak reads this)
4. Commit and push — GitHub Pages auto-deploys

## Site Structure
```
the-daily-pulse/
├── index.html          # Homepage
├── style.css           # Styles
├── feed.xml            # RSS feed (for NewsBreak)
└── posts/
    ├── ai-changing-everyday-life.html
    ├── morning-routines-that-work.html
    ├── street-food-trends-2026.html
    └── community-gardens-revival.html
```
