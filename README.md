# evergreen-infosec

Source for [evergreen-infosec.com](https://evergreen-infosec.com), a static site served by GitHub Pages.

| File | Page |
|------|------|
| `index.html` | Home |
| `assessments.html` | Security assessments |
| `grc.html` | GRC advisory and Trace GRC |
| `ai-solutions.html` | AI Solutions (forward deployment) |
| `contact.html` | Contact |
| `404.html` | Not-found page |

`styles.css` holds the styles shared by every page. The header and footer are repeated in each page, so a navigation change needs to be made in all five. `sitemap.xml` lists the pages for search engines; add any new page there too. `CNAME` sets the custom domain for GitHub Pages.

No build step. Edit the HTML and push to `main`; GitHub Pages publishes within a minute or two.

## DNS (Cloudflare)

DNS for evergreen-infosec.com is hosted on Cloudflare. The records point at GitHub Pages and are **DNS only** (grey cloud), so GitHub can issue and renew the HTTPS certificate.

| Type  | Name | Value                  |
|-------|------|------------------------|
| A     | @    | 185.199.108.153        |
| A     | @    | 185.199.109.153        |
| A     | @    | 185.199.110.153        |
| A     | @    | 185.199.111.153        |
| CNAME | www  | eregular13.github.io   |

GitHub Pages is set to deploy from `main`, `/ (root)`, with **Enforce HTTPS** on.
