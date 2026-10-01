# Rock Solid RCC — GitHub Pages Site

This is the multi-page static replacement for the Rock Solid RCC website. It preserves the main public-site sections and service-area URLs while using a responsive, conversion-focused design.

## Main pages
- `/index.html` — Home
- `/what-is-rcc.html` — What is RCC
- `/feedlot-concrete.html` — Feedyard Compacted Concrete
- `/grain-storage-concrete.html` — Grain Storage
- `/parking-lot-concrete.html` — Commercial / Industrial
- `/municipal.html` — Municipal
- `/projects.html` — Projects / Gallery
- `/about.html` — About
- `/contact.html` — Quote / Contact
- `/rcc-service-areas.html` — Service area hub
- `/rcc-service-areas/*.html` — individual city pages

## GitHub Pages
1. Create a GitHub repository and upload the contents of this folder.
2. In **Settings → Pages**, use **GitHub Actions** and the included workflow (`.github/workflows/pages.yml`).
3. In **Settings → Pages → Custom domain**, enter `www.rocksolidrcc.com` and save it. The included `CNAME` file is present, but GitHub still requires the custom domain to be configured in repository settings.
4. In Squarespace DNS, configure the `www` CNAME to the GitHub Pages default domain shown by GitHub. For the apex `rocksolidrcc.com`, use the four GitHub Pages A records shown in GitHub's current documentation if you want the root domain to resolve directly. Keep existing MX/email records intact.
5. Verify the domain and enable HTTPS in GitHub Pages after DNS verification.

## Important before launch
- The image URLs currently reference public Wix-hosted assets from the existing Rock Solid RCC site. If you have original image files, replace those URLs with local files under `assets/` before final production.
- The contact form uses `mailto:` so it works without a server, but a hosted form service can be added later for a more polished submission experience.
- Test every service-area URL and all phone/email links before switching DNS.


### Logo
The supplied Rock Solid RCC logo has been added as optimized transparent PNG assets:
- `assets/rock-solid-logo.png` — full logo
- `assets/rock-solid-wordmark.png` — compact header/footer version
- `assets/favicon.png` — browser icon


### Supplied project photography
Five original aerial/project photographs supplied by Rock Solid RCC were added under `assets/projects/` and placed on the Feedlot and Projects pages. Images are optimized JPEGs for web delivery.


### Supplied grain-storage photography
Five original grain storage/agricultural project photographs supplied in this conversation were added under `assets/projects/` and placed on the Grain Storage and Projects pages.

## Latest update
- Added locally hosted project photography supplied for this build under `assets/projects/customer/`.
- Promoted **Contact Us** to the primary header CTA on every page and added a persistent mobile contact bar.
- The Projects page now uses the supplied field photography rather than relying only on Wix-hosted image URLs.
