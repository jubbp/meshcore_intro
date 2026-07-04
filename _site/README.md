# MeshCore Intro (Bunbury)

Public-facing introduction site for MeshCore and the local Bunbury MeshCore network.

## What this repo now includes

- Jekyll setup using the `jekyll-theme-cayman` theme.
- Beginner-friendly content pages:
	- Home
	- What is MeshCore
	- Bunbury Network
	- Get Connected
	- Contact Us
- Static contact form wired for Formspree (email delivery via Formspree endpoint).

## Quick start (GitHub Pages)

1. Push this repository to your hosting platform.
2. Enable static site publishing from the repository root.
3. Confirm the site builds successfully.

## Custom domain (CNAME)

1. Replace the placeholder value in `CNAME` with your real domain.
2. In your DNS provider:
	 - Set `meshcore` as a `CNAME` to your site host target.
	 - Set root/apex records as required by your host documentation.
3. In your hosting settings, set the same custom domain and enable HTTPS after certificate provisioning.

## Contact form setup (Formspree)

The Contact page uses Formspree for handling email submissions from a static site.

1. Create a Formspree form and copy its endpoint URL.
2. Open `contact.md`.
3. Replace:

```text
https://formspree.io/f/xnjkgkor
```

with your real Formspree endpoint.

## Local preview (optional)

If you want to run locally:

```bash
bundle install
bundle exec jekyll serve
```

Then open: `http://127.0.0.1:4000`
