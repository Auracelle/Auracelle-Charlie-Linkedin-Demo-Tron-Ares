# GitHub Pages Deployment Guide

## Complete Deployment Steps

### 1. Create GitHub Repository

```bash
# On GitHub.com:
1. Click "+" → "New repository"
2. Name: "auracelle-charlie"
3. Description: "Strategic Intelligence War Gaming Governance Simulation Sandbox"
4. Public repository
5. Don't initialize with README (we have our own)
6. Click "Create repository"
```

### 2. Upload Files

**Option A: GitHub Web Interface**
1. Click "uploading an existing file"
2. Drag and drop ALL files:
   - index.html
   - README.md
   - LICENSE
   - .gitignore
3. Commit message: "Initial commit - Auracelle Charlie Tron Ares Edition"
4. Click "Commit changes"

**Option B: Command Line**
```bash
cd /path/to/auracelle-charlie

git init
git add .
git commit -m "Initial commit - Auracelle Charlie Tron Ares Edition"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/auracelle-charlie.git
git push -u origin main
```

### 3. Enable GitHub Pages

1. Go to repository Settings
2. Scroll to "Pages" section (left sidebar)
3. Source: Select "main" branch
4. Folder: Select "/ (root)"
5. Click "Save"
6. Wait 2-3 minutes for deployment

### 4. Access Your Site

Your site will be live at:
```
https://YOUR_USERNAME.github.io/auracelle-charlie/
```

### 5. Update README Links

Replace all instances of `yourusername` in README.md with your actual GitHub username.

---

## Troubleshooting

**Issue**: Site shows 404
- **Fix**: Wait 3-5 minutes, GitHub Pages needs time to build

**Issue**: Styling doesn't load
- **Fix**: Ensure index.html is in root directory, not in a subfolder

**Issue**: CDN resources blocked
- **Fix**: Check browser console, ensure you're using HTTPS

---

## Optional: Custom Domain

1. Buy domain (e.g., auracelle-charlie.com)
2. Settings → Pages → Custom domain
3. Add CNAME record in your DNS:
   - Type: CNAME
   - Name: www
   - Value: YOUR_USERNAME.github.io

---

## Deployment Complete! 🚀

Your Auracelle Charlie simulation is now live!
