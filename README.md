# ☀️ FOUNDRY

**Stop Guessing. Start Building.**

FOUNDRY is an entrepreneur growth platform that provides FREE templates, tools, and training to help aspiring solopreneurs and small business owners launch and grow their businesses.

---

## 🎯 What is FOUNDRY?

FOUNDRY gives you the exact blueprints you need to build a successful business:

- **8 Free Business Templates** - Business Model Canvas, One-Page Business Plan, Revenue Tracker, and more
- **7-Day Business Builder Course** - Go from idea to launch in one week
- **Interactive Tools** - Pricing Calculator, Break-Even Calculator
- **Zero Fluff** - Only proven frameworks that actually work

**Philosophy:** "Give away the blueprints. Charge for the building."

---

## 🚀 Quick Start

### Option 1: Deploy to GitHub Pages (Recommended)

1. **Create a new GitHub repository**
   ```bash
   # Navigate to the FOUNDRY folder
   cd ~/clawd/Projects/FOUNDRY
   
   # Initialize git repository
   git init
   git add .
   git commit -m "Initial commit - FOUNDRY platform"
   ```

2. **Push to GitHub**
   ```bash
   # Create a new repo on GitHub (https://github.com/new)
   # Then connect it:
   git remote add origin https://github.com/YOUR-USERNAME/FOUNDRY.git
   git branch -M main
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to your repository settings
   - Navigate to **Pages** section
   - Under "Source", select `main` branch
   - Click **Save**
   - Your site will be live at: `https://YOUR-USERNAME.github.io/FOUNDRY/`

**That's it!** Your site is now live and deployable.

---

### Option 2: Deploy to Netlify

1. **Drag & Drop** the FOUNDRY folder to [Netlify Drop](https://app.netlify.com/drop)
2. Your site goes live instantly
3. Optional: Connect to GitHub for automatic updates

---

### Option 3: Deploy to Vercel

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
cd ~/clawd/Projects/FOUNDRY
vercel
```

Follow the prompts and your site will be live in seconds.

---

## 📁 Project Structure

```
FOUNDRY/
├── index.html              # Landing page
├── templates.html          # Templates gallery
├── course.html            # Mini-course page
├── tools.html             # Interactive calculators
├── about.html             # About page
├── templates/             # Free downloadable templates
│   ├── business-model-canvas.md
│   ├── one-page-business-plan.md
│   ├── weekly-revenue-tracker.md
│   ├── content-calendar-30-days.md
│   ├── customer-avatar-worksheet.md
│   ├── pricing-strategy-calculator.md
│   ├── launch-checklist.md
│   └── email-sequence-templates.md
├── course/                # Mini-course lessons
│   ├── day-1.html
│   ├── day-2.html
│   └── day-3.html
└── README.md              # This file
```

---

## ✨ Features

### Landing Page (`index.html`)
- Pain-first messaging
- Email capture (localStorage)
- Testimonials section
- 3-tier pricing preview (Free / Pro / Elite)
- Dark theme with gold accents

### Templates Gallery (`templates.html`)
- 8 comprehensive business templates
- All downloadable as markdown files
- Real, useful content (not filler)

### Mini-Course (`course.html`)
- 7-Day Business Builder course
- Days 1-3 free, Days 4-7 locked behind email gate
- Full lesson content included

### Tools (`tools.html`)
- **Pricing Calculator**: Calculate optimal pricing based on costs and positioning
- **Break-Even Calculator**: Determine how many sales you need to break even
- Interactive, real-time calculations

### About Page (`about.html`)
- Founder story
- Rama Rajya philosophy
- Mission and values

---

## 🎨 Design System

**Colors:**
- Background: `#0a0a0a` (near-black)
- Accents: `#f59e0b` (amber/gold)
- Text: Gray scale (100-900)

**Typography:**
- Font: Inter (Google Fonts)
- Responsive, mobile-first

**Framework:**
- Tailwind CSS (via CDN)
- Pure HTML/CSS/JS (no build step required)

---

## 🔧 Customization

### Update Email Capture

Currently stores emails in `localStorage`. To connect to a backend:

1. **Supabase Integration:**
   ```javascript
   // In index.html, replace localStorage with:
   const { data, error } = await supabase
     .from('emails')
     .insert([{ email: email }])
   ```

2. **ConvertKit/Mailchimp:**
   - Add API endpoint
   - Replace form submission handler

### Add More Templates

1. Create a new `.md` file in `/templates/`
2. Add a card in `templates.html`
3. Link to the new file

### Customize Colors

Change Tailwind classes:
- `bg-[#0a0a0a]` → your background color
- `text-amber-500` → your accent color
- `border-amber-500` → your border color

---

## 🚦 Testing Locally

**Option 1: Python Server**
```bash
cd ~/clawd/Projects/FOUNDRY
python3 -m http.server 8000
# Open http://localhost:8000
```

**Option 2: PHP Server**
```bash
php -S localhost:8000
```

**Option 3: VS Code Live Server**
- Install "Live Server" extension
- Right-click `index.html` → "Open with Live Server"

---

## 📊 Analytics (Optional)

Add Google Analytics:

```html
<!-- Add to <head> in all HTML files -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

---

## 🔐 Environment Setup (Future)

When you add backend features:

1. Create `.env` file:
   ```
   SUPABASE_URL=your_supabase_url
   SUPABASE_KEY=your_supabase_key
   STRIPE_KEY=your_stripe_key
   ```

2. Add `.gitignore`:
   ```
   .env
   node_modules/
   .DS_Store
   ```

---

## 🛠️ Future Enhancements

**Phase 2 (Backend Integration):**
- [ ] Supabase for email storage
- [ ] Stripe for payments
- [ ] User authentication
- [ ] Member dashboard

**Phase 3 (Advanced Features):**
- [ ] AI content generator
- [ ] Advanced analytics
- [ ] Community forum
- [ ] 1-on-1 coaching scheduler

**Phase 4 (Scale):**
- [ ] Mobile app
- [ ] API for third-party integrations
- [ ] Affiliate program
- [ ] Premium templates marketplace

---

## 📝 Content Updates

To update templates or course content:

1. Edit the `.md` files in `/templates/` or HTML files in `/course/`
2. Commit and push to GitHub
3. GitHub Pages auto-deploys (or manually deploy to Netlify/Vercel)

---

## 🐛 Troubleshooting

**Templates not downloading:**
- Ensure browser allows downloads from localhost
- Use a real server (GitHub Pages) for production

**Calculators not working:**
- Check browser console for JavaScript errors
- Ensure all input IDs match the script

**Email gate not unlocking:**
- Check browser localStorage
- Try clearing cache

---

## 📄 License

© 2026 Divine Success Flow. All rights reserved.

This project is proprietary. Unauthorized copying, distribution, or use is prohibited.

---

## 🤝 Contributing

This is a proprietary project for Divine Success Flow. Not accepting external contributions at this time.

---

## 📧 Contact

**Founder:** Yashaswi  
**Brand:** Divine Success Flow  
**Website:** [Your Domain]

For support or inquiries: [Your Email]

---

## 🙏 Acknowledgments

Built with:
- [Tailwind CSS](https://tailwindcss.com/)
- [Inter Font](https://fonts.google.com/specimen/Inter)
- [GitHub Pages](https://pages.github.com/)

Inspired by entrepreneurs everywhere who are building the future.

---

**Made with ☀️ by Divine Success Flow**

*"Stop Guessing. Start Building."*
