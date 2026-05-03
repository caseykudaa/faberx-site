# faberx-site

One-page holding site for [faberx.co](https://faberx.co).

**Stack:** Single HTML file, inline CSS, no build step, no JS framework, no analytics.

**Hosting:** Vercel (free tier), DNS via Namecheap.

## Updating content

Edit `index.html` directly. Push to `main` — Vercel auto-deploys.

## Swapping placeholder values

- **Calendly URL:** Replace `https://calendly.com/casey-faberx` (appears 3× in index.html) with the real URL from `Faberx > 02 Admin > Calendly URL.txt` in Drive.
- **Colours:** Swap `--bg: #F5F1EB` and `--fg: #1A1A1A` in the `:root` block once `Faberx > 01 Brand > Site Visual Spec.md` is published.

## DNS (Namecheap → Vercel)

| Type  | Host | Value                  | TTL  |
|-------|------|------------------------|------|
| A     | @    | 76.76.21.21            | Auto |
| CNAME | www  | cname.vercel-dns.com   | Auto |

Remove any existing A records for @ before adding the Vercel one.
