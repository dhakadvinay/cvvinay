# Modern Interactive CV/Portfolio Website

A beautiful, modern, and fully responsive single-page portfolio website with smooth animations, interactive elements, and dark mode support. Optimized for GitHub Pages hosting.

![Portfolio Preview](https://img.shields.io/badge/Status-Live-brightgreen) ![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-blue) ![License](https://img.shields.io/badge/License-MIT-yellow)

## 🌟 Features

### Design & UI
- ✨ **Modern, Clean Design** - Minimalist and professional aesthetic
- 🎨 **Dark/Light Mode** - Toggle between themes with localStorage persistence
- 📱 **Fully Responsive** - Mobile-first design that works on all devices
- 🎭 **Smooth Animations** - AOS (Animate On Scroll) library integration
- 💫 **Interactive Elements** - Hover effects, transitions, and micro-interactions

### Sections
1. **Hero Section**
   - Animated typing text effect
   - Floating profile image
   - Smooth scroll indicator
   - Gradient background animation

2. **About Me**
   - Animated statistics counter
   - Skill tags with hover effects
   - Profile image with rotating border

3. **Portfolio**
   - Filterable project categories (All, Web, Design, Mobile)
   - Project cards with hover overlays
   - Technology tags
   - Live demo and GitHub links

4. **Skills**
   - Animated progress bars for technical skills
   - Radial charts for soft skills
   - Technology logos carousel

5. **Contact**
   - Working contact form with validation
   - Formspree integration ready
   - Social media links
   - Contact information display

6. **Footer**
   - Dynamic copyright year
   - Back-to-top button
   - Social media links

### Technical Features
- ⚡ **Fast Loading** - Optimized performance with lazy loading
- ♿ **Accessible** - ARIA labels and keyboard navigation support
- 🔍 **SEO Optimized** - Meta tags and Open Graph tags
- 📦 **Single Page** - All content in one HTML file
- 🎯 **GitHub Pages Ready** - Relative paths and optimized structure

## 🚀 Live Demo

Visit the live website: [Your GitHub Pages URL]

## 📋 Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- A GitHub account (for hosting on GitHub Pages)
- Basic knowledge of HTML, CSS, and JavaScript (for customization)

## 🛠️ Setup Instructions

### 1. Clone or Download

```bash
git clone https://github.com/yourusername/cv.git
cd cv
```

Or download the ZIP file and extract it.

### 2. Customize Content

#### Update Personal Information

1. **index.html** - Replace placeholder content:
   - Update `<title>` and meta tags
   - Replace "Your Name" with your actual name
   - Update job title and tagline
   - Add your profile images to `assets/` folder
   - Update portfolio projects
   - Modify skills and percentages
   - Update contact information

2. **Images** - Add your images to `assets/` folder:
   - `profile.jpg` - Hero section profile image
   - `about.jpg` - About section image
   - `project1.jpg` through `project6.jpg` - Portfolio project images
   - `favicon.ico` - Website favicon
   - `og-image.jpg` - Open Graph image for social sharing

#### Configure Contact Form

1. **Option 1: Formspree** (Recommended)
   - Sign up at [Formspree](https://formspree.io/)
   - Create a new form and get your form ID
   - In `script.js`, replace `YOUR_FORM_ID` with your actual Formspree form ID:
   ```javascript
   const response = await fetch('https://formspree.io/f/YOUR_FORM_ID', {
   ```

2. **Option 2: EmailJS**
   - Sign up at [EmailJS](https://www.emailjs.com/)
   - Follow their integration guide
   - Update the form submission code in `script.js`

### 3. Deploy to GitHub Pages

#### Method 1: Using GitHub Web Interface

1. Create a new repository on GitHub
2. Upload all project files
3. Go to Settings → Pages
4. Select `main` branch and `/ (root)` folder
5. Click Save
6. Your site will be live at `https://yourusername.github.io/repository-name/`

#### Method 2: Using Git Commands

```bash
# Initialize git repository
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: Portfolio website"

# Add remote repository
git remote add origin https://github.com/yourusername/cv.git

# Push to GitHub
git branch -M main
git push -u origin main
```

Then enable GitHub Pages in repository settings.

### 4. Custom Domain (Optional)

1. Add a `CNAME` file in the root directory with your domain name
2. Configure DNS settings with your domain provider
3. Update GitHub Pages settings with your custom domain

## 📁 Project Structure

```
cv/
│
├── index.html          # Main HTML file
├── style.css           # All styles and animations
├── script.js           # JavaScript functionality
├── README.md          # This file
├── .gitignore         # Git ignore file
├── 404.html           # 404 error page for GitHub Pages
│
└── assets/            # Images and static files
    ├── profile.jpg
    ├── about.jpg
    ├── project1.jpg
    ├── project2.jpg
    ├── project3.jpg
    ├── project4.jpg
    ├── project5.jpg
    ├── project6.jpg
    ├── favicon.ico
    └── og-image.jpg
```

## 🎨 Customization Guide

### Colors & Theme

Edit CSS variables in `style.css`:

```css
:root {
    --primary-color: #6366f1;
    --secondary-color: #8b5cf6;
    --accent-color: #ec4899;
    /* ... more variables */
}
```

### Typography

Change fonts in `style.css`:

```css
--font-primary: 'Poppins', sans-serif;
--font-secondary: 'Inter', sans-serif;
```

Update Google Fonts link in `index.html` if needed.

### Animations

- Adjust AOS settings in `script.js`:
```javascript
AOS.init({
    duration: 1000,
    once: true,
    offset: 100,
});
```

- Modify animation speeds in `style.css` keyframes

### Portfolio Projects

Add or remove projects in `index.html`:

```html
<div class="portfolio-item" data-category="web">
    <!-- Project content -->
</div>
```

## 🧪 Testing

### Local Testing

1. Open `index.html` in a web browser
2. Or use a local server:
   ```bash
   # Python 3
   python -m http.server 8000
   
   # Node.js (with http-server)
   npx http-server
   ```

### Browser Compatibility

Tested and working on:
- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)

## 📱 Mobile Responsiveness

The website is fully responsive with breakpoints at:
- Desktop: 1200px+
- Tablet: 768px - 1199px
- Mobile: 320px - 767px

## 🔧 Technologies Used

- **HTML5** - Semantic markup
- **CSS3** - Modern styling with CSS Variables
- **JavaScript (ES6+)** - Vanilla JS, no frameworks
- **AOS Library** - Animate On Scroll
- **Typed.js** - Typing animation effect
- **Font Awesome** - Icons
- **Google Fonts** - Typography

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/yourusername/cv/issues).

## 👤 Author

**Your Name**

- Portfolio: [Your Portfolio URL]
- LinkedIn: [Your LinkedIn]
- GitHub: [@yourusername](https://github.com/yourusername)
- Email: your.email@example.com

## 🙏 Acknowledgments

- [AOS Library](https://michalsnik.github.io/aos/) for scroll animations
- [Typed.js](https://github.com/mattboldt/typed.js/) for typing effects
- [Font Awesome](https://fontawesome.com/) for icons
- [Google Fonts](https://fonts.google.com/) for typography

## 📄 Changelog

### Version 1.0.0 (Initial Release)
- ✅ Complete portfolio website
- ✅ Dark/light mode toggle
- ✅ Responsive design
- ✅ Contact form integration
- ✅ Portfolio filtering
- ✅ Smooth animations
- ✅ GitHub Pages optimization

---

⭐ If you like this project, please give it a star on GitHub!

