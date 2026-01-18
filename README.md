# lifeblog

My life blog built with Hugo.

## Structure

- `lifeblog_source/` - Hugo source files (content, themes, config)
- `lifeblog_pub/` - Previously published files (kept for reference, not used for deployment)

## Automated Deployment

This repository uses GitHub Actions to automatically build and deploy the Hugo site to GitHub Pages whenever changes are pushed to the `main` branch in the `lifeblog_source/` directory.

The workflow:
1. Builds the Hugo site from `lifeblog_source/`
2. Deploys the built site to GitHub Pages
3. Preserves the custom domain (CNAME) configuration

## Local Development

To build and preview locally:

```bash
cd lifeblog_source
hugo server
```

The site will be available at `http://localhost:1313`
