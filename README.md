# Chez Nours

Public source for the temporary landing page at [chez-nours.com](https://chez-nours.com).

Chez Nours is a cosy duplex in Cauterets, in the French Pyrenees. The current page is a lightweight “coming soon” experience inspired by the property's warm cream-and-brown visual identity. The full website will be developed later.

## Deployment

The site is static and deployed from the `main` branch with GitHub Pages through [the Pages workflow](.github/workflows/pages.yml). The custom domain is declared in [`CNAME`](CNAME).

Public DNS should point the apex domain to GitHub Pages and `www` to the repository's GitHub Pages hostname. GitHub Pages must have **Enforce HTTPS** enabled. If Cloudflare proxies the domain, SSL/TLS mode should be **Full (strict)** and **Always Use HTTPS** should be enabled so HTTP requests redirect to HTTPS.

No credentials, account identifiers, private contact details, or deployment secrets belong in this repository.

## Local preview

Serve the repository with any static HTTP server, for example:

```sh
python3 -m http.server 8000
```

Then open `http://localhost:8000`.
