# Refrakt — app homepage

Static app homepage, privacy policy, support page, and AdMob app-ads.txt, following the Paper Boat site structure. Each page is self-contained: styles and the small icons are inlined, so there are no build tools, dependencies, tracking scripts, or external fonts.

## Preview

Run `python3 -m http.server 8080` in this folder, then open http://localhost:8080.

## GitHub Pages

Publish this repository using GitHub Pages (Settings → Pages → Deploy from a branch → main → / root). The site is served at https://weidinger-c.github.io/refrakt-app/.

- Marketing URL: site root
- Support URL: support.html
- Privacy URL: privacy.html

## Advertising verification

app-ads.txt uses the AdMob publisher ID `pub-6235626639390894`. AdMob looks for this file at the root of the developer website domain, so the copy in this project path alone may not satisfy that lookup: also serve the same file at https://weidinger-c.github.io/app-ads.txt (via the `weidinger-c.github.io` user-site repository), or use a custom domain with the file at its root. Set the developer website as the Marketing URL in App Store Connect and verify the crawl status in AdMob.

## Content

The privacy and support text reflects the current app: 400 free levels across eight chapters, progress stored only on the device (no iCloud sync), a Google AdMob interstitial after each solved level, Google UMP consent with a Privacy choices button in the field manual where required, and the one-time Remove Ads purchase (Family Sharing). Earlier Full Spectrum buyers are treated as ad-free. Recheck these pages when app behaviour or SDK data practices change.
