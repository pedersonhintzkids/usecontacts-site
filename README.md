# UseContacts Website

This public repo hosts the simple marketing website for `usecontacts.app`.

The real working app stays separate on Replit and in the private `pedersonhintzkids/usecontacts` app repo.

## App link

The website button is controlled in `index.html` by this one setting:

```js
window.USECONTACTS_CONFIG = {
  appUrl: "https://app.usecontacts.app",
  handle: "@getusecontacts"
};
```

When the Replit app has a final URL, update `appUrl`.

## GitHub Pages

This repo is built for GitHub Pages. Use either:

- Settings -> Pages -> Deploy from a branch -> `main` -> `/ (root)`, or
- Settings -> Pages -> GitHub Actions, using the included workflow.

Custom domain: `usecontacts.app`

## Namecheap DNS

Remove the current redirect or parking records for `usecontacts.app`, then add:

| Type | Host | Value |
| --- | --- | --- |
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | pedersonhintzkids.github.io |

For the Replit app, connect `app.usecontacts.app` in Replit first, then add the DNS record Replit gives you.
