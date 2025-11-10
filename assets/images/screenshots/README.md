# Wolfralyze Website Screenshots

This directory contains screenshots displayed on https://wolfralyze.org in the "See Wolfralyze in Action" section.

## Screenshot Files

The following screenshots should be placed in this directory:

1. **01-dashboard-overview.png** - SonarQube project dashboard
2. **02-issues-list.png** - Issues list with Mathematica violations
3. **03-code-with-issue.png** - Code viewer with syntax highlighting
4. **04-rule-detail.png** - Rule documentation page
5. **05-quality-profile.png** - Quality profile showing 529+ rules
6. **06-plugin-installed.png** - Plugin in marketplace

## Adding Screenshots

After taking screenshots following the guide in `/Users/bceverly/dev/wolfralyze/docs/images/screenshots/README.md`:

```bash
# Copy screenshots from the main repo to the website
cp /Users/bceverly/dev/wolfralyze/docs/images/screenshots/*.png \
   /Users/bceverly/dev/wolfralyze-docs/assets/images/screenshots/
```

Or copy from your desktop:

```bash
cp ~/Desktop/01-dashboard-overview.png ./
cp ~/Desktop/02-issues-list.png ./
cp ~/Desktop/03-code-with-issue.png ./
cp ~/Desktop/04-rule-detail.png ./
cp ~/Desktop/05-quality-profile.png ./
cp ~/Desktop/06-plugin-installed.png ./
```

## Screenshot Specifications

- **Format:** PNG (preferred for screenshots)
- **Recommended width:** 1200-1600px (will be responsive)
- **Quality:** High quality, readable text
- **Theme:** Light theme preferred for consistency
- **Compression:** Use moderate compression to balance quality and file size

## Display on Website

Screenshots are displayed in a responsive grid (index.html):
- Desktop: 3 columns
- Tablet: 2 columns
- Mobile: 1 column

Each screenshot includes:
- Title
- Description
- Hover effect (slight lift and shadow)
- Lazy loading for performance

## Testing

After adding screenshots, test the website locally:

```bash
cd /Users/bceverly/dev/wolfralyze-docs
open index.html
```

Or use a simple HTTP server:

```bash
python3 -m http.server 8000
# Then open http://localhost:8000
```

## Placeholder Images

If screenshots are not yet available, the website will show broken image icons. This is normal during development. The layout and styling are already in place and will work correctly once screenshots are added.

---

**Note:** These screenshots are synced from the main wolfralyze repository. When updating screenshots, update them in both locations.
