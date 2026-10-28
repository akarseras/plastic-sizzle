# Editing the Plastic Sizzle archive

## Recommended workflow

1. Keep one master spreadsheet workbook with tabs named Players, Matches, Timeline, Photos, and Memories.
2. Export each tab separately as **CSV UTF-8**, using the exact filenames in `/data`.
3. Keep the existing header row and column names unchanged. Replace fictional demonstration records with verified club information.
4. Upload changed CSV files to the GitHub repository under `data/`, preserving names. GitHub Pages will deploy the changes.
5. Keep independent backups of the workbook and original photographs. GitHub is not your only archive.

## Files and columns

- `players.csv`: name, position, seasons, appearances, goals, notes
- `matches.csv`: date, season, opponent, venue, goals_for, goals_against, competition, notes (reserved for a future match results page)
- `timeline.csv`: year, title, description
- `photos.csv`: year, title, filename, alt, caption, credit
- `memories.csv`: year, title, story, contributor

## Adding photographs

1. Save a resized JPEG, PNG or WebP image to `assets/photos/` (e.g. `team-2002.jpg`).
2. Add a row to `data/photos.csv` with `filename` set to `team-2002.jpg` (without the folder path).
3. Provide a meaningful `alt` description, caption, year and credit.
4. Obtain permission to publish photographs where necessary, especially images of minors.
5. If a filename is blank, the gallery displays a placeholder. Use simple filenames without spaces where possible.

## CSV tips

- For a comma inside a cell, spreadsheet export should quote the value automatically.
- If a cell contains double quotes, CSV escaping doubles them.
- Keep records as plain text; do not put formulas in exported CSVs.
- The website safely displays record values as text rather than executable HTML.
- All data is publicly readable; don't publish private phone numbers, addresses, or sensitive information.

## Branding

- Edit `assets/style.css` variables at the top to adjust colours.
- Replace the decorative SVG thistle inside `index.html` with your official club badge once you have an image and permission to use it.
- The heading and tagline in `index.html` can be changed without editing JavaScript.

## First-release caveat

The match CSV is not yet displayed on the site.


## Photo gallery: people pictured

Edit `data/photos.csv` in Excel or Google Sheets. The `names` column contains the names shown under each photo and in the full-size viewer. Separate names with semicolons (for example: `Back row: Alex; Sam; Jordan. Front row: Pat; Chris`). For commas inside a cell, export as standard CSV with the cell quoted. Leave the field empty until identities are confirmed.

The `filename` column refers to a file inside `assets/photos/`. Photograph dates are provisional until verified.

Photo filenames use lowercase letters, numbers and hyphens, with lowercase extensions (.jpg, .png or .webp). Use descriptive names for venues and pubs (e.g. oz-dome.png or pattys-pub.jpg) and team-YYYY-MM or team-YYYY-MM-DD for dated team photos. Preserve the original image format; use .jpg for JPEG files.
