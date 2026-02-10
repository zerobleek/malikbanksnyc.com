# Shabaka Malik Banks - Portfolio

Personal portfolio website showcasing iOS development projects and professional work.

## 🚀 Live Site

Visit the live site at: `https://[your-username].github.io/[repository-name]`

## 📋 Features

- Clean, minimalist design
- Responsive layout
- Smooth animations
- Project showcase
- Social links integration

## 🛠️ Tech Stack

- HTML5
- CSS3 (Custom Properties, Grid, Flexbox)
- Google Fonts (DM Sans, DM Serif Display)
- Pure CSS animations

## 📦 Deployment to GitHub Pages

1. Create a new repository on GitHub
2. Clone the repository locally:
   ```bash
   git clone https://github.com/[your-username]/[repository-name].git
   cd [repository-name]
   ```

3. Add the files to your repository:
   ```bash
   git add .
   git commit -m "Initial commit - Portfolio website"
   git push origin main
   ```

4. Enable GitHub Pages:
   - Go to your repository on GitHub
   - Navigate to Settings > Pages
   - Under "Source", select "Deploy from a branch"
   - Select the `main` branch and `/ (root)` folder
   - Click Save

5. Your site will be live at `https://[your-username].github.io/[repository-name]` in a few minutes!

## 🎨 Customization

### Adding Your Photo
Replace the placeholder image by:
1. Adding your image file to the repository (e.g., `profile.jpg`)
2. Updating line 392 in `index.html`:
   ```html
   <div class="header-image">
       <img src="profile.jpg" alt="Your Name">
   </div>
   ```

### Updating Projects
Edit the project sections in `index.html` starting at line 401.

### Changing Colors
Modify the CSS custom properties in the `:root` section (lines 11-18):
```css
:root {
    --bg: #fafaf9;
    --text: #1c1917;
    --text-muted: #57534e;
    --border: #e7e5e4;
    --accent: #0a0a0a;
    --hover: #292524;
}
```

### Updating Links
Update social media links in:
- Ventures section (lines 509-528)
- Footer section (lines 536-538)

## 📝 License

© 2026 Shabaka Malik Banks. All rights reserved.

## 📧 Contact

- Email: [Your Email]
- GitHub: [@malikbanks](https://github.com/malikbanks)
- LinkedIn: [malikbanks](https://linkedin.com/in/malikbanks)
- Twitter: [@malikbanks](https://twitter.com/malikbanks)
