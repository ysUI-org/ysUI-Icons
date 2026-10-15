# Icon list

The symbolic icons a modern Linux desktop asks for, in the order they are being drawn. App icons are not part of ysUI. Names are freedesktop and de facto GTK, NetworkManager, and UPower names, without the `-symbolic` suffix. Paths are under `scalable/`.

- **existing**: shipped before this list was written.
- **new**: added for this list. **(done)** means the file exists.
- **alias**: a file with the same artwork as another name.
- **redraw**: an existing icon moved to the 120×120 canvas or redrawn at ysUI weight.

## Tier 1: Folio panel, Lens, control center

### Battery

| Icon | Status |
| --- | --- |
| `status/battery-level-0` | new |
| `status/battery-level-10` | new |
| `status/battery-level-20` | new |
| `status/battery-level-30` | new |
| `status/battery-level-40` | new |
| `status/battery-level-50` | new |
| `status/battery-level-60` | new |
| `status/battery-level-70` | new |
| `status/battery-level-80` | new |
| `status/battery-level-90` | new |
| `status/battery-level-100` | alias of `devices/battery` |
| `status/battery-level-0-charging` | new |
| `status/battery-level-10-charging` | new |
| `status/battery-level-20-charging` | new |
| `status/battery-level-30-charging` | new |
| `status/battery-level-40-charging` | new |
| `status/battery-level-50-charging` | new |
| `status/battery-level-60-charging` | new |
| `status/battery-level-70-charging` | new |
| `status/battery-level-80-charging` | new |
| `status/battery-level-90-charging` | new |
| `status/battery-level-100-charging` | new |
| `status/battery-level-100-charged` | new |
| `status/battery-missing` | new |
| `status/battery-empty` | alias of `status/battery-level-0` |
| `status/battery-empty-charging` | alias of `status/battery-level-0-charging` |
| `status/battery-caution` | existing |
| `status/battery-caution-charging` | alias of `status/battery-level-10-charging` |
| `status/battery-low` | alias of `status/battery-level-20` |
| `status/battery-low-charging` | alias of `status/battery-level-20-charging` |
| `status/battery-good` | alias of `status/battery-level-70` |
| `status/battery-good-charging` | alias of `status/battery-level-70-charging` |
| `status/battery-full` | alias of `devices/battery` |
| `status/battery-full-charging` | alias of `status/battery-level-100-charging` |
| `status/battery-full-charged` | alias of `status/battery-level-100-charged` |

### Wi-Fi

| Icon | Status |
| --- | --- |
| `status/network-wireless` | alias of `status/network-wireless-signal-good` |
| `status/network-wireless-signal-excellent` | alias of `status/network-wireless-signal-good` |
| `status/network-wireless-signal-good` | existing |
| `status/network-wireless-signal-ok` | existing |
| `status/network-wireless-signal-weak` | existing |
| `status/network-wireless-signal-none` | existing |
| `status/network-wireless-disabled` | existing |
| `status/network-wireless-acquiring` | new |
| `status/network-wireless-offline` | new |
| `status/network-wireless-no-route` | new |
| `status/network-wireless-encrypted` | new |
| `status/network-wireless-hotspot` | new |

### Wired and general network

| Icon | Status |
| --- | --- |
| `status/network-wired` | alias of `devices/network-wired` |
| `status/network-wired-disconnected` | new |
| `status/network-wired-acquiring` | new |
| `status/network-wired-no-route` | new |
| `status/network-offline` | new |
| `status/network-vpn` | new |
| `status/network-vpn-acquiring` | new |
| `status/network-transmit-receive` | new |
| `status/network-transmit` | new |
| `status/network-receive` | new |
| `status/network-idle` | new |
| `status/network-error` | new |

### Cellular and airplane mode

| Icon | Status |
| --- | --- |
| `status/network-cellular-signal-none` | new |
| `status/network-cellular-signal-weak` | new |
| `status/network-cellular-signal-ok` | new |
| `status/network-cellular-signal-good` | new |
| `status/network-cellular-signal-excellent` | new |
| `status/network-cellular-offline` | new |
| `status/airplane-mode` | new |
| `status/airplane-mode-disabled` | new |

### Bluetooth

| Icon | Status |
| --- | --- |
| `status/bluetooth-active` | new |
| `status/bluetooth-disabled` | new |
| `status/bluetooth-disconnected` | new |
| `status/bluetooth-hardware-disabled` | new |

### Audio

