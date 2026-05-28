# Agent Marketing Desk — Newsletter

Public hosting for the AMD weekly newsletter — published at [newsletter.brokermarketingdesk.com](https://newsletter.brokermarketingdesk.com) and used as the image CDN for the email version sent via Brevo.

The newsletter source (brand guide, templates, content, generator) is kept private. This repo only contains the rendered output and the supporting image assets.

If you found this repo through a newsletter URL: hi 👋. The newsletter goes out weekly — you can subscribe at [agentmarketingdesk.com](https://agentmarketingdesk.com).

## Structure

```
index.html                      ← Landing page (newsletter.brokermarketingdesk.com)
vercel.json                     ← Hosting config (clean URLs, date rewrites, cache)
issues/
└── YYYY-MM-DD.html             ← Rendered newsletter for each issue
2026/
└── MM-month/
    └── YYYY-MM-DD/
        └── assets/images/      ← Per-issue images (the email's CDN)
assets/
├── brand/                      ← AMD logo variants (referenced every issue)
└── team/                       ← Team headshots (referenced every issue)
```

## URLs

- `/` — landing page
- `/YYYY-MM-DD` — that week's issue (rewritten internally to `/issues/YYYY-MM-DD.html`)

Each rendered HTML loads its images from `raw.githubusercontent.com/.../2026/MM-month/YYYY-MM-DD/assets/images/*` so the email version works regardless of whether the Vercel site is up.

## License

Brand and image assets © Agent Marketing Desk. Public hosting only — please don't reuse without permission.
