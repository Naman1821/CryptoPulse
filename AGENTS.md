# AGENTS.md

## Cursor Cloud specific instructions

This is **Cryptoplace**, a single-service client-side React + Vite SPA (a crypto price tracker). There is no backend, database, or required environment variables. The app fetches data directly from the public CoinGecko API in the browser, so it needs outbound internet access to `https://api.coingecko.com`.

- Standard commands live in `package.json`: `npm run dev` (Vite dev server on `http://localhost:5173`), `npm run build`, `npm run preview`, `npm run lint`.
- `npm run lint` currently reports pre-existing errors (e.g. unused `React` imports, missing prop-types). These are existing code issues, not environment problems; don't treat a non-zero lint exit as a setup failure.
- The CoinGecko demo API key is hard-coded in `src/context/CoinContext.jsx`; no secrets/`.env` setup is needed to run the app.
