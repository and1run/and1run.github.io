# Andrei Repida: personal website

A single-page static site (HTML and CSS, one small script). No build step and no dependencies.

Live at https://andreirepida.com

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The website |
| `404.html` | Shown for pages that don't exist |
| `favicon.svg`, `apple-touch-icon.png` | Browser tab and phone home-screen icons |
| `robots.txt`, `sitemap.xml` | Let search engines find and index the site |
| `social-preview.png` | Image shown when the link is shared in chats and on social media |
| `CNAME` | Tells GitHub Pages the custom domain, `andreirepida.com` |
| `.nojekyll` | Tells GitHub Pages to publish the files as they are |
| `.gitignore` | Keeps junk files out of the repository |

## Update the site on GitHub

1. Open the repository `and1run/and1run.github.io` on GitHub.
2. Click **Add file, Upload files** and drag in the files from this folder, including the hidden ones (`.nojekyll`, `.gitignore`). Replace the existing files when asked.
3. Write a short message such as "Update site" and click **Commit changes**.
4. Wait one or two minutes, then reload https://andreirepida.com (use a private window or a hard refresh if you still see the old version).

## First-time setup (already done)

1. Create a public repository named `and1run.github.io` and upload these files.
2. In **Settings, Pages**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`.
3. In **Settings, Pages, Custom domain**, enter `andreirepida.com`, add the DNS records GitHub lists at your registrar, and tick **Enforce HTTPS** once it becomes available.

## Edit the content

Everything is in `index.html`: the text, the projects, the links and the email address (inside the script at the bottom). If you change the inline `<style>` or `<script>` block, the security hash in the `Content-Security-Policy` meta tag at the top must be updated too, otherwise browsers will block that block. Ask Claude to do it, or remove the tag if you prefer.

## Notes

- The "Copy email" button copies the address to the clipboard. The address is not written in the page text, so spam programs that scan pages don't see it.
- The light and dark theme follows the visitor's device setting, and the toggle in the top bar overrides it. The choice is saved in the browser.
- Fonts (Caveat and Nunito) are loaded from Google Fonts. The chart in the intro and the spreadsheet figure in About me use sample data, as their captions say.
