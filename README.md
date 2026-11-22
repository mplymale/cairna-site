# Cairna — marketing site

Static site for **cairnagame.com**, built to the same shape as the Dive Tend and
ClearNight sites: plain HTML, no build step, GitHub Pages via `CNAME`.

| File | Purpose |
|---|---|
| `index.html` | Landing page (inline styles, like Dive Tend's) |
| `privacy.html` | Privacy Policy. **Apple requires this URL to resolve before submission** |
| `terms.html` | Terms of Use |
| `support.html` | Support page. The Support URL in App Store Connect |
| `styles.css` | Shared styles for the three document pages |
| `CNAME` | `cairnagame.com` |
| `app-ads.txt` | AdMob publisher record (same publisher as Dive Tend) |
| `img/` | Screenshots and the passage backgrounds (from the app's own art) |

## Differences from the Dive Tend site, and why

- **Dark throughout**, like the app and like ClearNight's site. The legal pages are
  dark too, so following a footer link never flips the page from dark to white.
- **Cairna's own brand:** Outfit (the app's typeface), forest tones from the
  passage backgrounds, Mike's white wordmark, one warm accent (#ffb37a).
- **No pricing plans:** Cairna has no subscription. The pricing section lists the
  one-time purchases and what the game never does.

## Before this goes live

- [ ] Replace `[EFFECTIVE DATE]` in `privacy.html` and `terms.html` with the
      publication date.
- [ ] Set the analytics retention in Privacy → *How long we keep it* (`[RETENTION]`),
      to match the PostHog project setting.
- [ ] **Make the policy match the shipped app.** It describes the launch plan:
      PostHog analytics, RevenueCat, iCloud progress sync and Game Center. Those
      are not in the app yet. Remove any that don't ship, or add them before launch.
- [ ] Swap the two "Coming soon" buttons for the App Store link once the listing
      exists (search for `APP STORE` in `index.html`).
- [ ] Replace the prototype screenshots in `img/` with real App Store screenshots.
- [ ] Replace `favicon.png`, `apple-touch-icon.png` and `og-image.jpg` once the app
      icon is final (they use a pebble cairn for now).
- [ ] Verify `app-ads.txt` against the AdMob account Cairna's app is created in.
- [ ] Confirm the prices against App Store Connect (they come from the
      monetization spec and are placeholders until the products exist).
- [ ] Have the privacy policy reviewed by someone who handles app privacy.

## Not written

A cookie notice. The site sets no cookies and loads no analytics, only Google Fonts.
