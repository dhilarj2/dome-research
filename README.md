# Dome Research

Static website for Dome Research — an investment, incubation, and research firm.

## Stack

- **Site:** plain HTML/CSS (no build step, no framework)
- **Hosting:** GitHub Pages (serves the `main` branch)
- **DNS:** Cloudflare
- **Registrar:** Squarespace (registration transfer to Cloudflare planned)
- **Email:** Google Workspace (`hello@domeresearch.xyz`)

## Files

- `index.html` — homepage
- `blog.html` — blog index
- `styles.css` — site styling
- `CNAME` — custom domain for GitHub Pages (`domeresearch.xyz`)

## Local preview

Open `index.html` in a browser, or serve the folder:

```sh
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Deploying

Pushing to `main` auto-publishes via GitHub Pages. No build step.

## DNS records (managed in Cloudflare)

| Type  | Name | Value                    | Notes                   |
|-------|------|--------------------------|-------------------------|
| A     | @    | 185.199.108.153          | GitHub Pages (DNS only) |
| A     | @    | 185.199.109.153          | GitHub Pages (DNS only) |
| A     | @    | 185.199.110.153          | GitHub Pages (DNS only) |
| A     | @    | 185.199.111.153          | GitHub Pages (DNS only) |
| CNAME | www  | dhilarj2.github.io       | GitHub Pages (DNS only) |
| MX    | @    | smtp.google.com (prio 1) | Google Workspace email  |
