# Armageddon Chart Scanner 2.2 — deployment bundle

## Deploy to GitHub Pages
1. Extract this ZIP.
2. Upload **the contents** of this folder to the root of your GitHub Pages repository (not the containing folder itself).
3. Make sure `index.html`, `manifest.webmanifest`, `sw.js`, and the `icons/` folder are all at the repository root/relative paths shown here.
4. In GitHub, open **Settings → Pages** and select the correct branch and root folder.
5. Open the deployed URL in Chrome on Android. Test **Demo (simulated)** first, then try live data.
6. To install, open the deployed site in Chrome → menu ⋮ → Install app / Add to Home screen.

## What is included
- Preserved self-contained mobile HTML app.
- 714 Method strategy for SAST windows 07:00–08:00, 13:00–14:00 and 16:00–17:00, using M5 pullback/continuation confirmation and a fixed target distance based on a configured pip convention.
- Voice alerts and 1% default risk calculator.
- PWA manifest, icons and a basic app-shell service worker.
- Licence-key system intentionally omitted.

## Important verified limitations
- The scanner does not place trades.
- The 714 Method has logic-level tests for bullish and bearish setups and out-of-session rejection, but is not backtested for profitability.
- The public Deriv WebSocket feed is not assumed to provide WTI oil. Crude Oil WTI is configured for the MetaApi broker bridge; it requires a connected broker offering oil and the exact broker symbol. A common name such as `USOIL` or `XTIUSD` is broker-specific; do not assume one is correct without checking your MT5 symbol list.
- The risk calculator estimates lots only from values you enter; it does not fetch account balance or contract specifications automatically.
- News calendar events are not the same as verified live fundamental analysis.
- The service worker caches the app shell only. Live market prices and external data still require an internet connection.

## Tests performed on this build
- Main JavaScript module syntax check with Node.js.
- Unit-style tests for bullish 714 detection, bearish 714 detection, fixed target distance, and no signal outside configured session windows.
- Manifest JSON parse and ZIP integrity checks.
- Live broker connectivity and a full browser session could not be verified in this environment; complete those checks on your hosted GitHub Pages URL and broker account.
