# Dinidu Dissanayake — Static Developer Portfolio

A fast, lightweight, and responsive static Software Developer Portfolio built using pure **HTML5, CSS3, and Vanilla JavaScript (ES6+)**. Completely free of Laravel, PHP, or database dependencies.

Designed specifically for zero-cost static hosting on **GitHub Pages, Netlify, Vercel, or Cloudflare Pages**, and ready to share directly on **LinkedIn** and resume profiles.

---

## 📁 Folder Structure

```
portfolio-static/
├── index.html                   <-- Complete static single-page portfolio
├── .nojekyll                    <-- Tells GitHub Pages to serve assets without Jekyll
├── README.md                    <-- Instructions for running and hosting
├── css/
│   └── portfolio.css            <-- Dark navy & cyan glassmorphism design system
├── js/
│   └── portfolio.js             <-- ScrollSpy, project filters, copy toast, contact mailto
├── images/
│   ├── profile.png              <-- Real profile photo from CV
│   ├── profile.jpg
│   └── profile.bmp
└── cv/
    └── Dinidu_Dissanayake_CV.pdf <-- Verified CV file for 1-click download
```

---

## 💻 How to Open and Test Locally

### Method 1: Direct File Open (No Server Needed)
Simply double-click `index.html` in your file explorer, or right-click and choose **Open with Google Chrome** (or Edge / Firefox).
All stylesheet links, images, project badges, and CV download links are relative (`./`) and work directly via `file:///`.

### Method 2: Local Static Web Server (Python / Node / VS Code Live Server)
- Using Python:
  ```powershell
  cd portfolio-static
  python -m http.server 8080
  ```
  Open `http://localhost:8080` in your browser.

- Using VS Code:
  Right-click `index.html` and choose **"Open with Live Server"**.

---

## 🚀 How to Publish for FREE on GitHub Pages

You can host this portfolio online for **100% free** under your personal GitHub URL (e.g. `https://dinidu2002.github.io/portfolio` or `https://dinidu2002.github.io`).

### Option A: Hosting in a New Dedicated GitHub Repository (Recommended)

1. Go to [github.com/new](https://github.com/new) and create a public repository named `portfolio` (or `dinidu-portfolio`).
2. Open PowerShell in this `portfolio-static` folder:
   ```powershell
   cd C:\xampp\htdocs\portfolio\portfolio-static
   ```
3. Initialize git and commit:
   ```powershell
   git init
   git add .
   git commit -m "feat: initial static developer portfolio"
   git branch -M main
   ```
4. Connect to your new repository and push:
   ```powershell
   git remote add origin https://github.com/dinidu2002/portfolio.git
   git push -u origin main
   ```
5. Enable GitHub Pages:
   - On GitHub, go to your repository **Settings** → **Pages** (under "Code and automation").
   - Under **Build and deployment** > **Source**, select **Deploy from a branch**.
   - Under **Branch**, choose `main` and `/ (root)`, then click **Save**.
6. Within 1-2 minutes, your website will be live at:
   👉 **`https://dinidu2002.github.io/portfolio/`**

### Option B: Hosting as your Primary GitHub Profile Website (`username.github.io`)
If you name your repository **`dinidu2002.github.io`**, GitHub will automatically host your portfolio at the root URL:
👉 **`https://dinidu2002.github.io/`**

---

## 🔗 How to Add to Your LinkedIn Profile

Once published on GitHub Pages:
1. Open your **LinkedIn profile**.
2. Click **Add profile section** → **Recommended** → **Add featured**.
3. Click the **+** button → **Add a link**.
4. Paste your GitHub Pages portfolio link (e.g., `https://dinidu2002.github.io/portfolio/`).
5. Title: `Dinidu Dissanayake — Software Developer Portfolio`
6. Description: `Modern developer portfolio showcasing full-stack projects (Foodhub, TaskFlow Pro, AgriConnect), technical stack (PHP, React, Node.js, MySQL), and verified CV.`
7. Click **Save**.

---

## 📧 Contact Form Functionality & Backendless Options

In this static edition:
- When a user submits the form, JavaScript validates the inputs and opens their default email program with a pre-filled message directly to `dissanayakedinidu@gmail.com`.
- It also displays an instant on-screen success confirmation and a **"Copy Message Text"** button so visitors can easily copy their text if using browser-based webmail (like Gmail or Outlook in a tab).

### Optional: Free Direct Email Inbox Delivery (Formspree / Web3Forms)
If you want messages submitted through the form to arrive directly in your Gmail inbox without opening the visitor's mail client:
1. Register for free at [formspree.io](https://formspree.io) or [web3forms.com](https://web3forms.com).
2. Replace the `<form id="contact-form">` tag in `index.html` with:
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
   No backend server or PHP required!
