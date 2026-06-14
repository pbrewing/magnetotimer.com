# Brewington Tech – Magnetotimer Website

Product website for the Magneto Synchronizer kit, hosted on GitHub Pages at [magnetotimer.com](https://magnetotimer.com).

## Files

| File | Purpose |
|------|---------|
| `index.html` | Home page – product features |
| `pictures.html` | Photo gallery |
| `pricing.html` | Pricing, shipping, payment methods, contact info |
| `order.html` | Online ordering via PayPal |
| `styles.css` | Site-wide styles (dark theme) |
| `CNAME` | Custom domain configuration for GitHub Pages |
| `images/` | Photos, banner, and datasheet PDF |

## Updating the Site

Edit files locally, then run:

```
cd "C:\Users\p\OneDrive\Desktop\my_files\BT\mt\web_site\new_site"
git add .
git commit -m "describe your change"
git push origin master
```

GitHub Pages will update the live site within a minute or two.

## Pricing

Prices are set in two places — update both if they change:

- `pricing.html` — pricing table
- `order.html` — display text and JavaScript variables `PRICE_REGULAR` and `PRICE_BULK`

Current prices:
- Regular (1–49): $29.00
- Bulk (50+): $25.00
- Shipping USA: $10.00 flat
- Shipping Canada: $35.00 flat

## PayPal

`order.html` contains a `SANDBOX` variable near the top of the script:

```js
var SANDBOX = false;  // true = test mode, false = live
```

- Live PayPal email: `p@brewingtontech.com`
- Currently set to **live mode**

## Domain & Hosting

| Service | Provider | Notes |
|---------|----------|-------|
| Website hosting | GitHub Pages | Free |
| DNS management | Cloudflare | Free |
| magnetotimer.com registration | SiteGround | Transfer to Cloudflare pending |
| brewingtontech.com registration | SiteGround | Transfer to Cloudflare pending |

## Email

| Address | Routes to |
|---------|-----------|
| paul@magnetotimer.com | brewington.paul@gmail.com |
| paul@brewingtontech.com | brewington.paul@gmail.com |

Email routing managed through Cloudflare Email Routing (free).

## Redirects

- `brewingtontech.com` → `magnetotimer.com` via Cloudflare Redirect Rule (301 permanent)
- `www.magnetotimer.com` → `magnetotimer.com` via Cloudflare

## To Do

- Transfer magnetotimer.com domain registration from SiteGround to Cloudflare
- Transfer brewingtontech.com domain registration from SiteGround to Cloudflare
- Cancel SiteGround hosting once transfers complete
- Set up Gmail Send As for paul@magnetotimer.com
