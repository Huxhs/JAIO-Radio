# Jai-O Radio — deployment checklist

Use this table before going live at **jaioradio.com**.

| Item | Status |
|------|--------|
| **Contact form (Formspree)** — `https://formspree.io/f/xykvgrzd` | ☑ |
| **Spotify tracks 1–5** (music carousel) | ☑ |
| **Spotify profile** | ☑ |
| **Apple Music** | ☑ |
| **YouTube** | ☑ |
| **Instagram** | ☑ |
| **TikTok** | ☑ |
| **Email drop list (Mailchimp)** — `#dropForm` `action` | ☐ |
| **Zeal footer link** — `.footer-zeal` `href` | ☐ |
| **Open Graph image** (1200×630 promo) | ☐ |
| **Favicon** (optional) | ☐ |

## Still to configure

### Mailchimp (drop list)

1. **Audience** → **Signup forms** → **Embedded forms**.
2. Copy the form `action` URL into `#dropForm` in `index.html`.

### Deploy

Upload the folder to Netlify, Cloudflare Pages, or similar. Set **index.html** as the home page. Point **jaioradio.com** DNS to your host.
