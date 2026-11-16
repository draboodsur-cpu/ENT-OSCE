# ENT OSCE

The app is split into two HTML files so each can be uploaded separately through GitHub's mobile web interface:

- `index.html` — main trainer (Image OSCE, Clinical, Viva, and the Board books tab)
- `board-books.html` — Board books data and embedded images, loaded automatically by `index.html`
- `manifest.webmanifest`, `service-worker.js`, `icon.svg` — install/offline support

## Upload to GitHub from a phone

Create/open your repository, choose **Add file → Upload files**, and select these files from the extracted folder. Upload all files to the repository root, including both HTML files. No `images` folder is required.

The filenames and their placement are important. Keep `index.html` and `board-books.html` together in the repository root. The Board books tab loads its data from `board-books.html` and preserves the original order: Comprehensive Board Examinations, ENT TZAR OSCE stations, ENT TZAR instruments, then audiograms.

## Offline use

Open the published GitHub Pages site once while online and wait for it to finish loading. The service worker caches both HTML files for offline use. Reopen the installed app/site after the first successful online load.

## Note

The original source page itself says the material/images are for personal study and not public sharing. Check permission before publishing the repository publicly; a private repository is safer.
