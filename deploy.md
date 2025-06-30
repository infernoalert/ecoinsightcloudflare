# Quick Deployment Guide - Cloudflare Pages

## Step-by-Step Instructions

### 1. Prepare Your Files
Make sure you have these files in your project folder:
- ✅ `index.html`
- ✅ `styles.css` 
- ✅ `script.js`
- ✅ `README.md`

### 2. Create Cloudflare Account
1. Go to [cloudflare.com](https://cloudflare.com)
2. Click "Sign Up" and create a free account
3. Verify your email address

### 3. Deploy to Cloudflare Pages

#### Method A: Direct Upload (Easiest)
1. Log into Cloudflare dashboard
2. Click "Pages" in the left sidebar
3. Click "Create a project"
4. Choose "Direct Upload"
5. Drag and drop your project folder (containing all files)
6. Click "Deploy site"
7. Your site will be live in seconds!

#### Method B: Git Repository
1. Upload your files to GitHub/GitLab
2. In Cloudflare Pages, choose "Connect to Git"
3. Connect your GitHub account
4. Select your repository
5. Configure build settings:
   - Framework preset: None
   - Build command: (leave empty)
   - Build output directory: (leave empty)
6. Click "Save and Deploy"

### 4. Custom Domain (Optional)
1. In your Pages project, go to "Custom domains"
2. Click "Set up a custom domain"
3. Enter your domain name
4. Follow the DNS configuration instructions

### 5. Your Site is Live!
Your website will be available at:
- `your-project-name.pages.dev` (Cloudflare subdomain)
- `yourdomain.com` (if you set up a custom domain)

## Quick Customization Tips

### Change Colors
Edit `styles.css` and look for:
- `#2563eb` (primary blue)
- `#667eea` and `#764ba2` (hero gradient)

### Update Contact Info
Edit `index.html` and find:
- Email: `research@ecoinsight.com.au`
- LinkedIn: `linkedin.com/in/payam-amerian`

### Add Your Photo
1. Add your photo to the project folder
2. Replace the placeholder in the About section with:
   ```html
   <img src="your-photo.jpg" alt="Payam Amerian" class="profile-image">
   ```

## Need Help?
- Cloudflare Pages documentation: https://developers.cloudflare.com/pages/
- Cloudflare support: https://support.cloudflare.com/

Your EcoInsight research website is ready to go! 🚀 