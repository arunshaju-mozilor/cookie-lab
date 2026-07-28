# CookieYes Test Site

A minimal static site for CookieYes banner QA testing, on a dark violet theme.

## Pages

| Page | Purpose |
|---|---|
| `index.html` | **Cookie Lab** home page — loads real third-party trackers and sets cookies in every category on load, with a live consent-status dashboard |
| `about.html` | About page for multi-page navigation tests |
| `privacy-policy.html` | Privacy policy (linked from banner) |

## Adding the CookieYes script

In each HTML file, uncomment and replace the script tag in `<head>`:

```html
<script id="cookieyes" type="text/javascript"
  src="https://cdn-cookieyes.com/client_data/YOUR_CLIENT_ID/script.js">
</script>
```

Get `YOUR_CLIENT_ID` from: CookieYes Dashboard → Settings → Installation.

## Hosting on GitHub Pages

1. Push this folder to a GitHub repository
2. Go to **Settings → Pages**
3. Set source to **Deploy from a branch → main → / (root)**
4. Your site will be live at `https://<username>.github.io/<repo-name>`

Use the live URL as the domain when adding a website in the CookieYes dashboard.
