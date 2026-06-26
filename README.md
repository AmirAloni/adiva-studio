# ADIVA Pole Studio

Landing page for [ADIVA Pole Studio](https://www.adivapole.com) — pole dance studio in Nahariya.

Hosted on [GitHub Pages](https://pages.github.com/) (`AmirAloni/adiva-studio`).

## Custom domain DNS (Cloudflare)

GitHub Pages expects:

| Type  | Name | Content               | Proxy      |
|-------|------|-----------------------|------------|
| CNAME | www  | `amiraloni.github.io` | DNS only   |
| A     | @    | `185.199.108.153`     | DNS only   |
| A     | @    | `185.199.109.153`     | DNS only   |
| A     | @    | `185.199.110.153`     | DNS only   |
| A     | @    | `185.199.111.153`     | DNS only   |

**Not** `www.amiraloni.github.io` — use `amiraloni.github.io` only.

To apply via API (optional):

```bash
CLOUDFLARE_API_TOKEN=your_token ./scripts/configure-cloudflare-dns.sh
```

After DNS propagates, re-check **Settings → Pages → Custom domain** on GitHub.
