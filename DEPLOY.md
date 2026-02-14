# 🚀 FOUNDRY Deployment Checklist

## ✅ Pre-Deployment Checklist

Before deploying, verify:

- [x] All HTML files are created
- [x] All templates are written with real content
- [x] Course pages (Days 1-3) are complete
- [x] Tools calculators are functional
- [x] About page is complete
- [x] README.md has deployment instructions
- [x] All internal links work
- [x] Mobile responsive (test in browser DevTools)

---

## 🌐 Deploy to GitHub Pages (5 minutes)

### Step 1: Create GitHub Repository

```bash
cd ~/clawd/Projects/FOUNDRY
git init
git add .
git commit -m "Initial commit - FOUNDRY platform"
```

### Step 2: Push to GitHub

1. Go to https://github.com/new
2. Create a new repository named `FOUNDRY` (or any name)
3. Don't initialize with README (we already have one)
4. Run these commands:

```bash
git remote add origin https://github.com/YOUR-USERNAME/FOUNDRY.git
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to repository **Settings**
2. Scroll to **Pages** section (left sidebar)
3. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
4. Click **Save**
5. Wait 1-2 minutes for deployment

✨ **Your site is now live at:**
`https://YOUR-USERNAME.github.io/FOUNDRY/`

---

## 🔗 Custom Domain (Optional)

### If you have a domain:

1. Add a `CNAME` file to root:
   ```
   foundry.yourdomain.com
   ```

2. In your domain DNS settings, add:
   - Type: `CNAME`
   - Name: `foundry`
   - Value: `YOUR-USERNAME.github.io`

3. In GitHub Pages settings, add custom domain: `foundry.yourdomain.com`

---

## 🧪 Test Checklist

After deployment, test these:

### Navigation
- [ ] All nav links work
- [ ] Logo links to home
- [ ] Mobile menu works (if added)

### Landing Page
- [ ] Hero section loads
- [ ] Email form stores to localStorage
- [ ] "Get Started" buttons work
- [ ] Pricing section displays correctly
- [ ] Footer links work

### Templates Page
- [ ] All 8 templates display
- [ ] Download buttons work
- [ ] Template files download correctly

### Course Page
- [ ] Days 1-3 are accessible
- [ ] Days 4-7 show lock icon
- [ ] Email gate modal opens
- [ ] Unlocking works after email submission
- [ ] Course content is readable

### Tools Page
- [ ] Pricing calculator works
- [ ] Break-even calculator works
- [ ] Results update in real-time
- [ ] Mobile layout is usable

### About Page
- [ ] All sections display
- [ ] Text is readable
- [ ] Philosophy section looks good

---

## 📊 Analytics Setup (Optional)

### Add Google Analytics:

1. Get your GA4 Measurement ID
2. Add to `<head>` of all HTML files:

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

## 🔄 Future Updates

To update the site:

```bash
# Make your changes
git add .
git commit -m "Update: description of changes"
git push

# GitHub Pages will auto-deploy in 1-2 minutes
```

---

## 🆘 Troubleshooting

### Site not loading:
- Wait 2-3 minutes after enabling Pages
- Check repository is public
- Verify branch is set to `main`

### Templates not downloading:
- Make sure you're using HTTPS (not localhost)
- Check browser download settings

### Calculators not working:
- Open browser console (F12)
- Check for JavaScript errors
- Ensure all input IDs match

### Email gate not unlocking:
- Clear browser cache
- Try incognito mode
- Check localStorage in DevTools

---

## 🎉 Launch Announcement

Once deployed, announce on:

- [ ] Twitter/X
- [ ] LinkedIn
- [ ] Instagram
- [ ] Reddit (r/Entrepreneur, r/SideProject)
- [ ] Product Hunt
- [ ] Indie Hackers

**Sample Tweet:**
```
🚀 Just launched FOUNDRY — free templates, tools, and training for entrepreneurs

✅ 8 business templates
✅ 7-day course
✅ Interactive calculators
✅ 100% free

Stop guessing. Start building.

👉 [your-link]

#buildinpublic #solopreneur
```

---

## 📈 Next Steps

### Week 1:
- Monitor analytics
- Collect email signups
- Engage with users
- Fix any bugs

### Week 2-4:
- Add testimonials (real ones from users)
- Create social media content
- Write blog posts for SEO
- Launch on Product Hunt

### Month 2:
- Build Days 4-7 of course
- Create premium templates
- Set up Stripe for payments
- Launch Pro tier

---

## 🎯 Success Metrics

Track these weekly:

| Metric | Week 1 | Week 2 | Week 3 | Week 4 |
|--------|--------|--------|--------|--------|
| Visitors | | | | |
| Email signups | | | | |
| Template downloads | | | | |
| Course starts | | | | |
| Social shares | | | | |

---

**Made with ☀️ by Divine Success Flow**

*You've got this. Now go launch!*
