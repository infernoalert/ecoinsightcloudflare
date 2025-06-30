# EcoInsight Research Project Website

A single-page website for the EcoInsight research project focused on understanding the workflow challenges of NCC 2022 for electrical engineers in Australia.

## Features

- **Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **Modern UI**: Clean, professional design with smooth animations
- **Smooth Scrolling**: Navigation links smoothly scroll to sections
- **Interactive Elements**: Hover effects and scroll-triggered animations
- **Accessibility**: Semantic HTML and keyboard navigation support

## File Structure

```
├── index.html          # Main HTML file
├── styles.css          # CSS styles
├── script.js           # JavaScript functionality
└── README.md           # This file
```

## Hosting on Cloudflare Pages

### Option 1: Using Cloudflare Dashboard (Recommended)

1. **Create a Cloudflare Account**
   - Go to [cloudflare.com](https://cloudflare.com) and sign up for a free account

2. **Access Cloudflare Pages**
   - Log into your Cloudflare dashboard
   - Navigate to "Pages" in the left sidebar
   - Click "Create a project"

3. **Connect Your Repository**
   - Choose "Connect to Git" 
   - Connect your GitHub/GitLab account
   - Select the repository containing these files
   - Or choose "Direct Upload" to upload files directly

4. **Configure Build Settings**
   - **Framework preset**: None (or Static HTML)
   - **Build command**: Leave empty
   - **Build output directory**: Leave empty (or `/` if required)
   - **Root directory**: Leave empty

5. **Deploy**
   - Click "Save and Deploy"
   - Your site will be available at `your-project-name.pages.dev`

### Option 2: Using Wrangler CLI

1. **Install Wrangler**
   ```bash
   npm install -g wrangler
   ```

2. **Login to Cloudflare**
   ```bash
   wrangler login
   ```

3. **Deploy**
   ```bash
   wrangler pages publish . --project-name=your-project-name
   ```

## Customization

### Updating Content
- Edit `index.html` to change text content
- Modify `styles.css` to adjust colors, fonts, and layout
- Update `script.js` for additional functionality

### Adding Your Photo
Replace the placeholder in the About section:
1. Add your photo to the project folder
2. Update the HTML in the about section:
   ```html
   <div class="about-image">
       <img src="your-photo.jpg" alt="Payam Amerian" class="profile-image">
   </div>
   ```
3. Add CSS for the image:
   ```css
   .profile-image {
       width: 200px;
       height: 200px;
       border-radius: 50%;
       object-fit: cover;
   }
   ```

### Updating Contact Information
- Change the email address in `index.html`
- Update the LinkedIn profile URL
- Modify any other contact details as needed

## Performance Features

- **Optimized Loading**: Minimal external dependencies
- **CDN Resources**: Font Awesome and Google Fonts loaded from CDN
- **Responsive Images**: Optimized for different screen sizes
- **Smooth Animations**: Hardware-accelerated CSS transitions

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## License

This project is created for the EcoInsight research project. Feel free to modify and use as needed.

## Support

For any issues with the website or deployment, please contact the development team. 