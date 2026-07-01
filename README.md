# dmac-assets

Media assets for the [DMAC website](https://github.com/aztaryx/digital-multimedia-arts-club) —
kept in a separate repo so the main site repo stays light.

Served via **GitHub Pages** at:

```
https://aztaryx.github.io/dmac-assets/
```

## ⚠️ Setup required

For that URL to actually serve files, enable Pages on this repo:
`Settings → Pages → Source → Deploy from branch → main / (root)`.
It can take a minute or two after enabling (or after each push) for changes to
go live.

## Structure

```
dmac-assets/
├── logo.png
├── images/
│   ├── hero/        D / M / A panel photos      (index.html)
│   ├── misc/        group photos, org logos      (about/index.html)
│   ├── members/      member photos — currently empty, reserved
│   └── projects/     project thumbnails — currently empty, reserved
├── avatars/          member avatar images         (js/pages/members.js)
├── icons/             social platform icons        (js/pages/members.js)
├── lib/               self-hosted JS libraries (e.g. pixi.min.js)
└── audio/             sound effects and audio tracks
```

## Adding a new asset

1. Drop the file in the right folder above (create new subfolders as needed).
2. Commit & push.
3. Reference it from the main site as:
   `https://aztaryx.github.io/dmac-assets/<path-to-file>`

## What's NOT here

Badge icons (`assets/badges/` in the main repo) stay in the main site repo —
they're SVGs that get edited directly as part of that codebase, not just
dropped in as static files.
