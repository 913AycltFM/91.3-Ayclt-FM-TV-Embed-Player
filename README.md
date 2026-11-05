# 91.3 Ayclt FM TV — Embed Player

A responsive, branded web player for watching the 91.3 Ayclt FM television channels from a website. The player supports five live HLS feeds, channel switching, standard video controls, and fullscreen playback.

## Live player

<https://913aycltfm.github.io/91.3-Ayclt-FM-TV-Embed-Player/embed-player.html>

The player repository is public, and the site is published with GitHub Pages.

## TV channels

| Channel | Description |
| --- | --- |
| 01 | 91.3 Ayclt FM |
| 02 | 91.3 Ayclt FM HD2 |
| 03 | 91.3 Ayclt FM HD3 |
| 04 | Live Studio Cam |
| 05 | Mobile Studio Cam |

The channel streams are configured in `embed-player.html`.

## Player features

- Five selectable live HLS channels
- Responsive layout for desktop, tablet, and mobile
- HTML5 video controls, including fullscreen where supported
- HLS.js playback for browsers that do not support HLS natively
- Native HLS fallback for compatible browsers, including Safari
- 91.3 Ayclt FM dark theme with red accents

## Embed the player on a website

Copy this iframe into the HTML of the website where you want the player to appear:

```html
<iframe
  src="https://913aycltfm.github.io/91.3-Ayclt-FM-TV-Embed-Player/embed-player.html"
  title="91.3 Ayclt FM TV"
  width="100%"
  height="700"
  style="border:0; max-width:1100px;"
  allow="autoplay; fullscreen; picture-in-picture"
  allowfullscreen
  loading="lazy">
</iframe>
```

Adjust the iframe height to fit your website layout. The player itself is responsive; the iframe height is controlled by the website embedding it.

## GitHub Pages deployment

This repository is published using GitHub Pages.

To review or change the publishing configuration:

1. Open **Settings → Pages**.
2. Under **Build and deployment**, check that **Deploy from a branch** is selected.
3. Confirm the `main` branch and `/(root)` folder are selected.

The public player address is:

`https://913aycltfm.github.io/91.3-Ayclt-FM-TV-Embed-Player/embed-player.html`

## Use the player code directly

If you are adding the player to a page you control, you can copy the contents of `embed-player.html` into the page's HTML. Keep the HLS.js script include and the player script so channel switching works.

## Playback notes and troubleshooting

- **A black screen or playback error:** Confirm that the selected live stream is online and reachable.
- **The player loads but video does not start:** Press the video play button. Browsers commonly block autoplay with sound until a visitor interacts with the page.
- **HLS is unsupported:** Use a modern browser. The player uses HLS.js where Media Source Extensions are available and falls back to native HLS where supported.
- **Fullscreen does not work inside an embed:** Make sure the iframe includes both `allow="fullscreen"` and `allowfullscreen`.
- **The page cannot be found:** Check the repository's GitHub Pages deployment status under **Actions** or **Settings → Pages**.

Live stream availability depends on the 91.3 Ayclt FM TV streaming service and is not guaranteed by this repository.

## Repository

[View the source code](https://github.com/913AycltFM/91.3-Ayclt-FM-TV-Embed-Player)

---

© 91.3 Ayclt FM. All rights reserved.
