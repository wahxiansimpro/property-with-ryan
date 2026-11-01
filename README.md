# Property With Ryan — website starter

A responsive static website built with HTML, CSS and vanilla JavaScript. No database or build tools required.

## Run locally
1. Extract the ZIP.
2. Open `index.html` in a browser, or use VS Code's Live Server extension.
3. Edit `index.html`, `css/style.css` and `js/script.js` as needed.

## Before publishing — important checklist
- Replace both `ADD RYAN'S PROFESSIONAL PHOTO` placeholders with Ryan's approved professional portrait. Use a locally stored image, e.g. `assets/ryan-profile.jpg`, and update the relevant CSS/HTML.
- Add the official PropNex logo only if Ryan/PropNex has approved its use. The current header uses a simple Property With Ryan house mark and text branding.
- Confirm the agency's exact registered legal name, REN details and any required advertising/disclosure wording with the agency/compliance team.
- Add real property listings only after confirming permission to advertise, availability, price, photos and property details. The first version intentionally has no invented listings.
- Replace the generic hero and YouTube section background photos with Ryan's own licensed photography if desired. Current images are remote Unsplash images and require internet access.
- Add real client testimonials only with permission. The site currently links to Ryan's Facebook reviews instead of reproducing them.
- Confirm all contact and social links before launch.

## Add a property listing
Copy this card structure into the `#listingGrid` element in `index.html` and replace the placeholder content. Use `data-category="sale"`, `"rent"` or `"new"` for the filters.

```html
<article class="property-card" data-category="sale">
  <img src="assets/property-01.jpg" alt="Living room of property in Petaling Jaya" loading="lazy">
  <div class="property-card-body">
    <span class="property-tag">FOR SALE</span>
    <h3>Property title</h3>
    <p>Location · Property type</p>
    <strong>RM [confirmed asking price]</strong>
    <a href="https://wa.me/60137701082?text=Hi%20Ryan%2C%20I%27m%20interested%20in%20[PROPERTY]." target="_blank" rel="noopener">Enquire on WhatsApp</a>
  </div>
</article>
```

You will also want to add styles for `.property-card`, `.property-card img`, `.property-card-body` and `.property-tag` in `css/style.css`.

## Deploy
Recommended: GitHub repository + GitHub Pages for a simple static site, or Cloudflare Pages / Netlify. Connect the repository, select the root folder as the site source, and add a custom domain when ready. No server-side runtime is required.
