# Agent Marketing Desk — Newsletter

Public hosting for the AMD weekly newsletter — published at [newsletter.brokermarketingdesk.com](https://newsletter.brokermarketingdesk.com) and used as the image CDN for the email version sent via Brevo.

The newsletter source (brand guide, templates, content, generator) is kept private. This repo only contains the rendered output and the supporting image assets.

If you found this repo through a newsletter URL: hi 👋. The newsletter goes out weekly — you can subscribe at [agentmarketingdesk.com](https://agentmarketingdesk.com).

## Structure

```
index.html                ← Landing page
2026-MM-DD.html           ← Rendered newsletter for each issue
vercel.json               ← Hosting config (clean URLs + cache headers)
assets/
├── brand/                ← AMD logo variants
└── team/                 ← Team headshots
2026/
└── MM-month/
    └── YYYY-MM-DD/
        └── assets/images/  ← Per-issue images
```

## License

Brand and image assets © Agent Marketing Desk. Public hosting only — please don't reuse without permission.
