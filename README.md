# 91.3 Ayclt FM TV — Embed Player

A responsive, branded web player for watching the 91.3 Ayclt FM television lineup. It provides six selectable live HLS feeds, channel switching, video controls, and fullscreen playback.

## Watch live

**[Open the 91.3 Ayclt FM TV Player](https://913aycltfm.github.io/91.3-Ayclt-FM-TV-Embed-Player/embed-player.html)**

The player is hosted with GitHub Pages. Use this as the public player link.

## Channel lineup

| Channel | Name |
| --- | --- |
| 01 | 91.3 Ayclt FM |
| 02 | 91.3 Ayclt FM HD2 |
| 03 | 91.3 Ayclt FM HD3 |
| 04 | 91.3 Ayclt FM HD4 |
| 05 | 91.3 Ayclt FM Live Studio Cam |
| 06 | 91.3 Ayclt FM Mobile Studio Cam |

All six channel entries are configured in `embed-player.html`.

## Embed on a website

Add this iframe to the HTML of your website:

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

Change the iframe height to suit your page layout. The player adjusts to the available width; the website controls the iframe's height.

## Fullscreen playback

The player includes native HTML5 video controls. To allow the video to enter fullscreen when embedded on another website, the embedding iframe must include both:

- `allow="autoplay; fullscreen; picture-in-picture"`
- `allowfullscreen`

Use the complete iframe example above rather than removing these attributes. If fullscreen still does not work, check whether the website builder or the page's own embedding settings restrict fullscreen permissions. Also test the standalone [TV Player](https://913aycltfm.github.io/91.3-Ayclt-FM-TV-Embed-Player/embed-player.html) directly. If fullscreen works on the standalone page but not inside the website, the restriction is likely in the website's iframe/embed configuration.

## Player features

- Six selectable live HLS channels, including HD4
- Responsive layout for desktop, tablet, and mobile
- HTML5 video controls and fullscreen playback where supported
- HLS.js playback in browsers that support Media Source Extensions
- Native HLS playback fallback for compatible browsers, including Safari
- 91.3 Ayclt FM dark theme with red accents

## Updating channel streams

1. Open `embed-player.html`.
2. Find the channel configuration in the player code.
3. Update the HLS stream URL for the channel you want to change.
4. Commit the change to the `main` branch.
5. Allow GitHub Pages to publish the update, then reload the live player.

Keep each channel's name, button, and stream URL matched. Use the current HLS playlist URL provided by the TV streaming service.

## GitHub Pages

The site is published through GitHub Pages from this repository.

To review the publishing settings:

1. Open **Settings → Pages**.
2. Under **Build and deployment**, confirm **Deploy from a branch**.
3. Confirm the `main` branch and `/(root)` folder are selected.

If the player does not show a recent update, check the repository's **Actions** tab and **Settings → Pages** for deployment status.

## Troubleshooting

- **Black screen or playback error:** Check that the selected HLS stream is online and reachable.
- **Player loads but video does not start:** Press Play. Browsers may block autoplay with sound until the visitor interacts with the page.
- **Playback is unsupported:** Try a current version of Chrome, Firefox, or Safari.
- **Fullscreen does not work in an embed:** Confirm the iframe has both fullscreen permissions shown in the [Fullscreen playback](#fullscreen-playback) section. The website builder may also restrict iframe fullscreen.
- **Player page is missing or outdated:** Check the GitHub Pages deployment status and refresh the page after deployment completes.

Stream availability depends on the 91.3 Ayclt FM TV streaming service. This repository hosts the player and does not guarantee that a live feed is always online.

## Repository files

- `embed-player.html` — the current standalone six-channel player and GitHub Pages entry point.
- `README.md` — project documentation.

The obsolete `embed-player-2.html` file has been removed. Use `embed-player.html` for the live player and website embeds.

## Links

- [Live TV Player](https://913aycltfm.github.io/91.3-Ayclt-FM-TV-Embed-Player/embed-player.html)
- [GitHub Repository](https://github.com/913AycltFM/91.3-Ayclt-FM-TV-Embed-Player)

---

© 91.3 Ayclt FM. All rights reserved.
