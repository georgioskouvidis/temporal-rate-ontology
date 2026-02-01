# Temporal Rate Ontology Website

This repository contains the source code for the Temporal Rate Ontology (TRO) website, hosted via GitHub Pages.

## Website URL

Once deployed, your site will be available at: `https://[your-username].github.io/temporal-rate-ontology/`

Or with a custom domain: `https://temporalrateontology.com` (if configured)

## Setup Instructions

### 1. Create GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in (create account if needed)
2. Click the "+" icon in top right → "New repository"
3. Name it: `temporal-rate-ontology`
4. Make it **Public**
5. Check "Add a README file"
6. Click "Create repository"

### 2. Upload Website Files

**Option A: Web Interface (Easiest)**
1. In your repository, click "Add file" → "Upload files"
2. Drag and drop these three files:
   - `index.html`
   - `styles.css`
   - `script.js`
3. Scroll down and click "Commit changes"

**Option B: Git Command Line**
```bash
git clone https://github.com/[your-username]/temporal-rate-ontology.git
cd temporal-rate-ontology
# Copy the three files (index.html, styles.css, script.js) into this folder
git add .
git commit -m "Initial website files"
git push
```

### 3. Enable GitHub Pages

1. In your repository, go to "Settings" tab
2. Scroll down to "Pages" in left sidebar
3. Under "Source", select:
   - Branch: `main`
   - Folder: `/ (root)`
4. Click "Save"
5. Wait 2-3 minutes for deployment
6. Your site will be live at: `https://[your-username].github.io/temporal-rate-ontology/`

### 4. Update Content

Before going live, update these items in `index.html`:

**Required Updates:**
- Replace `XXXXXXX` in Zenodo DOI links with actual DOI numbers
- Replace `XXXXX` in PhilSci Archive links with actual archive IDs
- Replace `XXXX-XXXX-XXXX-XXXX` with your actual ORCID ID
- Update publication status when papers are accepted

**Once Papers Published:**
- Change "Forthcoming" to actual publication info
- Add DOI links for published versions
- Update year if needed

## File Structure

```
temporal-rate-ontology/
├── index.html          # Main website content
├── styles.css          # Styling and design
├── script.js           # Interactive features
└── README.md          # This file
```

## Customization

### Colors
Edit color variables in `styles.css` (lines 3-12):
```css
:root {
    --primary-color: #1a5490;      /* Main blue */
    --secondary-color: #2e7bc4;    /* Lighter blue */
    --accent-color: #5a9fd4;       /* Accent blue */
    /* etc. */
}
```

### Content
All content is in `index.html`. Sections:
- **Overview**: Main description of TRO
- **Papers**: List of publications
- **FAQ**: Common questions
- **Contact**: Your contact info

### Adding New Sections
1. Add section in `index.html`:
```html
<section id="newsection">
    <h2>New Section Title</h2>
    <p>Content here...</p>
</section>
```

2. Add navigation link:
```html
<nav>
    <div class="container">
        <a href="#overview">Overview</a>
        <!-- ... -->
        <a href="#newsection">New Section</a>
    </div>
</nav>
```

## Custom Domain (Optional)

To use `temporalrateontology.com` instead of GitHub's default URL:

1. Purchase domain from registrar (Namecheap, Google Domains, etc.)
2. Add these DNS records at your registrar:
   ```
   Type: A
   Host: @
   Value: 185.199.108.153
   
   Type: A
   Host: @
   Value: 185.199.109.153
   
   Type: A
   Host: @
   Value: 185.199.110.153
   
   Type: A
   Host: @
   Value: 185.199.111.153
   
   Type: CNAME
   Host: www
   Value: [your-username].github.io
   ```
3. In GitHub Settings → Pages, enter custom domain
4. Enable "Enforce HTTPS"
5. Wait 24-48 hours for DNS propagation

## Maintenance

### Regular Updates Needed:
- Paper publication status
- New papers added
- Contact information
- FAQ answers as common questions emerge

### Analytics (Optional):
To track visitors, add Google Analytics or similar:
1. Get tracking code
2. Add to `<head>` of `index.html`

## Support

For GitHub Pages issues: https://docs.github.com/en/pages
For questions about the website: georgioskouvidis@gmail.com

## License

Content: © 2026 Georgios Kouvidis
Website code: MIT License (free to use and modify)
