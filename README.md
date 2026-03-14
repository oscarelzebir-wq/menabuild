# Menabuild Professional Builders — Website

## Files Included
- `index.html` — Home page
- `about.html` — About Us
- `services.html` — Services
- `renovation.html` — Renovation
- `gallery.html` — Gallery
- `reviews.html` — Reviews
- `contact.html` — Contact
- `style.css` — All styles
- `script.js` — Navigation, animations, form
- `images/` — PUT YOUR IMAGES HERE

## Before Going Live — Update These

1. **Logo**: Place your logo file at `images/logo.png`
2. **Phone number**: Search & replace `(305) 555-0000` with your real number
3. **Email**: Search & replace `info@menabuild.com` with your real email
4. **Hero image**: In `index.html`, replace the `.hero__bg-placeholder` div with:
   `<img src="images/hero.jpg" alt="Menabuild custom home" />`
5. **Photos**: Replace all `img-placeholder` divs in gallery and pages with real `<img>` tags
6. **Contact form**: Add your Formspree ID or backend endpoint to the form `action` attribute
7. **Google Maps**: In `contact.html`, replace the map div with your Google Maps embed iframe

## How to Add Photos

Replace any placeholder div like this:
```html
<div class="gallery-grid__item img-placeholder"><span>Add Photo</span></div>
```
With:
```html
<div class="gallery-grid__item"><img src="images/your-photo.jpg" alt="Description" /></div>
```

## How to Deploy (Free Options)

### Option A: Netlify (Recommended — Free)
1. Go to netlify.com → Sign up free
2. Drag & drop the entire `menabuild` folder onto the Netlify dashboard
3. Your site is live instantly at a `.netlify.app` URL
4. Add your custom domain (menabuild.com) in settings

### Option B: GitHub Pages (Free)
1. Create a GitHub account and new repository
2. Upload all files
3. Go to Settings → Pages → Deploy from main branch
4. Live at `yourusername.github.io/menabuild`

### Option C: Any Web Host
Upload all files via FTP to your hosting provider's `public_html` folder.

## Custom Domain
Once deployed, point your domain's DNS:
- A record → your host's IP address, OR
- CNAME → your netlify/github URL

## Connect the Contact Form (Free)
1. Go to formspree.io → Create free account
2. Create a new form → Copy the endpoint URL
3. In `contact.html`, change:
   `<form action="#" method="POST">`
   to:
   `<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">`
4. Form submissions go straight to your email!
