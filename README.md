# finalversionv1.com

A brutalist portfolio site that's definitely the final version (until it's not).

## What This Is

A no-nonsense, brutalist portfolio showcasing web development, Meshtastic radio projects, and the general chaos of perpetual tinkering. Built with Tailwind CSS and a healthy dose of self-awareness.

## Files Included

- `index.html` - Main homepage
- `page-template.html` - Template for creating new pages
- `sitemap.xml` - SEO sitemap
- `robots.txt` - Search engine instructions
- `vercel.json` - Vercel deployment config
- `README.md` - This file

## Customization

Before deploying, update these in `index.html`:

### SEO & Meta Tags (IMPORTANT!)
In the `<head>` section, update:
- Line 6: Page title
- Line 7: Meta description (keep under 160 characters)
- Line 8: Keywords
- Line 9: Author name
- Lines 12-16: Open Graph title, description, URL (for social sharing)
- Lines 19-23: Twitter card info
- Line 26: Canonical URL to `https://finalversionv1.com/`
- Lines 40-50: JSON-LD structured data (your name, GitHub URL)

### Contact Info
- Update email address
- Update GitHub username and URL
- Update location if desired

### Projects Section
Replace the three placeholder projects with your actual work:
- Update project names, descriptions, tech stacks
- Add real links to your projects
- Change status badges (ONGOING, ACTIVE, WIP, COMPLETE, etc.)

### Personal Touches
- Add more projects as needed (copy the project div structure)
- Update the "WHO" section with your own voice
- Modify the "WHAT" cards to reflect your specific skills
- Tweak the CHANGELOG with your own version history jokes

## Adding New Pages

Use `page-template.html` as a starting point for new pages:

1. Copy `page-template.html` to a new file (e.g., `my-project.html`)
2. Update the SEO meta tags in the `<head>`
3. Change the page title, breadcrumb, and content
4. Add the new page to `sitemap.xml`
5. Link to it from your homepage or other pages

**Example folder structure:**
```
/
├── index.html
├── about.html
├── projects/
│   ├── meshtastic-setup.html
│   └── website-redesign.html
├── blog/
│   └── first-post.html
├── sitemap.xml
├── robots.txt
└── vercel.json
```

## SEO Setup

### 1. Update sitemap.xml
Add each new page to `sitemap.xml`:
```xml
<url>
  <loc>https://finalversionv1.com/projects/my-project</loc>
  <lastmod>2024-02-12</lastmod>
  <changefreq>monthly</changefreq>
  <priority>0.8</priority>
</url>
```

### 2. Create a favicon
Generate a favicon and save as `favicon.ico` in your root directory. You can use:
- [favicon.io](https://favicon.io)
- [realfavicongenerator.net](https://realfavicongenerator.net)

### 3. Create an OG image
Create a social share image (1200x630px) named `og-image.jpg` and update the OG meta tags with the correct path.

### 4. Submit to search engines
After deploying:
- Submit your sitemap to [Google Search Console](https://search.google.com/search-console)
- Submit to [Bing Webmaster Tools](https://www.bing.com/webmasters)

### 5. Performance optimization (optional)
Consider adding to Vercel deployment:
- Enable automatic compression
- Set up CDN for images
- Add analytics (Vercel Analytics, Google Analytics, etc.)

## Deploy to Vercel

### Quick Deploy (Recommended)

1. Install Vercel CLI:
```bash
npm install -g vercel
```

2. Navigate to your project folder:
```bash
cd path/to/finalversionv1
```

3. Deploy:
```bash
vercel
```

4. Follow the prompts and select:
   - Your Vercel account
   - Create new project
   - Project name: `finalversionv1` (or whatever you prefer)
   - Deploy!

5. Add your custom domain:
   - Go to your Vercel dashboard
   - Click on your project
   - Settings → Domains
   - Add `finalversionv1.com`
   - Follow the DNS instructions from your domain registrar

### Alternative: GitHub → Vercel

1. Create a new GitHub repo
2. Push your code:
```bash
git init
git add .
git commit -m "v1.0.0 - definitely final"
git branch -M main
git remote add origin https://github.com/yourusername/finalversionv1.git
git push -u origin main
```

3. Connect to Vercel:
   - Go to [vercel.com](https://vercel.com)
   - Import your GitHub repo
   - Deploy
   - Add your custom domain in project settings

## Domain Setup (finalversionv1.com)

Once deployed to Vercel, you'll need to point your domain:

1. In Vercel project settings, add domain: `finalversionv1.com`
2. Vercel will provide DNS records
3. Go to your domain registrar (where you bought the domain)
4. Update DNS settings with Vercel's nameservers or A/CNAME records
5. Wait for DNS propagation (can take a few hours)

## Local Testing

Just open `index.html` in your browser, or run a local server:

```bash
# Python
python -m http.server 8000

# Node.js
npx serve

# PHP
php -S localhost:8000
```

Then visit `http://localhost:8000`

## Features

- ✅ Brutalist design (thick borders, bold typography, in-your-face colors)
- ✅ Fully responsive (works on mobile, tablet, desktop)
- ✅ Self-deprecating humor built-in
- ✅ Monospace font (Courier New) for that dev aesthetic
- ✅ Hover effects on project cards
- ✅ Console easter egg (check your browser console)
- ✅ Zero JavaScript frameworks (just vanilla JS)
- ✅ No build step required

## Tech Stack

- HTML5
- Tailwind CSS (via CDN)
- Vanilla JavaScript
- Pure comedy gold

## Philosophy

This site embraces the "work in progress" nature of all personal projects. The brutalist design is intentional - raw, honest, and doesn't try to be something it's not. Just like the domain name suggests, it's self-aware about being perpetually in v1.

## License

Do whatever you want with it. It's the internet. ¯\_(ツ)_/¯

---

**Note:** Remember to update your contact info before deploying. Unless you want random people emailing `your.email@example.com`, which would be funny but not useful.
