# livetv-updates

Update files for **Live TV**, a personal-use Android TV app. Only this update repository is public;
the app's code is private. The README will be expanded later.

## Disclaimer

Live TV hosts nothing and holds no rights to any channel. It is only a front end for public channel
lists and for other apps on the TV. If you use it, you do so **at your own risk**.

## Requirements

- An **Android TV** (not phones or tablets), Android 8.0 or newer, ARM (armeabi-v7a / arm64-v8a).
- Nothing else for most channels: install `live-tv.apk` and watch.
- If some channels don't play, install the optional apps:
  - **JTV Go**, for the channels that come from it.
  - **SmartTube**, if you want to watch the channels that are only on YouTube.

## Files

| File | What it is |
|---|---|
| `live-tv.apk` | The app. |
| `manifest.json` + `manifest.json.sig` | The current version, signed. TVs ignore unsigned or changed files. |
| `sources.json` | Channel fixes that reach TVs without an app update. |

## Credits

Channel lists from [Famelack](https://github.com/famelack/famelack-data) (MIT licence) and
[iptv-org](https://github.com/iptv-org/iptv); JTV Go and
[SmartTube](https://github.com/yuliskov/SmartTube) for their channels.
