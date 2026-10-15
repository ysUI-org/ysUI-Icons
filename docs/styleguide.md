# ysUI Icons Style Guide

ysUI icons are symbolic: one color, outlined, drawn on a 120×120 canvas. They take SF Symbols as inspiration and use freedesktop icon names, but they are not a copy of either. This guide describes what the shipped icons actually do. When an icon disagrees with this guide, match the icons around it and fix the guide.

## Canvas

- **Size:** 120×120 units. Every icon uses `viewBox="0 0 120 120"`.
- **Small-size check:** an icon must still read at 16 and 24 pixels. Render it at those sizes before committing.
- **Live area:** most icons sit inside about 15–105 on their long side. Typical boxes in the shipped set:

| Shape | Typical box | Examples |
| --- | --- | --- |
| Wide object | x 15–105, height 60–75 | `drive-harddisk`, `video-display`, `utilities-terminal`, `network-server` |
| Circle | 17.6–102.4 (diameter 84.8) | `dialog-information`, `help-browser`, `internet-web-browser` |
| Tall object | y 20–100, width 60–80 | `folder`, `document-new`, `edit-paste`, `system-lock-screen` |
| Arrows and marks | 70–78 long, 58 across | `go-next`, `go-up`, `view-refresh`, `list-add` (59×59) |
| Status glyphs | 80–94 wide | Wi-Fi 19.2–100.8, volume 12.8–106.5 |

- **Exception for very wide objects:** the battery fills the full width (x 0.4–119.2, y 32.1–89). Battery icons keep that body so their levels line up.
- Leave at least 5 units of padding on every side, except for the battery family.

## Weight

- **Main outline:** 7 units. Measured outlines in the set range from 6.8 to 8.0. Use 7 for new work.
- **Details:** 4–6 units for inner marks: the speaker waves (5.1–5.6), the sun's rays (5.2), keyboard keys, and cloud rain (5). Do not go below 4. Anything thinner fills in or disappears at 16px.
- **Bars and arrow shafts:** 8 units with fully round ends, as in `list-add`, `list-remove`, and the `go-*` arrows.
- Thinner strokes, such as the 3-unit squares in an early `view-app-grid`, do not belong in this set.

## Shape

- **Outlined, not stroked.** Every stroke is converted to a filled shape. Files contain only filled paths.
- **Round caps and round joins** on all open strokes.
- **Corner radii scale with the shape.**
  - Large bodies use an outer radius of about 9–12, and the inner edge of the outline uses outer − 7. The battery is 12.1/5.1 and the folder is 9.7/2.
  - Small parts and inner shapes use 4–5.
  - A bar's radius is half its width.
- **Gaps:** when one shape crosses or sits on another (a slash, a badge, a lock), cut a gap of about 4 units into the shape underneath. Shapes should not merge into one blob.
- **Text:** letters and symbols inside an icon (`?`, `!`, `i`) follow Fredoka Medium.

## Color and opacity

- **Color:** `#000000`. No other colors and no gradients.
- **Inactive parts:** parts of a level icon that are "off" are drawn at 25% opacity with the class `.st1{opacity:0.25;}`. Wi-Fi signal and volume do this: `network-wireless-signal-weak` draws all three arcs with the top two dimmed, and `audio-volume-low` dims the outer waves. A level icon always draws the full shape, so it keeps its size as the level changes.
- No other partial opacity.

## Variants and naming

Names follow the [freedesktop Icon Naming Specification](https://specifications.freedesktop.org/icon-naming-spec/latest/), plus the de facto names GTK, libadwaita, NetworkManager, and UPower request (for example `battery-level-40-charging`, `view-reveal`, `pan-down`). Files are stored without the `-symbolic` suffix.

- **Folders** follow the freedesktop contexts: `actions`, `apps`, `categories`, `devices`, `emblems`, `emotes`, `mimetypes`, `places`, `status`.
- **Filled:** `name.filled.svg` is a solid version of `name.svg` (for example `folder.filled.svg`). It is redrawn, not just the outline filled in. Inner marks become cut-outs, and outlines that would merge are reshaped. `battery.filled` is a solid body with no gap around the level bar.
- **Alternative:** `name_alt.svg` is a second design for the same meaning (for example `go-next_alt.svg`, a chevron instead of an arrow).
- **States and actions:** append them with a dash: `address-book-new`, `printer-error`, `network-wireless-signal-weak`.
- **Same artwork, two names:** when two names mean the same thing (`system-search` and `edit-find`), both files exist with identical artwork. Do not use symlinks.

## Families

New icons start from the family they belong to and reuse its geometry.

- **Battery:** body and tip from `devices/battery.svg`. The level is a bar inside the body with a 4-unit gap. Charging puts a bolt over the bar with a 4-unit gap around it. Levels 0–10 use the caution treatment.
- **Wi-Fi:** the wedge and two arcs from `network-wireless-signal-good.svg`. ysUI has three segments, so `signal-excellent` and `signal-good` look the same.
- **Volume:** the speaker from `audio-volume-*`, with up to three waves.
- **Slashed (disabled, muted, off):** a 7-unit diagonal from top left to bottom right, with a 4-unit gap cut into the shape underneath. See `network-wireless-disabled` and `audio-volume-muted`.
- **Badges:** small status marks (`!`, `+`, a lock, a clock) sit at the bottom right, with a 4-unit gap around them.

## File layout

```xml
<?xml version="1.0" encoding="utf-8"?>
<svg version="1.1" id="icon-name" xmlns="http://www.w3.org/2000/svg" x="0px" y="0px"
	 viewBox="0 0 120 120" style="enable-background:new 0 0 120 120;" xml:space="preserve">
<style type="text/css">
	.st0{fill:none;}
	.st1{opacity:0.25;}
</style>
<rect id="BG" class="st0" width="120" height="120"/>
<g>
	<path d="..."/>
	<path class="st1" d="..."/>
</g>
</svg>
```

- `id` is the icon name.
- The transparent `BG` rect keeps the canvas size in editors.
- Coordinates use one decimal place.
- Only include `.st1` when the icon has dimmed parts.

**Packaging note:** GTK recolors symbolic icons by forcing a fill on `rect`, `circle`, and `path`, which can turn the `BG` rect solid. Remove the `BG` rect, and add the `-symbolic` suffix, when building an installable theme from these sources.

## Usage

- Icons are SVG and scale to any size.
- They must work on light and dark backgrounds. Check both.

Updated: October 14, 2026
