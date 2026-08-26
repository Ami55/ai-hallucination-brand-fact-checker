# AI Hallucination & Brand Fact Checker

Vercel-ready app for comparing captured AI answers with an approved, source-backed brand fact knowledge base.

## App deployment

Upload all files from the app ZIP to a new GitHub repository and import it into Vercel. The app project requires no environment variables.

## Gemini Proxy 3

Upload `brand-fact-check.js` from the proxy ZIP to the `api` folder of the existing `gemini-proxy-3` repository. Confirm that Proxy 3 has `GEMINI_API_KEY` in Vercel.

The app calls `https://gemini-proxy-3.vercel.app/api/brand-fact-check`.

The MVP stores facts and audit history in the current browser. Export JSON backups. A multi-user production version should add authentication, database storage and review permissions.
