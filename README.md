# playbonehead.com

The holding site for Bonehead, a pixel-art card game by Beautiful Distraction. One page of plain HTML with its CSS inline, no build step and no script. Hosted on Cloudflare Pages (project `playbonehead-com`, also at playbonehead-com.pages.dev; `playbonehead.com` and `www` are its custom domains), which deploys every push to `main`.

## Release state

Pre-launch: the page says "Coming soon to iPhone & iPad" and has no App Store badge. When the app is live, swap the `.soon` badge for Apple's "Download on the App Store" badge (one per page, from watchpinball.com's assets) linking to `https://apps.apple.com/app/id<ID>`. Don't print a price or version.

## Assets

- `assets/img`: sprites exported at 1x from the game's own art code (`buildLogo`, `wordmark` in `dist/js/art/logo.js`, `Cards` in `dist/js/art/cards.js`) and scaled up in CSS with `image-rendering: pixelated`. Card files are `card-<rank>-<suit>.png`. Re-export them if the game's art changes.
- `assets/share.jpg`: the 1200×630 link preview, built from the same sprites.
- `assets/favicon.png`, `assets/apple-touch-icon.png`: the game's icon.
- `assets/beautiful-distraction.png`: the studio badge, as on the other sites.
- `assets/fonts`: Pixelify Sans and Atkinson Hyperlegible (the dev pages' fonts), under the SIL Open Font License 1.1, self-hosted so the page loads nothing from third parties.

Local preview: the `playbonehead` entry in `~/dev/.claude/launch.json` (port 8137).
