# Editing the Plastic Sizzle archive

## Recommended workflow

1. Keep one master spreadsheet workbook with tabs named Seasons, Players, Matches, Honours, Timeline, Photos, and Memories.
2. Export each tab separately as **CSV UTF-8**, using the exact filenames in `/data`.
3. Keep the existing header row and column names unchanged. Replace fictional demonstration records with verified club information.
4. Upload changed CSV files to the GitHub repository under `data/`, preserving names. GitHub Pages will deploy the changes.
5. Keep independent backups of the workbook and original photographs. GitHub is not your only archive.

## Files and columns

- `seasons.csv`: season, competition, position, played, won, drawn, lost, points, notes
- `players.csv`: name, position, seasons, appearances, goals, notes
- `matches.csv`: date, season, opponent, venue, goals_for, goals_against, competition, notes (reserved for a future match results page)
- `honours.csv`: year, competition, achievement, notes
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

The match CSV is not yet displayed on the site. The Seasons page shows aggregated seasonal statistics, not individual match scores.


### Version 3 photos and timeline

Both supplied photographs are already installed in `assets/photos/`. Edit `data/photos.csv` to change their captions, dates or credits. Edit `data/timeline.csv` to add verified milestones. Keep CSV column headings unchanged and save as UTF-8 CSV. The homepage automatically displays the timeline entries and currently features the 2003 image.
