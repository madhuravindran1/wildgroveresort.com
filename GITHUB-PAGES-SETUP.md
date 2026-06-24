# 🚀 GitHub Pages Setup — Step-by-Step Guide
## Deploy Wild Grove Resort Website (FREE hosting)

---

## STEP 1: Create a GitHub Account (if you don't have one)

1. Go to **[github.com](https://github.com)**
2. Click **Sign Up**
3. Enter your email, create a password, choose a username
4. Verify your email
5. Done!

---

## STEP 2: Create a New Repository

1. Click the **+** icon (top-right) → **New repository**
2. Fill in:
   - **Repository name:** `wildgroveresort.com`  (or any name you like)
   - **Description:** `Wild Grove Resort Website`
   - **Public** ✅ (must be public for free GitHub Pages)
   - **Add a README file** — ❌ Don't check this (we already have one)
3. Click **Create repository**

---

## STEP 3: Upload Your Website Files

1. On the new repository page, click **"uploading an existing file"** link
   (or click **Add file** → **Upload files**)
2. **Drag and drop ALL these files** from the `wildgrove-github-pages` folder:
   - `index.html`
   - `gallery.html`
   - `blog.html`
   - `privacy-policy.html`
   - `CNAME`
   - `README.md`
3. Scroll down → type commit message: `Initial website upload`
4. Click **Commit changes**
5. Wait 10-20 seconds for upload to complete

---

## STEP 4: Enable GitHub Pages

1. Go to your repository → **Settings** (tab at the top)
2. Scroll down to **Pages** (left sidebar)
3. Under **Source**, select:
   - **Branch:** `main`
   - **Folder:** `/ (root)`
4. Click **Save**
5. Wait 1-2 minutes → GitHub will show:
   **"Your site is live at https://yourusername.github.io/wildgroveresort.com/"**

🎉 **Your website is now LIVE!**

---

## STEP 5: Connect Your Custom Domain (wildgroveresort.com)

### A) In GitHub:
1. Still in **Settings → Pages**
2. Under **Custom domain**, enter: `www.wildgroveresort.com`
3. Click **Save**
4. Check **Enforce HTTPS** ✅

### B) In Your Domain Registrar (where you bought wildgroveresort.com):
1. Log into your domain registrar (Hostinger, GoDaddy, Namecheap, etc.)
2. Go to **DNS Settings** for `wildgroveresort.com`
3. **Delete any existing A records** pointing to Zyro/Hostinger builder
4. **Add these 4 A records:**

   | Type | Name | Value |
   |---|---|---|
   | A | @ | 185.199.108.153 |
   | A | @ | 185.199.109.153 |
   | A | @ | 185.199.110.153 |
   | A | @ | 185.199.111.153 |

5. **Add this CNAME record:**

   | Type | Name | Value |
   |---|---|---|
   | CNAME | www | yourusername.github.io |

   *(Replace `yourusername` with your actual GitHub username)*

6. **Save DNS changes**
7. Wait **24-48 hours** for DNS propagation

### C) Verify:
- Visit `https://www.wildgroveresort.com` → should show your new website!
- Visit `https://wildgroveresort.com` → should also work (redirects to www)

---

## ✅ WHAT YOU GET (FREE)

| Feature | Included? |
|---|---|
| Custom domain (wildgroveresort.com) | ✅ Free |
| SSL certificate (HTTPS) | ✅ Free & automatic |
| Global CDN (fast worldwide) | ✅ Free |
| Bandwidth | ✅ 100GB/month (more than enough) |
| Uptime | ✅ 99.9% |
| Cost | ✅ $0 forever |

---

## 🔄 HOW TO UPDATE YOUR WEBSITE LATER

1. Go to your repository on github.com
2. Click on the file you want to update (e.g., `index.html`)
3. Click the **pencil icon** ✏️ (Edit this file)
4. Make your changes
5. Click **Commit changes**
6. Site updates automatically in ~1 minute!

**Or** to replace a whole file:
1. Click **Add file** → **Upload files**
2. Drag the new version of the file
3. Commit → site updates automatically

---

## ⚠️ IMPORTANT NOTES

- **Don't delete the CNAME file** — it tells GitHub to use your custom domain
- **Keep the repository PUBLIC** — GitHub Pages is free only for public repos
- **index.html is your homepage** — GitHub serves it automatically at the root URL
- **Changes go live in ~1 minute** — after every commit
- **Free SSL takes up to 24 hours** — to fully provision after adding custom domain

---

## 🆘 NEED HELP?

If anything doesn't work:
1. Check **Settings → Pages** for error messages
2. Make sure DNS records are correct (use [dnschecker.org](https://dnschecker.org) to verify)
3. Wait 24-48 hours for DNS if you just changed it
4. Come back to Arena.ai and ask me — happy to help debug!
