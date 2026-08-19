# FILE3X — personal site

Single page, English only, no external libraries or build step.
Everything lives in `index.html`.

```
index.html          the whole site (HTML + CSS + JS)
assets/file3x.png   logo
assets/favicon.png  tab icon
```

## Change before publishing

Search `index.html` for these placeholders (contact section, near the bottom):

| Placeholder | Replace with |
|---|---|
| `https://discord.com/users/YOUR_ID` | your Discord profile link |
| `file3x` | your real Discord handle |
| `https://github.com/YOUR_USERNAME` | your GitHub |
| `you@example.com` | your email (2 places: href + shown text) |

## Colors

Top of the `<style>` block, under `:root`. The palette runs from deep red
(`--red-900` … `--red-700`) to bright red (`--red`, `--red-300`, `--red-200`).
`--grad` is the gradient used on buttons, the headline accent, and progress bars.

## Publishing on GitHub Pages

1. New **public** repo, upload the three files with `index.html` at the root.
2. Settings → Pages → Source: `Deploy from a branch`, branch `main`, folder `/ (root)`, Save.
3. Live in a minute or two at `https://your-username.github.io/repo-name/`.

Custom domain: add A records `185.199.108.153`, `185.199.109.153`,
`185.199.110.153`, `185.199.111.153` on `@`, a CNAME on `www` pointing to
`your-username.github.io`, then set the domain under Settings → Pages and
enable **Enforce HTTPS**.
