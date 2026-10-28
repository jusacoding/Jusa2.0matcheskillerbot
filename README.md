# Matches Deriv

A mobile-friendly, read-only dashboard for viewing public market ticks and digit frequencies.

## Files
- `index.html` — dashboard structure
- `style.css` — responsive neon theme
- `app.js` — WebSocket connection and statistics
- `README.md` — this guide

## Publish using GitHub Pages (no Termux required)
1. Sign in at https://github.com/
2. Create a repository named `matches-deriv`.
3. Upload all four files to the repository root.
4. Open **Settings → Pages**.
5. Under **Build and deployment**, select **Deploy from a branch**.
6. Select branch `main` and folder `/ (root)`, then save.
7. Wait for deployment and open the Pages URL shown by GitHub.

## Run locally
Open `index.html` in a browser. Some browsers restrict WebSocket behavior for local files, so GitHub Pages or another HTTPS static host is recommended.

## Privacy and safety
- This version does not ask for, collect, or store a Deriv API token.
- Do not put API tokens, passwords, or private credentials in these files or in GitHub.
- This dashboard is read-only and does not place trades.
- Past digit frequencies are descriptive statistics and do not predict or guarantee future outcomes.

## API compatibility note
The public WebSocket endpoint and request format can change. If the app shows `Connection closed` or an API error, check the current official Deriv API documentation before relying on the live feed. Verify that both tick subscriptions and historical tick requests are supported by the endpoint currently in use.
