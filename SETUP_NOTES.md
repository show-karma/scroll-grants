# Scroll Grants Website Setup Notes

This website has been created by adapting the Optimism Grants Council site for Scroll.

## Completed Changes

### 1. Content Updates
- Replaced all "Optimism" references with "Scroll"
- Replaced "Growth Grants" with "Community Grants" throughout the site
- Updated social media links to Scroll's official accounts (Twitter: @Scroll_ZKP)
- Updated external links to point to Scroll domains

### 2. Branding Updates
- Primary color: `#ffeeda` (Scroll primary)
- Light color: `#F18740`
- Background: `#FFF8F3`
- Updated all CSS variables in `assets/scss/common/_variables-custom.scss`
- Updated navbar logo color

### 3. Configuration
- Updated `config/_default/hugo.toml` with Scroll branding
- Updated `config/_default/params.toml` with Scroll info
- Updated menu items in `config/_default/menus/menus.en.toml`
- Updated CNAME to `grants.scroll.io`

### 4. Visual Assets
- Downloaded official Scroll favicon from scroll.io (`static/favicon.ico`)
- Downloaded official Scroll logo PNG from scroll.io (`static/apple-touch-icon.png`)
- Downloaded Scroll OG image from scroll.io (`static/cover.jpg`)
- Created "S" logo in SVG format for additional icons
- Logo colors match Scroll brand (#ffeeda background, #FFF8F3 text)

## Action Items for Manual Update

### Visual Assets Status
✅ **Downloaded from scroll.io:**
- `/static/favicon.ico` - Official Scroll favicon
- `/static/apple-touch-icon.png` - Official Scroll logo (180x180 PNG)
- `/static/cover.jpg` - Official Scroll OG image (1774x716 PNG)
- `/assets/favicon.png` - Copy of official Scroll logo

✏️ **Custom SVG Placeholders:**
- `/static/icon.svg` - Placeholder "S" logo with Scroll branding
- `/assets/favicon.svg` - Placeholder "S" logo with Scroll branding
- `/static/scroll-logo.svg` - Placeholder Scroll text logo

### Optional Improvements
1. **Replace SVG Placeholders:**
   If you have vector versions of the Scroll logo, replace the placeholder SVG files:
   - `/static/icon.svg`
   - `/assets/favicon.svg`
   - `/static/scroll-logo.svg`

2. **Other Assets:**
   - `/static/karma-logo.svg` - Consider removing or replacing if not needed

### URL Updates Needed
Some placeholder URLs may need to be updated once Scroll's grant system is live:
- Application URLs in `/layouts/home.html` currently point to Season 8 page
- Menu grant links in `/config/_default/menus/menus.en.toml`
- Grant platform URLs (currently using placeholder karma URLs)

### Testing Before Deployment
1. Install dependencies: `npm install`
2. Run local dev server: `hugo server`
3. Check all pages render correctly
4. Verify all links work
5. Test responsive design on mobile
6. Replace placeholder URLs with actual grant application URLs

## Scroll Brand Colors Reference
- Primary: #ffeeda
- Light: #F18740
- Dark: #FFDEB5
- Background: #FFF8F3
- Secondary: #595959

## Social Links
- Twitter: https://twitter.com/Scroll_ZKP
- Discord: https://discord.gg/scroll
- GitHub: https://github.com/scroll-tech
- Website: https://scroll.io/
