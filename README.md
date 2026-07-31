# Parcelle — parcelleuae.com

Static single-page site. Every file lives at the top level (root), including the images. Nothing is in a subfolder, so nothing can be flattened by mistake.

## Publish on GitHub Pages
1. Create a new **public** repository (e.g. `parcelle-site`). 
2. Drag **all** of these files into the upload box together: `index.html`, `CNAME`, `404.html`, `README.md`, `.nojekyll`, and every `.jpg` / `.png`. They all belong at the root.
3. Commit.
4. **Settings > Pages** -> Source: *Deploy from a branch*, Branch: *main*, Folder: */ (root)*. Save.
5. Under **Custom domain**, enter `parcelleuae.com`. Save. Tick **Enforce HTTPS** when it appears.

## DNS (at your domain provider)
Apex `parcelleuae.com` -> four **A** records, name `@`:
185.199.108.153 / 185.199.109.153 / 185.199.110.153 / 185.199.111.153
`www` -> one **CNAME** record pointing to `YOUR-GITHUB-USERNAME.github.io`

## Editing later
- Copy: open `index.html`, find the text, edit, re-upload.
- Images: replace a file keeping the same name.
- Contact: buttons are `mailto:hello@parcelleuae.com`. Swap for `https://wa.me/...` when WhatsApp is live.
