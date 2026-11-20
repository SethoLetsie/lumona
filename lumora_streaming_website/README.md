# LUMORA — Streaming Discovery Website

A responsive front-end streaming discovery platform created for the Limkokwing University BIWD1110/DIWD1110 Principles of Web Design group assignment.

## Run locally
1. Extract the ZIP file.
2. Open the folder in Visual Studio Code.
3. Start a local server (recommended: VS Code Live Server).
4. Open `index.html` through the local server.

The JSON catalogue is loaded with the Fetch API from `data/catalogue.json`. If fetching is blocked (for example, when opening the HTML file directly with `file://`), the app uses a built-in fallback catalogue and displays a status message.

## Why trailers show "Error 153"
YouTube blocks embedded players on pages opened by double-clicking `index.html` (`file://`). Serve the folder over http(s) (Live Server, `python -m http.server`, Netlify, GitHub Pages) and trailers play. When opened from disk, LUMORA shows a "Watch on YouTube" button instead of a broken player.

Sample trailers are Blender Foundation open movies (CC BY): Big Buck Bunny, Sintel, Tears of Steel, Elephants Dream.

## Files
- `index.html` — semantic HTML5 structure and Bootstrap components.
- `css/style.css` — custom styling, layout, hover/focus states and responsive media queries.
- `js/app.js` — dynamic rendering, search, filters, details, trailer modal, form validation and localStorage watchlist.
- `data/catalogue.json` — sample catalogue data.

## Assignment coverage
- Home, Explore, My List, About/Help and Sign In sections.
- 12 sample titles across multiple genres and content types.
- Dynamic catalogue generated from an array of JavaScript objects / fetched JSON.
- Search by title or description, genre filter and content-type filter.
- Details modal and third-party trailer embeds for sample videos.
- My List add/remove with localStorage persistence.
- Demonstration form with HTML constraints and JavaScript validation; no password, account creation or data transmission.
- Bootstrap navbar, grid, buttons, forms, modal, toast and responsive utilities.
- CSS Grid, Flexbox, hover/focus states and responsive breakpoints.
- Poster images are sourced from Unsplash; trailer samples are embedded from YouTube. Third-party availability may change.

## Before submission
- Publish the folder to GitHub Pages, Netlify or Vercel.
- Test the public URL in a private/incognito browser.
- Check that images, Bootstrap CDN, JSON fetch and video embeds load.
- Submit the public website URL and a ZIP backup.
- Prepare a short report explaining Bootstrap usage, Fetch/API fallback, design choices, testing and each group member's contribution.
