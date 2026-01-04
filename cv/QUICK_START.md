# Quick Start Guide

## 🚀 Getting Started in 5 Minutes

### Step 1: Add Your Images

1. Add your profile images to the `assets/` folder:
   - `profile.jpg` (400x400px recommended)
   - `about.jpg` (600x400px recommended)
   - `project1.jpg` through `project6.jpg` (800x450px recommended)
   - `favicon.ico` (32x32px)

### Step 2: Update Personal Information

Open `index.html` and replace:

- "Your Name" with your actual name (appears in multiple places)
- Job title and tagline
- Portfolio project details
- Skills and percentages
- Contact information (email, phone, location)
- Social media links

### Step 3: Configure Contact Form (Optional)

1. Sign up at [Formspree.io](https://formspree.io/)
2. Create a new form
3. Copy your form ID
4. In `script.js`, line ~280, replace `YOUR_FORM_ID` with your actual form ID

### Step 4: Test Locally

Open `index.html` in your browser or use a local server:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`

### Step 5: Deploy to GitHub Pages

1. Create a new GitHub repository
2. Upload all files
3. Go to Settings → Pages
4. Select `main` branch
5. Your site will be live at `https://yourusername.github.io/repository-name/`

## 📝 Important Notes

- **Images**: Make sure all image paths in `index.html` match your actual image filenames
- **Formspree**: The contact form will work without Formspree (shows success message), but won't actually send emails
- **Dark Mode**: Theme preference is saved in localStorage
- **Mobile**: Test on mobile devices or use browser dev tools

## 🎨 Customization Tips

- **Colors**: Edit CSS variables in `style.css` (lines 4-30)
- **Fonts**: Change Google Fonts link in `index.html` head section
- **Animations**: Adjust AOS settings in `script.js` (line 3)

## ❓ Need Help?

Check the main [README.md](README.md) for detailed documentation.
