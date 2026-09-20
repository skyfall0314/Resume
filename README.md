# Chris Franco — Interactive Resume Website 🚀

A modern, animated, dark-themed resume website built to stand out to hiring managers.

## Features

- ✨ **Dark/Light Mode** — Toggle between themes, preference saved locally
- 📊 **Animated Skill Bars** — Fill on scroll with staggered animations
- 📅 **Interactive Timeline** — Click to expand/collapse role details
- 🔢 **Animated Counters** — Key metrics animate as you scroll
- 📥 **Download Resume** — One-click PDF download button
- 📬 **Contact Form** — Formspree integration (or mailto fallback)
- 🎯 **QR Code** — In the footer, scannable to share the site URL
- 🖱️ **Cursor Glow** — Subtle interactive glow effect (desktop)
- 📱 **Fully Responsive** — Mobile, tablet, and desktop ready
- ⚡ **Single File** — No build tools needed, just deploy

---

## Quick Start (Local Preview)

1. Open `index.html` in your browser — it works immediately!

---

## Deploy to GitHub Pages (Free)

### Step 1: Create a GitHub Repository
1. Go to [github.com/new](https://github.com/new)
2. Name it `resume` (or any name you like)
3. Set it to **Public**
4. Click **Create repository**

### Step 2: Push Your Files
```bash
cd resume
git init
git add .
git commit -m "Initial commit - resume website"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/resume.git
git push -u origin main
```

### Step 3: Enable GitHub Pages
1. Go to your repo → **Settings** → **Pages**
2. Under **Source**, select **Deploy from a branch**
3. Choose **main** branch and **/ (root)** folder
4. Click **Save**
5. Your site will be live at: `https://YOUR_USERNAME.github.io/resume`

### Step 4: Update the QR Code URL
In `index.html`, find the QR code `<img>` tag near the bottom and replace `YOUR_GITHUB_USERNAME` with your actual GitHub username:
```
https://api.qrserver.com/v1/create-qr-code/?size=200x200&color=00d4ff&bgcolor=06060e&data=https://YOUR_USERNAME.github.io/resume
```

---

## Setup: Contact Form (Optional)

The contact form uses [Formspree](https://formspree.io) for processing. To enable it:

1. Create a free account at [formspree.io](https://formspree.io)
2. Create a new form
3. Copy your form endpoint (e.g., `https://formspree.io/f/xyzabcde`)
4. In `index.html`, replace `YOUR_FORM_ID` in the form action:
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

> **Note:** Without Formspree configured, the form will gracefully fall back to opening the user's email client with a pre-filled message.

---

## Setup: Downloadable PDF

Place your resume PDF in this folder and name it `resume.pdf`. The download button in the hero section will link to it automatically.

---

## Customization

### Colors
Edit the CSS custom properties at the top of `index.html`:
- `--accent-cyan`: Primary accent color
- `--accent-purple`: Secondary accent color  
- Both dark and light theme palettes are fully customizable

### Content
All resume content is directly in the HTML — search for the section you want to update and edit the text.

---

## Generating a QR Code for Your Business Card

Once deployed, you can print the QR code from the footer, or generate a high-res version at:
```
https://api.qrserver.com/v1/create-qr-code/?size=400x400&data=https://YOUR_USERNAME.github.io/resume
```

---

Built with ❤️ using vanilla HTML, CSS, and JavaScript. No frameworks, no build steps, no dependencies.
