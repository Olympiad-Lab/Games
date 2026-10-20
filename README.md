# Arcade Nest — browser arcade starter

A responsive static website shell for a future browser-game collection. It includes no playable games yet, as requested.

## Files
- `index.html` — page structure and metadata
- `styles.css` — responsive design and styling
- `games.js` — central game catalogue; edit this when adding games
- `script.js` — search, category filters, empty state, mobile navigation

## Preview locally
Open `index.html` in a modern browser. No build tools or dependencies are required. Google Fonts are optional; the site falls back to system fonts.

## Publish with GitHub Pages
1. Create a new GitHub repository.
2. Upload all four files (`index.html`, `styles.css`, `games.js`, `script.js`) plus this README.
3. In the repository, open **Settings → Pages**.
4. Choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
5. Wait for GitHub Pages to publish the site.

## Add a game later
Add an object to `window.GAME_CATALOGUE` in `games.js`. Use one category from `puzzle`, `arcade`, `strategy`, or `casual`.
When a real game page exists, set `status: "Available"` and set `href` to a relative path such as `games/number-puzzle/`. The starter deliberately marks every card as “Coming soon”.

## Notes
- Search matches title, category, description, and mood.
- Category filters work together with search.
- Layout adapts to mobile screens and respects reduced-motion preferences.
- No analytics, accounts, database, advertising, or third-party game embeds are included.
