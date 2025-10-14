# KYRIOS - AI Services Website

Welcome to the Kyrios website! This is a modern, responsive static website built with pure HTML and CSS.

## 🎨 Design Overview

- **Color Scheme**: Black (#0a0a0a), Yellow (#FFF82C), Cyan (#00E5FF)
- **Typography**: Android (headings), Roboto (body text)
- **Style**: Modern, minimalist, professional

## 📁 Project Structure

```
website/
├── index.html          # Main landing page
├── blog.html           # Blog/News page
├── css/
│   ├── style.css       # Main stylesheet
│   └── blog.css        # Blog-specific styles
├── js/
│   └── script.js       # JavaScript functionality
└── assets/
    └── images/         # All images and logos
```

## 🚀 Features

### Main Page (index.html)
- **Hero Section**: Eye-catching landing with animated logo
- **About Section**: Company overview with animated statistics
- **Services Section**: Two featured services (AI Agent Development & Consulting)
- **Portfolio Section**: Showcase of 3 client projects
- **Team Section**: Team member profiles
- **Contact Section**: Contact information and WhatsApp integration

### Blog Page (blog.html)
- **Blog Posts**: Grid layout with featured and regular posts
- **Sidebar**: Search, categories, recent posts, newsletter signup, tags
- **Pagination**: Navigate through blog posts

### Interactive Features
- Smooth scrolling navigation
- Mobile-responsive menu
- Animated elements on scroll
- WhatsApp floating button
- Active navigation highlighting

## 📱 WhatsApp Integration

The website includes WhatsApp contact functionality:
- Floating WhatsApp button (bottom-right)
- Contact section with WhatsApp button
- **IMPORTANT**: Update the phone number in these files:
  - `index.html` (search for `15551234567` and replace)
  - `blog.html` (search for `15551234567` and replace)

Format: `https://wa.me/PHONENUMBER` (include country code, no + or spaces)
Example: `https://wa.me/5511999998888` for Brazil

## ✏️ Customization Guide

### 1. Update Contact Information

**In `index.html`, find and update:**

```html
<!-- Email -->
<p>contact@kyrios.ai</p>

<!-- Phone -->
<p>+1 (555) 123-4567</p>

<!-- Location -->
<p>San Francisco, CA</p>

<!-- WhatsApp -->
href="https://wa.me/15551234567..."
```

### 2. Add Your Images

Replace placeholder images in `assets/images/`:

**Required Images:**
- `logo-symbol.svg` - Already included (your logo)
- `client-1.jpg` - Portfolio image 1 (recommended: 800x500px)
- `client-2.jpg` - Portfolio image 2 (recommended: 800x500px)
- `client-3.jpg` - Portfolio image 3 (recommended: 800x500px)
- `team-1.jpg` - Team member photo (recommended: 400x400px)
- `team-2.jpg` - Team member photo (recommended: 400x400px)
- `team-3.jpg` - Team member photo (recommended: 400x400px)

**Blog Images (optional):**
- `blog-featured.jpg` - Featured post (1200x600px)
- `blog-1.jpg` to `blog-5.jpg` - Blog posts (800x400px)
- `blog-thumb-1.jpg` to `blog-thumb-3.jpg` - Thumbnails (150x150px)

### 3. Update Team Information

In `index.html`, find the Team Section and update:

```html
<h4 class="member-name">Your Name</h4>
<p class="member-role">Your Role</p>
```

### 4. Modify Services

To add or modify services, edit the Services Section in `index.html`. Each service uses this structure:

```html
<div class="service-card featured">
    <div class="service-icon">
        <!-- SVG icon here -->
    </div>
    <h3 class="service-title">Service Name</h3>
    <p class="service-description">Description...</p>
    <ul class="service-features">
        <li>Feature 1</li>
        <li>Feature 2</li>
    </ul>
</div>
```

### 5. Update Blog Posts

In `blog.html`, each blog post follows this structure:

```html
<article class="blog-post">
    <div class="post-image">
        <img src="assets/images/blog-1.jpg" alt="Blog Post">
    </div>
    <div class="post-content">
        <div class="post-meta">
            <span class="post-category">Category</span>
            <span class="post-date">Date</span>
        </div>
        <h3 class="post-title">Post Title</h3>
        <p class="post-excerpt">Post excerpt...</p>
        <a href="#" class="post-link">Read More →</a>
    </div>
</article>
```

### 6. Update Social Media Links

Find and replace `#` with your actual social media URLs:

```html
<!-- LinkedIn -->
<a href="YOUR_LINKEDIN_URL" aria-label="LinkedIn">

<!-- Twitter -->
<a href="YOUR_TWITTER_URL" aria-label="Twitter">

<!-- Instagram -->
<a href="YOUR_INSTAGRAM_URL" aria-label="Instagram">
```

## 🌐 Deployment to GitHub Pages

1. **Create a new repository** on GitHub
2. **Push your website folder** to the repository
3. **Enable GitHub Pages**:
   - Go to repository Settings
   - Scroll to "Pages" section
   - Select "main" branch as source
   - Select "/ (root)" folder
   - Click Save
4. Your site will be live at: `https://yourusername.github.io/repository-name/`

### Important for GitHub Pages:
- Make sure `index.html` is in the root directory
- All file paths should be relative (already set up)
- Images must be in the `assets/images/` folder

## 🔧 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📝 Notes

- The website is fully responsive and mobile-friendly
- All animations are optimized for performance
- The design follows your brand guidelines (yellow #FFF82C and cyan #00E5FF)
- No external dependencies required (except Google Fonts)
- Static website - no backend required

## 🎯 Future Enhancements (Optional)

If you want to add more features later:
- Contact form with backend integration
- Blog CMS integration
- Live chat widget
- Analytics tracking (Google Analytics)
- SEO optimization
- Performance optimization

## 📞 Support

For any questions about the website:
- Review the code comments in HTML/CSS files
- All sections are clearly labeled
- Check the console for any errors (F12 in browser)

---

**Built with ❤️ for Kyrios AI Services**

Last Updated: October 14, 2025
