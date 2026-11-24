# evergreen-infosec

Source for [evergreen-infosec.com](https://evergreen-infosec.com), a static site served by GitHub Pages.

- `index.html`: the page content
- `styles.css`: styles
- `CNAME`: the custom domain for GitHub Pages

No build step. Edit the HTML and push to `main`.

## DNS (at the domain registrar)

| Type  | Host | Value                  |
|-------|------|------------------------|
| A     | @    | 185.199.108.153        |
| A     | @    | 185.199.109.153        |
| A     | @    | 185.199.110.153        |
| A     | @    | 185.199.111.153        |
| CNAME | www  | eregular13.github.io   |

Then go to repo **Settings → Pages**, set the source to "Deploy from a branch" with `main` and `/ (root)`, and turn on **Enforce HTTPS** once the certificate is issued.
