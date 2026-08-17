# Noah's Bark Pet Care — Website

A lightweight static website for **noahsbark.au**.

## What's included
- `index.html` — the page
- `styles.css` — all styling
- `script.js` — mobile menu + subtle scroll animation
- `assets/ark.png` — cropped from the Noah's Bark branding artwork
- `assets/walker-strip.jpg` — cropped from the business-card artwork
- `assets/social-preview.jpg` — preview image for social sharing
- `.nojekyll` — tells GitHub Pages to serve the files directly

There are **no paid libraries, themes, plugins, web fonts or hosting dependencies**.

## Before publishing
The current contact details are:
- Phone: 0432 897 738
- Instagram: @noahsbark.au
- Service area: Sydney's Eastern Suburbs

No prices are hard-coded, so you can settle pricing later.

## Publish on GitHub Pages
1. Create a GitHub account if you don't already have one.
2. Create a new **public** repository. A simple name such as `noahsbark` is fine.
3. Upload everything in this folder to the repository root. Make sure `index.html` is at the top level, not inside another folder.
4. Open the repository's **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select the `main` branch and `/(root)`, then Save.
7. Wait a few minutes for the temporary `github.io` site to appear.

## Connect noahsbark.au
Do this in this order:

### 1. In GitHub
Go to **Settings → Pages → Custom domain** and enter:

`noahsbark.au`

Save it.

### 2. In Porkbun
Open **Domain Management → noahsbark.au → DNS**.

The easiest current Porkbun method is **Quick DNS Config → GitHub**.

Porkbun will ask for the GitHub Pages target for the `www` CNAME. It should be:

`YOUR-GITHUB-USERNAME.github.io`

GitHub's current apex-domain A records are:

- `185.199.108.153`
- `185.199.109.153`
- `185.199.110.153`
- `185.199.111.153`

Porkbun's GitHub Quick DNS Config can create the needed GitHub Pages records for you.

### 3. Back in GitHub
Once DNS has propagated, return to **Settings → Pages** and enable **Enforce HTTPS** when the option becomes available.

DNS changes can take some time to propagate.

## Editing the site later
For simple wording changes, edit `index.html` directly in GitHub and click **Commit changes**. GitHub Pages will republish automatically.

For styling changes, edit `styles.css`.

## Adding your own dog photography later
Create an `assets/photos/` folder, upload resized JPGs/WebPs, and add a gallery section to `index.html`. Keeping images around 1600–2200 px on the long edge is plenty for a normal web gallery.
