# Jaio Radio deployment checklist

**Current site version: v1.0.2**

## Configured

| Item | Status |
|------|--------|
| Contact form (Formspree) — `https://formspree.io/f/xykvgrzd` | Done |
| Contact confirmation page — `contact-confirmation.html` | Done |
| Signup confirmation page — `signup-confirmation.html` | Done |
| Mailchimp signup — Inner Circle list | Done |
| Spotify tracks 1–5 | Done |
| Social / platform links | Done |

## You must do in external dashboards

### Formspree — change notification email

Messages are sent through Formspree. The recipient is **not** set in HTML.

1. Log in at [formspree.io](https://formspree.io)
2. Open form **xykvgrzd**
3. Set notification email to: **jaiomusicproductions@gmail.com**
4. Remove or update **nicolaegiurgiu1@gmail.com** if it is still listed
5. Submit a test message on the live site and confirm delivery

### Mailchimp — optional double opt-in redirect

The site redirects to `signup-confirmation.html` after signup. For Mailchimp’s own “confirm your email” step, you can also set:

**Audience → Signup forms → Form settings → Redirect URL**  
`https://jaioradio.com/signup-confirmation.html`

### Still optional

| Item | Notes |
|------|--------|
| Zeal footer link | `https://www.instagram.com/zealthreads_/` |
| Open Graph image | Replace `og:image` with 1200×630 promo art |
| Dedicated favicon | Optional `favicon.png` |

## Deploy v1.0.2

Push these files to GitHub so Cloudflare redeploys:

- `index.html`
- `contact-confirmation.html`
- `signup-confirmation.html`
- `privacy.html`
- `Main.html`
- All image assets (unchanged)

Test after deploy:

- `https://jaioradio.com`
- Contact form → `contact-confirmation.html`
- Drop list signup → `signup-confirmation.html`
- Footer shows **v1.0.2**
