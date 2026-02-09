# How to Deploy to Vercel - EASY METHOD

## ⚡ Quickest Way (GitHub + Vercel Dashboard)

### Step 1: Push to GitHub

```bash
# Initialize git repository
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit - Packers and Movers London"

# Add your GitHub repository
git remote add origin https://github.com/YOUR_USERNAME/packers-and-movers-london.git

# Push to GitHub
git push -u origin main
```

### Step 2: Deploy via Vercel Dashboard

1. Go to **[vercel.com](https://vercel.com)**
2. Click **"Add New Project"**
3. Click **"Import Git Repository"**
4. Select your GitHub repository: `packers-and-movers-london`
5. **IMPORTANT:** In the configuration screen:
   - **Framework Preset:** Select "Other"
   - **Root Directory:** Leave as `./`
   - **Build Command:** Leave EMPTY (delete any default value)
   - **Output Directory:** Leave EMPTY (delete any default value)
   - **Install Command:** Leave as default or empty
6. Click **"Deploy"**

That's it! Vercel will automatically detect your HTML files and deploy them.

---

## 🔧 Alternative: Via Vercel CLI

If you prefer using the command line:

```bash
# Install Vercel CLI
npm install -g vercel

# Login
vercel login

# Deploy
vercel
```

When prompted:
- **Set up and deploy?** → Y
- **Which scope?** → Select your account
- **Link to existing project?** → N
- **What's your project's name?** → packers-and-movers-london
- **In which directory is your code located?** → ./
- **Want to modify these settings?** → N

Then deploy to production:
```bash
vercel --prod
```

---

## 🎯 Your Website URLs

After deployment, your site will be available at:
- `https://packers-and-movers-london.vercel.app`
- `https://packers-and-movers-london-your-username.vercel.app`

### All pages will work:
- Home: `https://your-domain.vercel.app/`
- Services: `https://your-domain.vercel.app/services.html`
- About: `https://your-domain.vercel.app/about.html`
- Contact: `https://your-domain.vercel.app/contact.html`
- Areas: `https://your-domain.vercel.app/areas.html`
- Blog: `https://your-domain.vercel.app/blog.html`

---

## 📝 Files You Need

Make sure you have these files in your project root:
- ✅ index.html
- ✅ services.html
- ✅ about.html
- ✅ contact.html
- ✅ areas.html
- ✅ blog.html
- ✅ styles.css
- ✅ script.js

**DO NOT include:**
- ❌ vercel.json (not needed for simple static sites)
- ❌ package.json (not needed)

---

## 🔄 Continuous Deployment

Once connected to GitHub:
- Every push to `main` branch = automatic deployment
- Vercel gives you preview URLs for each commit
- Easy rollback to previous versions

---

## 🌐 Adding Custom Domain (Optional)

After deployment:
1. Go to your project in Vercel Dashboard
2. Settings → Domains
3. Add domain: `packersandmoverslondon.co.uk`
4. Follow DNS instructions from Vercel
5. Wait for SSL certificate (automatic, takes ~1 minute)

---

## 🐛 Troubleshooting

### If deployment fails:
1. Make sure all HTML files are in the root directory (not in a subdirectory)
2. Check that you don't have a `vercel.json` or `package.json` file
3. Try deploying via Vercel Dashboard (GitHub method) instead of CLI

### Clean URLs (removing .html):
After deployment, go to:
1. Project Settings → General
2. Scroll to "Clean URLs"
3. Enable it

Now your URLs will work as:
- `/services` instead of `/services.html`
- `/about` instead of `/about.html`
- etc.

---

## ✅ Success Checklist

- [ ] All HTML files in root directory
- [ ] No vercel.json or package.json
- [ ] Deployed via Vercel Dashboard or CLI
- [ ] Website is live and loading
- [ ] All pages work
- [ ] CSS and JavaScript loading correctly
- [ ] Mobile responsive working
- [ ] Forms validating properly

---

**Need help?** Vercel has excellent support and documentation at [vercel.com/docs](https://vercel.com/docs)

---

Built with ❤️ for Packers and Movers London