| Icon | Status |
| --- | --- |
| `status/audio-volume-high` | existing |
| `status/audio-volume-medium` | existing |
| `status/audio-volume-low` | existing |
| `status/audio-volume-muted` | existing |
| `status/audio-volume-overamplified` | new |
| `status/microphone-sensitivity-high` | new |
| `status/microphone-sensitivity-medium` | new |
| `status/microphone-sensitivity-low` | new |
| `status/microphone-sensitivity-muted` | new |
| `devices/audio-input-microphone` | new |

### Brightness and notifications

| Icon | Status |
| --- | --- |
| `status/display-brightness` | new |
| `status/keyboard-brightness` | new |
| `status/night-light` | new |
| `status/notifications` | new |
| `status/notifications-disabled` | new |

### Session and Lens

| Icon | Status |
| --- | --- |
| `actions/system-shutdown` | existing |
| `actions/system-reboot` | new |
| `actions/system-log-out` | new |
| `actions/system-suspend` | new |
| `actions/system-lock-screen` | existing |
| `actions/system-switch-user` | new |
| `status/avatar-default` | new |
| `actions/system-search` | alias of `actions/edit-find` |
| `actions/view-app-grid` | redraw |
| `apps/accessories-calculator` | new |

### Privacy indicators

| Icon | Status |
| --- | --- |
| `devices/camera-web` | new |
| `actions/media-record` | new |
| `actions/find-location` | new |

## Tier 2: GTK and libadwaita widget icons

### Window controls and menus

| Icon | Status |
| --- | --- |
| `actions/window-close` | new |
| `actions/window-minimize` | new |
| `actions/window-maximize` | new |
| `actions/window-restore` | new |
| `actions/open-menu` | new |
| `actions/view-more` | new |
| `actions/view-more-horizontal` | new |
| `actions/pan-up` | new |
| `actions/pan-down` | new |
| `actions/pan-start` | new |
| `actions/pan-end` | new |
| `actions/object-select` | new |
| `status/process-working` | new |

### Entries and lists

| Icon | Status |
| --- | --- |
| `actions/view-reveal` | new |
| `actions/view-conceal` | new |
| `actions/edit-select-all` | new |
| `actions/view-list` | new |
| `actions/view-grid` | new |
| `actions/view-sort-ascending` | new |
| `actions/view-sort-descending` | new |
| `actions/sidebar-show` | new |
| `actions/sidebar-show-right` | new |
| `actions/zoom-in` | new |
| `actions/zoom-out` | new |
| `actions/zoom-original` | new |
| `actions/zoom-fit-best` | new |
| `actions/tab-new` | new |
| `actions/view-pin` | new |
| `status/starred` | new |
| `status/non-starred` | new |

### Documents and dialogs

| Icon | Status |
| --- | --- |
| `actions/document-open` | new |
| `actions/document-open-recent` | new |
| `actions/document-save-as` | new |
| `actions/document-edit` | new |
| `actions/document-properties` | new |
| `actions/document-send` | new |
| `status/dialog-error` | new |
| `status/dialog-question` | new |
| `status/dialog-password` | new |
| `actions/help-about` | new |
| `categories/preferences-system` | new |

### Media

| Icon | Status |
| --- | --- |
| `actions/media-playback-start` | new |
| `actions/media-playback-pause` | new |
| `actions/media-playback-stop` | new |
| `actions/media-skip-forward` | new |
| `actions/media-skip-backward` | new |
| `actions/media-seek-forward` | new |
| `actions/media-seek-backward` | new |
| `actions/media-playlist-shuffle` | new |
| `actions/media-playlist-repeat` | new |

### Text formatting

| Icon | Status |
| --- | --- |
| `actions/format-text-bold` | new |
| `actions/format-text-italic` | new |
| `actions/format-text-underline` | new |
| `actions/format-text-strikethrough` | new |
| `actions/format-justify-left` | new |
| `actions/format-justify-center` | new |
| `actions/format-justify-right` | new |
| `actions/format-justify-fill` | new |
| `actions/insert-image` | new |
| `actions/insert-link` | new |

### GTK emoji chooser tabs

| Icon | Status |
| --- | --- |
| `categories/emoji-recent` | new |
| `categories/emoji-people` | new |
| `categories/emoji-body` | new |
| `categories/emoji-nature` | new |
| `categories/emoji-food` | new |
| `categories/emoji-travel` | new |
| `categories/emoji-activities` | new |
| `categories/emoji-objects` | new |
| `categories/emoji-symbols` | new |
| `categories/emoji-flags` | new |

## Tier 3: Places, devices, file types, emblems, Settings, weather

### Places

| Icon | Status |
| --- | --- |
| `places/user-home` | new |
| `places/user-bookmarks` | new |
| `places/folder-documents` | new |
| `places/folder-download` | new |
| `places/folder-music` | new |
| `places/folder-pictures` | new |
| `places/folder-videos` | new |
| `places/folder-templates` | new |
| `places/folder-publicshare` | new |
| `places/inode-directory` | alias of `places/folder` |

