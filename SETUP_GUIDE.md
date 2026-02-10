# GitHub Pages Setup Guide

Follow these steps to deploy your portfolio to GitHub Pages:

## Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the "+" icon in the top right corner
3. Select "New repository"
4. Name your repository (e.g., `portfolio` or `[your-username].github.io`)
   - If you name it `[your-username].github.io`, it will be your main GitHub Pages site
   - Otherwise, it will be accessible at `https://[your-username].github.io/[repository-name]`
5. Choose "Public" (required for free GitHub Pages)
6. Do NOT initialize with README (we already have files)
7. Click "Create repository"

## Step 2: Upload Your Files

### Option A: Using GitHub Web Interface (Easiest)
1. On your new repository page, click "uploading an existing file"
2. Drag and drop these files:
   - `index.html`
   - `README.md`
   - `.gitignore`
3. Add a commit message like "Initial commit"
4. Click "Commit changes"

### Option B: Using Git Command Line
```bash
# Navigate to your project folder
cd /path/to/your/files

# Initialize git repository
git init

# Add all files
git add .

# Commit the files
git commit -m "Initial commit - Portfolio website"

# Add your GitHub repository as remote
git remote add origin https://github.com/[your-username]/[repository-name].git

# Push to GitHub
git branch -M main
git push -u origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on "Settings" tab
3. Scroll down to "Pages" in the left sidebar
4. Under "Source", select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click "Save"
6. GitHub will show a message: "Your site is ready to be published at..."

## Step 4: Wait for Deployment

- The first deployment takes 1-3 minutes
- You'll see a green checkmark when it's ready
- Visit your site at the URL provided

## Step 5: Add Your Photo (Optional)

1. Add your photo to the repository (upload via GitHub or git)
2. Edit `index.html` line 392 to reference your photo:
   ```html
   <img src="your-photo.jpg" alt="Shabaka Malik Banks">
   ```
3. Commit and push the changes

## Troubleshooting

### Site not loading?
- Wait a few more minutes (can take up to 10 minutes)
- Check that you selected the correct branch (main)
- Make sure the repository is public

### 404 Error?
- Verify the file is named `index.html` (not `index_2.html`)
- Check that it's in the root folder, not a subfolder

### Changes not showing?
- GitHub Pages has a cache - try clearing browser cache
- Force refresh with Ctrl+F5 (Windows) or Cmd+Shift+R (Mac)
- Can take a few minutes for changes to appear

## Custom Domain (Optional)

If you want to use your own domain:

1. Add a file named `CNAME` with your domain:
   ```
   yourdomain.com
   ```
2. Configure DNS records with your domain provider:
   - Add an A record pointing to GitHub's IPs:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - Or add a CNAME record pointing to `[your-username].github.io`

## Need Help?

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Pages Quickstart](https://docs.github.com/en/pages/quickstart)
