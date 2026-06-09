# Deploy to GitHub

Your PONG game is ready to push to GitHub! Follow these steps:

## 1. Create the GitHub Repository

Go to https://github.com/new and create a new repository:
- **Repository name**: `pong`
- **Description**: Classic two-player Pong game as a Progressive Web App
- **Public** (so GitHub Pages works)
- **Do NOT** initialize with README, .gitignore, or license (we already have these)

## 2. Push Your Code

After creating the repository on GitHub, run these commands:

```bash
cd /Users/jscalia/ClaudeProjects/pong

# Add the GitHub remote (replace YOUR-USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR-USERNAME/pong.git

# Push to GitHub
git branch -M main
git push -u origin main
```

## 3. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages** (left sidebar)
3. Under **Source**, select **main** branch
4. Click **Save**
5. Wait 1-2 minutes for deployment

Your game will be live at: `https://YOUR-USERNAME.github.io/pong/pong.html`

## 4. Update README (Optional)

After GitHub Pages is deployed, update the "Play Now" link in README.md:

```bash
# Edit README.md and replace the URL with your actual GitHub Pages URL
git add README.md
git commit -m "Update live demo link"
git push
```

## All Set! 🎉

Your game is now:
- ✅ Version controlled on GitHub
- ✅ Publicly accessible online
- ✅ Installable as an iPhone app
- ✅ Shareable with anyone

## Useful Commands

```bash
# Check git status
git status

# Make changes and commit
git add .
git commit -m "Your commit message"
git push

# View remote URL
git remote -v
```
