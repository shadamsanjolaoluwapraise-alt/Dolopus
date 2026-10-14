# Dolopus

Single-page marketing site for **Dolopus** - CRM, lead generation and automation by Shadamoro Anjolaoluwa Praise.

Plain HTML, CSS and JavaScript. No build step, no dependencies.

## Structure

```
index.html                         the whole site (HTML + CSS + JS)
assets/
  favicon.svg                      browser tab icon
  apple-touch-icon.png             iOS home-screen icon (180x180)
  icon-512.png                     large app icon (512x512)
  images/
    logo.png                       nav logo (transparent, lime/green)
    logo-original-wordmark.png     original navy wordmark (source file)
    shadamoro.webp                 about-section photo
.nojekyll                          tells GitHub Pages to serve files as-is
```

## Run locally

Open `index.html` in a browser, or serve the folder:

```
python3 -m http.server 8000
```

## Deploy on GitHub Pages

1. Push this folder to a GitHub repository.
2. Repository **Settings > Pages**.
3. Source: **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. Your site goes live at `https://<username>.github.io/<repo>/`.

## Settings inside index.html

Search for these in the script section:

| What | Where | Note |
|---|---|---|
| Web3Forms access key | `access_key` hidden input in `#mf` and `#bf` | Restrict the key to your domain in the Web3Forms dashboard |
| WhatsApp number | `WA` and `WNUM` | International format, no `+` |
| Contact email | `EMAIL` | Used for the fallback links |
| Calendly link | `CAL` | Still a placeholder (`YOUR-USERNAME`) |
| Activity tracking | `PASTE_YOUR_APPS_SCRIPT_URL_HERE` | Tracking stays off until you add a Google Apps Script URL |

## Brand colours

| Role | Code |
|---|---|
| Primary (lime) | `#c3f53c` |
| Secondary (green) | `#22c55e` |
| Background | `#0a0c0a` |
| Cards | `#141714` |
| Text | `#f3f6f1` |
| Muted text | `#9ba79d` |
