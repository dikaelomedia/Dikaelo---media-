# Dikaelo Media website

Static site (HTML, CSS, JS). No build step, no dependencies.

## Files
- `index.html` – all page content
- `styles.css` – design (black, gold and ivory palette (matches the logo), Cormorant Garamond + Manrope)
- (script is built into `index.html`) mobile menu and the 3-step quote form (sends to WhatsApp, email fallback)
- `privacy.html`, `terms.html` – placeholders; write real policies before launch
- `logo.jpg` – your logo

## Publish on GitHub Pages (free)
1. Create a GitHub repo (e.g. `dikaelo-media`) and upload all these files.
2. Repo **Settings > Pages > Build and deployment**: Source = *Deploy from a branch*, branch `main`, folder `/ (root)`.
3. Your site goes live at `https://<your-username>.github.io/dikaelo-media/`.

## Connect your .co.za domain
1. Buy the domain from a South African registrar.
2. In Settings > Pages, enter your domain under **Custom domain** (GitHub creates a `CNAME` file).
3. At the registrar's DNS settings add:
   - `A` records for `@` pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` for `www` pointing to `<your-username>.github.io`
4. Wait for DNS to update, then tick **Enforce HTTPS**.
(Check GitHub's current Pages docs in case the IPs have changed.)

## Edit
- Phone/email: search `063 445 0476` and `27634450476` / `admin@dikaelomedia.net` in `index.html` and `script.js`.
- Colours: `:root` variables at the top of `styles.css`.
