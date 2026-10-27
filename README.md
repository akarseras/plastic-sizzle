# Plastic Sizzle — club history website

A complete, responsive, static GitHub Pages starter website for Plastic Sizzle (founded 1998). Colours: dark red, black, white, with a heritage-inspired gold accent.

**IMPORTANT:** All player records, match results, league standings, honours, sample memories and non-founding timeline events are **fictional demonstration data**. The club name, colours and founding year were supplied by the requester. The thistle graphic is a simple temporary emblem, not an official club crest.

## Publish for free using GitHub Pages

1. Sign in at https://github.com and click **New repository**.
2. Name the repository `plastic-sizzle` (or any name you like), choose **Public**, then **Create repository**.
3. Upload the *contents* of this folder to the repository root: `index.html`, `assets/`, `data/`, `docs/`, and this README. GitHub's **Add file → Upload files** supports uploading the files; for entire folder trees, extracting the ZIP and using GitHub Desktop or Git is often easiest.
4. Open **Settings → Pages** in your repository.
5. Under **Build and deployment**, select **Deploy from a branch**, choose `main`, folder `/(root)`, then **Save**.
6. Once published, the site will normally be at `https://YOUR-USERNAME.github.io/plastic-sizzle/`. Deployment can take a few minutes.
7. Test the pages, photo placeholders, and search. **Replace all fictional sample data before promoting the website.**

For a repository named `YOUR-USERNAME.github.io`, the URL is `https://YOUR-USERNAME.github.io/` instead.

## Preview locally

You cannot reliably preview by double-clicking `index.html` because browsers block `fetch()` of local CSV files under `file://`.

From this folder, run:

```sh
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Edit records

See [docs/EDITING.md](docs/EDITING.md). Edit the CSV files in `data/` using Excel, Google Sheets, LibreOffice Calc, or a text editor. Export **CSV UTF-8** with the same column headers and filenames. Commit/upload the updated CSV files to GitHub; the site updates automatically after deployment.

## Limitations / future enhancements

- Match records are included in `data/matches.csv` as a foundation for a future match-results view; the first release does not yet display individual match results.
- Photo gallery images are stored in `assets/photos/`; there are no bundled real team photos.
- The site is entirely static and has no login, private database, or in-browser editing. Public GitHub Pages content is publicly accessible.
- GitHub Pages has usage limits and is intended for static sites. Avoid storing huge original image archives in the repository; resize/compress photos before upload.
- This starter uses no third-party scripts, analytics, fonts, or paid services.

## Official club badge
The header displays `assets/plastic-sizzle-badge.png`, supplied by the club. To replace it, overwrite that file with another PNG of the same name.


## Version 3: official photo archive and homepage

The homepage prominently features the official club badge and the 14 December 2003 team photo. Both user-supplied photos are in `assets/photos/` and listed in `data/photos.csv`. The homepage timeline draws from `data/timeline.csv`. The year 1998 is the confirmed founding year supplied by the club; 2003 and 2018 dates derive from photo filenames. Please verify dates, venues and names before adding captions. Other demonstration records remain explicitly fictional.