### Devices

| Icon | Status |
| --- | --- |
| `devices/computer` | new |
| `devices/phone` | new |
| `devices/tablet` | new |
| `devices/camera-photo` | new |
| `devices/audio-headphones` | new |
| `devices/audio-headset` | new |
| `devices/audio-speakers` | new |
| `devices/audio-card` | new |
| `devices/input-gaming` | new |
| `devices/input-tablet` | new |
| `devices/input-touchpad` | new |
| `devices/printer` | new |
| `devices/scanner` | new |
| `devices/media-flash` | new |
| `devices/media-removable` | new |
| `devices/drive-harddisk-solidstate` | new |
| `devices/bluetooth` | new |

### File types

| Icon | Status |
| --- | --- |
| `mimetypes/text-x-generic` | new |
| `mimetypes/image-x-generic` | new |
| `mimetypes/video-x-generic` | new |
| `mimetypes/audio-x-generic` | alias of `apps/audio-x-generic` |
| `mimetypes/package-x-generic` | new |
| `mimetypes/application-x-executable` | new |
| `mimetypes/text-x-script` | new |
| `mimetypes/font-x-generic` | new |
| `mimetypes/x-office-document` | new |
| `mimetypes/x-office-spreadsheet` | new |
| `mimetypes/x-office-presentation` | new |

### Emblems

| Icon | Status |
| --- | --- |
| `emblems/emblem-ok` | new |
| `emblems/emblem-important` | new |
| `emblems/emblem-shared` | new |
| `emblems/emblem-symbolic-link` | new |
| `emblems/emblem-readonly` | new |
| `emblems/emblem-synchronizing` | new |
| `emblems/emblem-favorite` | new |

### Settings pages

| Icon | Status |
| --- | --- |
| `apps/preferences-desktop-appearance` | new |
| `apps/preferences-desktop-wallpaper` | new |
| `apps/preferences-desktop-display` | new |
| `apps/preferences-desktop-keyboard` | new |
| `apps/preferences-desktop-accessibility` | new |
| `apps/preferences-system-privacy` | new |
| `apps/preferences-system-time` | new |
| `apps/preferences-system-notifications` | new |
| `apps/system-users` | new |

### Weather

| Icon | Status |
| --- | --- |
| `status/weather-fog` | new |
| `status/weather-fog.filled` | new |
| `status/weather-windy` | new |
| `status/weather-windy.filled` | new |
| `status/weather-tornado` | new |
| `status/weather-tornado.filled` | new |

## Redrawn existing icons

| Icon | Change |
| --- | --- |
| `emotes/face-angel` | moved from a 40×40 to the 120×120 canvas |
| `emotes/face-crying` | moved from a 40×40 to the 120×120 canvas |
| `emotes/face-devil-grin` | moved from a 40×40 to the 120×120 canvas |
| `emotes/face-glasses` | moved from a 40×40 to the 120×120 canvas |
| `emotes/face-grin` | moved from a 40×40 to the 120×120 canvas |
| `emotes/face-kiss` | moved from a 40×40 to the 120×120 canvas |
| `emotes/face-monkey` | moved from a 40×40 to the 120×120 canvas |
| `emotes/face-plain` | moved from a 40×40 to the 120×120 canvas |
| `emotes/face-sad` | moved from a 40×40 to the 120×120 canvas |
| `emotes/face-smile-big` | moved from a 40×40 to the 120×120 canvas |
| `emotes/face-smile` | moved from a 40×40 to the 120×120 canvas |
| `emotes/face-surprise` | moved from a 40×40 to the 120×120 canvas |
| `emotes/face-wink` | moved from a 40×40 to the 120×120 canvas |
| `status/weather-showers` | moved from a 40×40 to the 120×120 canvas |
| `status/weather-showers.filled` | moved from a 40×40 to the 120×120 canvas |
| `status/weather-showers-scattered` | moved from a 40×40 to the 120×120 canvas |
| `status/weather-showers-scattered.filled` | moved from a 40×40 to the 120×120 canvas |
| `status/weather-snow` | moved from a 40×40 to the 120×120 canvas |
| `status/weather-snow.filled` | moved from a 40×40 to the 120×120 canvas |
| `status/weather-storm` | moved from a 40×40 to the 120×120 canvas |
| `status/weather-storm.filled` | moved from a 40×40 to the 120×120 canvas |
| `actions/view-app-grid` | added at 7-unit weight; the earlier copy used 3-unit lines |
