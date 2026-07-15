# Holy Bible — KJV (Offline PWA) — v1.1

A complete, framework-free King James Version Bible reader built for older iPhones, including the iPhone 5S.

## Included

- All 66 books and 31,102 verses
- Offline reading after the first successful load
- Book and chapter picker
- Full-Bible word search and direct reference lookup
- Bookmarks, highlights and private verse notes
- Light, sepia and dark reading themes
- Adjustable font size
- Swipe left/right between chapters
- Home-screen icon and standalone iPhone display

## Test on your computer

Do not double-click `index.html`; browser security prevents the Bible data from loading from a `file://` address.

From this folder, run:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Put it on the iPhone 5S

For offline installation on iPhone, host this folder on an HTTPS static host such as GitHub Pages, Cloudflare Pages, Netlify or your own HTTPS server. In Safari:

1. Open the hosted app.
2. Wait until the first chapter appears.
3. Tap Share.
4. Tap **Add to Home Screen**.
5. Launch it once from the new icon while connected.
6. It will then continue working offline.

## Data and privacy

The King James Version text is public domain. All bookmarks, notes, highlights and reading position are stored only in the browser on the device. No account, analytics or external API is used.


## v1.1 — iOS 12.5.x layout repair

This build fixes the iPhone 5S standalone layout so that:

- the header and bottom navigation remain fixed;
- only the current page/chapter scrolls;
- the passage picker and `Aa` panel receive taps reliably on iOS 12;
- the bottom bar sits against the bottom edge;
- the service worker replaces the older cached shell.

When replacing v1.0 on GitHub Pages, upload the contents of this folder over the existing repository files. Then open the site in Safari and refresh once. If the Home Screen copy still shows v1.0, remove that icon and add the site to the Home Screen again.
