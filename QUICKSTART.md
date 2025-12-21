# Quick Start Guide - GitHub Pages Deployment

## Method 1: Simple GitHub Pages (Recommended for beginners)

1. **Create a new repository on GitHub**
   - Go to https://github.com/new
   - Name it (e.g., `r-course-brochure`)
   - Make it **public** (required for free GitHub Pages)
   - Don't initialize with README

2. **Push your code**
   ```bash
   cd "/home/aswath/Landing page R course brochure"
   git init
   git add .
   git commit -m "Initial commit: R Course Brochure"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to your repository → **Settings** → **Pages**
   - Under **Source**, select **Deploy from a branch**
   - Choose **main** branch and **/ (root)** folder
   - Click **Save**

4. **Your site is live!**
   - Visit: `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/`
   - Wait 1-2 minutes for first deployment

## Method 2: Using GitHub Actions (Automatic deployment)

The included `.github/workflows/deploy.yml` will automatically:
- Regenerate HTML when you push changes
- Deploy to GitHub Pages automatically

Just follow steps 1-2 above, then:
- Go to **Settings** → **Pages**
- Under **Source**, select **GitHub Actions**
- The workflow will run automatically on every push

## Updating Your Site

1. **Edit content** in `generate_site.py` or `index.html`
2. **If using Python script**: Run `python3 generate_site.py`
3. **Commit and push**:
   ```bash
   git add .
   git commit -m "Update course content"
   git push
   ```

## Troubleshooting

- **404 Error**: Make sure `index.html` is in the root directory
- **Images not loading**: Check that `images/` folder is included in git
- **Styling broken**: Verify `styles.css` is in the root directory
- **Site not updating**: Wait 1-2 minutes, GitHub Pages can take time to update

