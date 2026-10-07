# Andrei Repida: personal website

A single-page static site (HTML and CSS, one small script). No build step and no dependencies.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The website |
| `404.html` | Shown for pages that don't exist |
| `favicon.svg`, `apple-touch-icon.png` | Browser tab and phone home-screen icons |
| `robots.txt` | Lets search engines index the site |
| `.nojekyll` | Tells GitHub Pages to publish the files as they are |
| `.gitignore` | Keeps junk files out of the repository |

## Publish on GitHub Pages

1. On GitHub, create a new **public** repository. For the address `https://and1run.github.io`, name it exactly `and1run.github.io`. Any other name works too, and the site will then live at `https://and1run.github.io/<repo-name>/`.
2. Upload all files from this folder to the repository root (drag and drop in the browser works). Make sure the hidden files `.nojekyll` and `.gitignore` are included.
3. Open **Settings, Pages**. Under "Build and deployment" choose **Deploy from a branch**, branch `main`, folder `/ (root)`, and save.
4. Wait a minute or two, then open the address shown on that page.

## Use your own domain

1. In **Settings, Pages, Custom domain**, enter your domain and save. GitHub creates a `CNAME` file in the repository for you.
2. At your domain registrar, add the DNS records GitHub lists in its documentation for custom domains.
3. Back in Settings, Pages, tick **Enforce HTTPS** once it becomes available.

## Edit the content

Everything is in `index.html`: the text, the projects, the email and the links. If you change the inline `<style>` or `<script>` block, the security hash in the `Content-Security-Policy` meta tag at the top must be updated too, otherwise browsers will block that block. Ask Claude to do it, or remove the tag if you prefer.

## Notes

- The contact form opens the visitor's email app. It does not send anything by itself, so nothing is stored.
- Fonts (Caveat and Nunito) are loaded from Google Fonts.
