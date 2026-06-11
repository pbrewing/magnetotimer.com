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
git add .
git commit -m "describe your change"
git push origin master
```

GitHub Pages will update the live site within a minute or two.

## Pricing

Prices are set in two places — update both if they change:

- `pricing.html` — pricing table
- `order.html` — display text and JavaScript variables `PRICE_REGULAR` and `PRICE_BULK`

## PayPal

`order.html` contains a `SANDBOX` variable near the top of the script:

```js
var SANDBOX = false;  // true = test mode, false = live
```

- Live PayPal email: `p@brewingtontech.com`
- Shipping: USA $10 / Canada $35 flat rate

## Domain & Hosting

- Domain registrar: SiteGround
- DNS managed at: SiteGround (Groundsite)
- Hosting: GitHub Pages (free)
- `brewingtontech.com` redirects to `magnetotimer.com` via SiteGround 301 redirect
