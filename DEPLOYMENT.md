# Deploying EcoInsight to Cloudflare Pages

This guide will help you deploy your EcoInsight website to Cloudflare Pages.

## Prerequisites

1. **Node.js** installed on your computer (download from https://nodejs.org/)
2. **Git** installed (download from https://git-scm.com/)
3. **Cloudflare account** (free at https://cloudflare.com/)

## Method 1: Deploy via Cloudflare Dashboard (Recommended for beginners)

### Step 1: Prepare Your Files
1. Make sure all your files are in the project directory:
   - `index.html`
   - `styles.css`
   - `script.js`
   - `README.md`

### Step 2: Create a GitHub Repository
1. Go to [GitHub](https://github.com) and create a new repository
2. Name it something like `ecoinsight-website`
3. Upload your files to the repository

### Step 3: Deploy to Cloudflare Pages
1. Go to [Cloudflare Dashboard](https://dash.cloudflare.com/)
2. Click on "Pages" in the left sidebar
3. Click "Create a project"
4. Choose "Connect to Git"
5. Select your GitHub repository
6. Configure the build settings:
   - **Framework preset**: None
   - **Build command**: Leave empty
   - **Build output directory**: Leave empty
   - **Root directory**: Leave empty
7. Click "Save and Deploy"

Your site will be deployed to a URL like: `https://your-project-name.pages.dev`

## Method 2: Deploy via Wrangler CLI

### Step 1: Install Wrangler
```bash
npm install -g wrangler
```

### Step 2: Login to Cloudflare
```bash
wrangler login
```

### Step 3: Deploy
```bash
wrangler pages deploy .
```

## Custom Domain (Optional)

1. In your Cloudflare Pages dashboard, go to your project
2. Click on "Custom domains"
3. Add your domain (e.g., `ecoinsight.com.au`)
4. Follow the DNS configuration instructions

## Troubleshooting

### Common Issues:
1. **Files not found**: Make sure all files are in the root directory
2. **CSS/JS not loading**: Check that file paths in `index.html` are correct
3. **Deployment fails**: Check the build logs in Cloudflare dashboard

### Support:
- Cloudflare Pages documentation: https://developers.cloudflare.com/pages/
- Wrangler documentation: https://developers.cloudflare.com/workers/wrangler/

## File Structure
```
ecoinsightcloudflare/
├── index.html          # Main HTML file
├── styles.css          # CSS styles
├── script.js           # JavaScript functionality
├── wrangler.toml       # Wrangler configuration
├── package.json        # Project metadata
├── .gitignore          # Git ignore rules
├── README.md           # Project documentation
└── DEPLOYMENT.md       # This file
``` 