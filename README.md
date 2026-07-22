# BARCODEMAN landing page

## Files
- `index.html`
- `styles.css`
- `assets/barcodeman-avatar.webp`
- `assets/barcodeman-header.webp`

## Publish on GitHub Pages

1. Create a new **public** GitHub repository, for example `barcodeman-site`.
2. Upload everything inside this folder, keeping the `assets` folder intact.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, select:
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/(root)**
5. Click **Save**.
6. In the **Custom domain** box, enter:
   `barcodeman.rocks`
7. GitHub will display the DNS records that need to be added at IONOS.
8. In IONOS DNS, add the records GitHub requests. For the root/apex domain, GitHub commonly uses these A records:
   - `185.199.108.153`
   - `185.199.109.153`
   - `185.199.110.153`
   - `185.199.111.153`
9. Add a `www` CNAME pointing to your GitHub Pages hostname, typically:
   `YOUR-GITHUB-USERNAME.github.io`
10. Return to GitHub Pages and enable **Enforce HTTPS** once available.

DNS changes can take anywhere from a few minutes to 24 hours.
