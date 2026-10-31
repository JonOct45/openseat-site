# Open Seat site

Public pages for the app: privacy policy, terms, and support. Served by GitHub Pages from `main` (root). Plain HTML, no build step.

## Fill in the placeholders

Every value in `[[...]]` must be replaced before launch:

```sh
grep -o '\[\[[^]]*\]\]' *.html | sort | uniq -c
```

Replace one across all pages (macOS):

```sh
sed -i '' 's/\[\[STORE NAME\]\]/Your Store Name/g' *.html
```

## Custom domain

Add a `CNAME` file containing the domain, set the DNS records GitHub shows under Settings → Pages, then tick "Enforce HTTPS".

## Keep in sync with the app

The privacy policy describes what the app collects. When the app starts collecting something new, update `privacy.html` and the App Store privacy answers together.
