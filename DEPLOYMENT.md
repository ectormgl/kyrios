# GitHub Pages Deployment Guide for Kyrios Website

## Quick Deployment Steps

### Option 1: Deploy from VS Code (Recommended)

1. **Initialize Git Repository**
   ```bash
   cd website
   git init
   git add .
   git commit -m "Initial commit: Kyrios website"
   ```

2. **Create GitHub Repository**
   - Go to https://github.com/new
   - Repository name: `kyrios-website` (or your preferred name)
   - Make it Public
   - Do NOT initialize with README (we already have one)
   - Click "Create repository"

3. **Push to GitHub**
   ```bash
   git remote add origin https://github.com/YOUR-USERNAME/kyrios-website.git
   git branch -M main
   git push -u origin main
   ```

4. **Enable GitHub Pages**
   - Go to your repository on GitHub
   - Click "Settings"
   - Scroll to "Pages" in the left sidebar
   - Under "Source", select "main" branch
   - Select "/ (root)" folder
   - Click "Save"
   - Wait 1-2 minutes for deployment

5. **Access Your Site**
   - Your site will be available at: `https://YOUR-USERNAME.github.io/kyrios-website/`
   - GitHub will show you the URL in the Pages settings

### Option 2: Upload via GitHub Web Interface

1. **Create New Repository on GitHub**
   - Go to https://github.com/new
   - Name: `kyrios-website`
   - Public repository
   - Click "Create repository"

2. **Upload Files**
   - Click "uploading an existing file"
   - Drag and drop ALL files from your `website` folder
   - Write commit message: "Initial commit"
   - Click "Commit changes"

3. **Enable GitHub Pages**
   - Go to Settings → Pages
   - Source: main branch, / (root)
   - Save

4. **Wait for Deployment**
   - Check the Actions tab to see deployment progress
   - Site will be live in 1-2 minutes

## Important Notes

✅ **Before Deploying:**
- Update all contact information (email, phone, location)
- Replace WhatsApp number (`15551234567`) with your actual number
- Add your actual project and team images
- Update team member names and roles
- Add your social media links

✅ **After Deploying:**
- Test all links work correctly
- Check mobile responsiveness
- Verify WhatsApp button works
- Test on different browsers

## Custom Domain (Optional)

If you want to use your own domain (e.g., kyrios.ai):

1. **Purchase a domain** from a registrar (Namecheap, GoDaddy, etc.)

2. **Add CNAME file to repository**
   - Create a file named `CNAME` (no extension)
   - Add your domain: `www.kyrios.ai`
   - Commit and push

3. **Configure DNS at your registrar**
   - Add these DNS records:
     ```
     Type: CNAME
     Host: www
     Value: YOUR-USERNAME.github.io
     
     Type: A (for apex domain)
     Host: @
     Values: 
       185.199.108.153
       185.199.109.153
       185.199.110.153
       185.199.111.153
     ```

4. **Enable HTTPS in GitHub Pages settings**

## Updating Your Website

Whenever you make changes:

```bash
cd website
git add .
git commit -m "Description of changes"
git push
```

GitHub Pages will automatically redeploy (takes 1-2 minutes).

## Troubleshooting

**Site not loading?**
- Wait a few minutes after enabling Pages
- Check GitHub Actions tab for deployment status
- Ensure repository is public

**Images not showing?**
- Check file paths are relative (no absolute paths)
- Verify images are in `assets/images/` folder
- Check image filenames match exactly (case-sensitive)

**CSS not loading?**
- Clear browser cache (Ctrl+Shift+R / Cmd+Shift+R)
- Check `css/style.css` path is correct
- Verify files are in correct folders

**404 Error?**
- Ensure `index.html` is in root folder
- Check repository name in URL matches

## Performance Tips

- Compress images before uploading (use TinyPNG.com)
- Keep images under 500KB each
- Test site speed with PageSpeed Insights
- Enable HTTPS for better security and SEO

## SEO Optimization (Optional)

Add these meta tags to `<head>` section:

```html
<meta name="keywords" content="AI, Artificial Intelligence, Machine Learning, AI Consulting">
<meta name="author" content="Kyrios">
<meta property="og:title" content="Kyrios | AI Services & Solutions">
<meta property="og:description" content="Custom AI Agents, Model Development & Consulting">
<meta property="og:image" content="URL_TO_YOUR_LOGO">
```

## Analytics (Optional)

Add Google Analytics to track visitors:

1. Create account at analytics.google.com
2. Get tracking ID (G-XXXXXXXXXX)
3. Add to `<head>` of both HTML files:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

---

Need help? Check GitHub Pages documentation: https://docs.github.com/pages
