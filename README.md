# NerveSec Website

Modern cybersecurity services website with automated deployment workflow.

## Quick Start

1. **Clone locally:**
   ```bash
   git clone https://github.com/n3rv3s3c/nerve-security.git
   cd nerve-security
   ```

2. **Make changes locally** - Edit `index.html` in any text editor

3. **Push to staging for testing:**
   ```bash
   git checkout staging
   git add index.html
   git commit -m "Update: describe your changes"
   git push origin staging
   ```

4. **Review on staging URL** (provided by Vercel)

5. **Merge to main for live deployment:**
   ```bash
   git checkout main
   git merge staging
   git push origin main
   ```

## Development Workflow

- **main** branch → Production (live site)
- **staging** branch → Testing environment
- Both auto-deploy to Vercel on push

## Content You Can Customize

- **Branding**: Search "NERVESEC" to update brand name and logo
- **Services**: Edit the 8 service cards (SVC-01 to SVC-08)
- **About**: Update company mission and philosophy
- **Colors**: CSS variables at top of `<style>` tag (e.g., `--accent: #00f5c4`)
- **Contact Form**: Form fields in contact section

## Deployment Setup (Vercel)

1. Go to **https://vercel.com**
2. Import this GitHub repository
3. Create two deployments:
   - **Production**: Deploy from `main` → your domain
   - **Preview**: Deploy from `staging` → staging URL
4. Enable auto-deploy on push

## File Structure

```
nerve-security/
├── index.html         # Main website (single file)
├── README.md          # This file
└── .gitignore         # Git configuration
```

Everything is self-contained in one HTML file (CSS + JavaScript included).

## Need Help?

- **Edit locally**: Open `index.html` in your browser to preview changes
- **Test live**: Push to `staging` branch and check the Vercel preview URL
- **Deploy**: Merge `staging` to `main` when ready for production

---

Built with vanilla HTML, CSS, and JavaScript. No build process needed.
