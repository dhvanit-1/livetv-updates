# livetv-updates

Update files for **Last TV** (formerly Live TV), a personal-use live-channel app for Android TV.
Only this update repository is public; the app's code is private.

## Disclaimer

Last TV hosts nothing and holds no rights to any channel. It is only a front end: every stream is
read from publicly available lists and free services, or opened in another app on the TV. If you
use it, you do so **at your own risk**.

## Install

1. Download `live-tv.apk` from the [latest release](https://github.com/dhvanit-1/livetv-updates/releases/latest).
2. Install it on the TV (open the file there, or `adb install live-tv.apk`).

After that the app updates itself: it checks this repository, and installs a new version only when
its files carry the right signature.

## Requirements

- An **Android TV** (not phones or tablets), Android 8.0 or newer, ARM (armeabi-v7a / arm64-v8a).
- Nothing else for most channels.
- Optional:
  - A **JioTV sign-in** (Settings → JioTV account, with your own Jio number) for the channels that
    come from JioTV.
  - **SmartTube**, for the channels that are only on YouTube.

## What the app does

- Channels from several sources merged into one list, by language and genre, with favourites,
  search and a "what's on now" panel.
- Each channel's streams are tried in order until one plays. The sources are shown as numbers, and
  their order can be changed in Settings.
- Opens in a few seconds from the list it saved last time, then refreshes in the background.

## Files

| File | What it is |
|---|---|
| `manifest.json` + `manifest.json.sig` | The current version and where its APK is, signed. TVs ignore unsigned or changed files. |
| `sources.json` | Channel fixes and extra lists that reach TVs without an app update. |
| Releases → `live-tv.apk` | The app itself. |

## Credits

- Channel lists: [Famelack](https://github.com/famelack/famelack-data) (MIT licence) and
  [iptv-org](https://github.com/iptv-org/iptv).
- JioTV sign-in and playback follow [jiotv_go](https://github.com/JioTV-Go/jiotv_go)
  (CC BY 4.0).
- Free ad-supported channel lists (Samsung TV Plus, LG Channels) from community-maintained
  playlists.
- [SmartTube](https://github.com/yuliskov/SmartTube) for the YouTube channels.
