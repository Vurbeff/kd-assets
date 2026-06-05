# kd-assets

Public web assets for the Kaleidoscope Desert sites (served free via the
[jsDelivr](https://www.jsdelivr.com/) CDN, which has no egress cost).

These are decorative, muted background video loops used on the booking /
visit pages. The clips are already public on the Kaleidoscope Desert
YouTube channel; this repo just hosts web-optimized copies so the site
can use chrome-free native `<video>` players instead of YouTube embeds.

| File | What | Notes |
|------|------|-------|
| `brand.mp4` | Sanctuary aerial montage | 1440×810, muted, ~6 MB |
| `gamelatron.mp4` | Animated Gamelatron gong loop | 1920×1080, muted, ~2 MB |
| `brand.jpg` / `gamelatron.jpg` | Poster frames | shown while the video loads |

## Usage

Reference a tagged version so URLs are immutable and cache well:

```
https://cdn.jsdelivr.net/gh/Vurbeff/kd-assets@v1/brand.mp4
https://cdn.jsdelivr.net/gh/Vurbeff/kd-assets@v1/gamelatron.mp4
```

To update a clip: replace the file, commit, then create a new tag
(`v2`, `v3`, …) and point the site at the new tag.
