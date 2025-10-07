# Setup Guide for Simple Telugu Bible Landing Page

## Waitlist Form Setup

The landing page uses Formspree for email collection (free, no backend required).

### Steps:

1. **Go to Formspree**
   - Visit: https://formspree.io/
   - Sign up with your email (free account)

2. **Create a New Form**
   - Click "New Form"
   - Name it: "Simple Telugu Bible Waitlist"
   - Copy the form endpoint (looks like: `https://formspree.io/f/xyzabc123`)

3. **Update index.html**
   - Open `index.html`
   - Find line with: `action="https://formspree.io/f/YOUR_FORM_ID"`
   - Replace `YOUR_FORM_ID` with your actual form ID (just the part after `/f/`)
   - Example: `action="https://formspree.io/f/xyzabc123"`

4. **Test It**
   - Open the site
   - Submit an email
   - Check Formspree dashboard to see submissions

## Deploying to GitHub Pages

Site will be live at: `https://ratchetptnr.github.io/simple-telugu-bible/`

Already handled via git commands in session.

## Updating Changelog

When you make app changes:

1. Edit `CHANGELOG.md`
2. Add new version with date
3. List changes under Added/Changed/Fixed/Removed
4. Commit and push
5. Website updates automatically

## Social Links

Current links in index.html:
- Instagram: https://www.instagram.com/ratchetpotnuru/
- X: https://x.com/ratchet__tweets
- YouTube: https://www.youtube.com/@ratchetpotnuru

Update these if needed.

## Future: Auto-posting to X/Threads

We'll set this up later with GitHub Actions:
- When CHANGELOG.md updates, automatically post to X and Threads
- Requires API access (separate setup)
