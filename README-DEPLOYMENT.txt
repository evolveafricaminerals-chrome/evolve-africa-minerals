# Evolve Africa Minerals — Website files

This is a custom-coded, responsive, single-page corporate website for Evolve Africa Minerals. It is built with plain HTML, CSS and JavaScript so it can be hosted on GitHub Pages without a framework or build process.

## Files
- `index.html` — all website content and page structure
- `styles.css` — layout, typography, colours and responsive design
- `script.js` — mobile navigation and current year
- `assets/favicon.svg` — browser tab icon

## Before publishing: make these edits
1. Open `index.html`.
2. Find `YOUR_EMAIL@example.com` in the contact form action and replace it with the email address that should receive enquiries.
3. Find the contact detail text `Update with your business email` and replace it with the same business email.
4. Review the wording and ensure every statement accurately reflects Evolve Africa Minerals' current status.
5. The site uses externally hosted Unsplash images and Google Fonts. An internet connection is needed for those assets to load.

## Preview locally
The simplest method is to open `index.html` in Chrome. For a more reliable preview, use a local static server, but no build step is required.

## Publish using GitHub Pages
1. Sign in to GitHub and create a new **public** repository, for example `evolve-africa-minerals`.
2. Keep the repository name simple. Do not add a README, .gitignore or licence if you are uploading these prepared files as a complete set.
3. On the repository page, choose **Add file → Upload files**.
4. Open the unzipped website folder on your computer. Upload `index.html`, `styles.css`, `script.js`, and the `assets` folder. Upload the contents so `index.html` sits in the repository's root, not inside an extra nested folder.
5. Enter a commit message such as `Launch Evolve Africa Minerals website` and click **Commit changes**.
6. In the repository, open **Settings → Pages**.
7. Under **Build and deployment**, choose **Deploy from a branch**.
8. Select branch `main` and folder `/ (root)`, then click **Save**.
9. Wait for GitHub Pages to publish. The website address will appear in the Pages panel, usually in the form `https://YOUR-USERNAME.github.io/evolve-africa-minerals/`.
10. Open that address and test the desktop and mobile layouts.

## Connect a custom domain through Cloudflare
You need to own/register the domain first. Do not add a domain you have not purchased or do not control.

1. In GitHub, open **Settings → Pages → Custom domain**.
2. Enter your chosen domain, for example `www.example.com`, and save.
3. In Cloudflare, add the domain to your account if it is not already there, and make sure its nameservers are correctly delegated to Cloudflare at the domain registrar.
4. In Cloudflare DNS, create a `CNAME` record:
   - Type: `CNAME`
   - Name: `www`
   - Target: `YOUR-USERNAME.github.io`
   - Proxy status: **DNS only** while first configuring GitHub Pages.
5. If you also want the root domain (`example.com`) to work, add the four GitHub Pages A records for `@`:
   - `185.199.108.153`
   - `185.199.109.153`
   - `185.199.110.153`
   - `185.199.111.153`
   Keep these records DNS only during initial setup.
6. In GitHub Pages, enable **Enforce HTTPS** once GitHub has issued the certificate. DNS and certificate provisioning can take time.
7. After HTTPS works, you can consider enabling Cloudflare proxying, but if you encounter redirect or certificate problems, return the relevant DNS records to DNS only and troubleshoot first.

## Important domain notes
- Replace `YOUR-USERNAME` with your actual GitHub username.
- Use the exact domain you own in GitHub Pages. Choose either `www` or the apex/root domain as the primary address and configure the other to redirect or resolve consistently.
- Do not create conflicting A, AAAA or CNAME records for the same hostname.
- GitHub's current Pages documentation should be checked before changing DNS, as its recommended records and interface may change.

## Contact form setup (FormSubmit)
1. The form is already configured to send enquiries to `evolveafricaminerals@gmail.com`.
2. Publish the site and submit a test enquiry using an email address you can access.
3. FormSubmit will send an activation email to the receiving address. Open it and confirm/activate the form.
4. Submit another test to confirm delivery.
5. The first submission may be used for activation. Do not assume the form is live until you have completed the activation and a successful test.
6. Consider adding a dedicated business email rather than a personal inbox.

## Images and brand assets
The image links currently point to Unsplash-hosted photographs. For a production website, confirm the chosen images are suitable for commercial use and replace them with licensed company imagery or photographs you have permission to use. The geometric mark is a simple editable SVG-style brand treatment, not a registered trademark.

## Content and compliance
This website describes Evolve Africa Minerals' intended business scope and development direction. It does not claim that the company currently owns or operates a mine, wash plant or processing facility. Keep this distinction accurate as the business develops.
