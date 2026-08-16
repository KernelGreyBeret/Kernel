# KernelGreyBeret.com

Deploy-ready static personal site for **Tommy Burke / KernelGreyBeret**.

## What is included

- `index.html` — full single-page personal site
- `404.html` — custom GitHub Pages 404 page
- `assets/styles.css` — all styling
- `assets/script.js` — mobile navigation + dynamic copyright year
- `assets/favicon.svg` — simple KGB favicon
- `CNAME` — custom domain configuration for `kernelgreyberet.com`
- `.nojekyll` — tells GitHub Pages to serve the repository as plain static files

## Fastest deployment to GitHub Pages

1. Create a new GitHub repository. A repo named `kernelgreyberet.com` is clean and easy, but the repository name can be anything.
2. Upload every file and folder in this package to the repository root.
3. In GitHub, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select your default branch (usually `main`) and `/ (root)`.
6. Save.
7. In your DNS provider, point `kernelgreyberet.com` at GitHub Pages using the DNS records GitHub currently documents for apex domains, or use the configuration you already use for your other GitHub Pages sites.
8. In GitHub Pages settings, confirm the custom domain is `kernelgreyberet.com` and enable **Enforce HTTPS** once the certificate is ready.

## Before launch: check these links

Search `index.html` for these values and replace them if needed:

- `hello@kernelgreyberet.com`
- `https://www.linkedin.com/in/tommy-burke`
- `https://asymmetricprecision.com`
- `https://kgbarcade.com`

The Amazon button is already wired to the current Amazon listing for the book.

## Add a real headshot

The hero currently contains a deliberately styled initials placeholder.

To use a real photo:

1. Add the image as `assets/tommy-burke.jpg`.
2. In `index.html`, replace the entire `div` with class `avatar-placeholder` with:

```html
<div class="avatar-placeholder">
  <img src="assets/tommy-burke.jpg" alt="Tommy Burke" style="width:100%;height:100%;object-fit:cover;" />
</div>
```

## Editing philosophy

This package has no framework, package manager, build process, external font dependency, or JavaScript library. Edit the files, commit, and GitHub Pages serves the result.
