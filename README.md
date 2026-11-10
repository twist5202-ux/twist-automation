# TWIST Automation Studio

Static website and n8n workflow collection for automation use cases including small businesses, customer support, crypto monitoring, content, education, events, and more.

## Website

- Main project site: https://twist5202-ux.github.io/automation/
- This repository contains website pages and workflow JSON files. The public URL above is served from a GitHub Pages repository, so changes here may need to be synchronized separately to appear there.

## Repository layout

```text
twist-automation/
├── index.html             # Root landing page
├── automation/
│   ├── index.html         # Automation storefront / catalog
│   ├── umkm/              # Small-business workflow files and page
│   ├── crypto/            # Crypto monitoring workflow files and page
│   ├── cs/                # Customer support workflow files and page
│   └── ...                # Other industry/category folders
├── cs/                    # Customer support demonstration page
├── demo/                  # Interactive demo
├── fashion/               # Fashion-related web pages
├── harga/                 # Pricing page
├── n8n/                   # Additional n8n materials and documentation
├── n8n-crypto/            # Additional crypto workflow collection
├── build.py               # Existing site-generation script
├── README.md              # English documentation
└── README-ID.md           # Dokumentasi bahasa Indonesia
```

## Working locally

For local preview, serve the repository with a static HTTP server:

```bash
python -m http.server 8000
```

Visit http://localhost:8000/ or http://localhost:8000/automation/.

n8n workflows are JSON exports. Import each intended file into a trusted n8n environment, then review credentials, webhook URLs, third-party service requirements, and activation settings before use. Files here are templates; they are not guaranteed to work without configuration.

## Maintenance and deployment

- **Do not rearrange or delete `automation/`, `n8n/`, or `n8n-crypto/` without checking all links.** Similar-looking directories may contain different versions or routes.
- The website contains inline styles and scripts; extracting them requires browser regression tests.
- The `twist5202-ux.github.io` repository also contains automation content. Keep the two repositories' deployed routes and source of truth clear when making updates.
- Never commit API keys, access tokens, production credentials, or personal customer data.
- Always preview changes on mobile and desktop and verify all navigation before publishing.

## Related project

Security research write-ups live in [security-writeups](https://github.com/twist5202-ux/security-writeups), not in this automation repository.
