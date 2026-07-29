# Earnings Calendar

A tiny static web app: add stock tickers and see their upcoming earnings report dates on a calendar. No backend — it runs entirely in your browser and is hosted for free on GitHub Pages.

## Setup

1. Open the live site (link in the repo's "About" section once Pages is enabled).
2. Get a free API key from [Alpha Vantage](https://www.alphavantage.co/support/#api-key) (instant, no cost).
3. Paste the key into the site when prompted. It's saved only in your browser's local storage — it is **not** committed to this repo and is never sent anywhere except directly to Alpha Vantage.
4. Add tickers and their earnings dates fill in automatically.

## Notes

- Alpha Vantage's free tier is rate-limited (a handful of requests per day/minute). The site caches earnings data for 24 hours and only refetches when you click Refresh or the cache goes stale.
- Because the API key lives in browser local storage and calls go straight from your browser to Alpha Vantage, the key is visible to anyone who opens this browser's dev tools — don't use a key you care about keeping fully private. For a personal low-stakes free-tier key this is the standard tradeoff for a no-backend static site.
- Data and dates come from Alpha Vantage and can change — confirm with a company's investor relations page before relying on a date.

## Local development

Just open `index.html` in a browser, or serve the folder with any static file server.
