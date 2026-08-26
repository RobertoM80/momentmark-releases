# MomentMark — Releases

This repository exists only to host **release assets** for
[MomentMark](https://github.com/RobertoM80/video-bookmarks-chrome-extension), the Chrome
extension for timestamped video notes and local transcription.

There is no source code here.

## Why it is separate

The MomentMark extension downloads the transcription helper installer **without GitHub
authentication**, so the download URL has to be publicly readable. The source repository is
private — it contains the Python helper that is being prepared for commercial licensing.

Splitting only the *published binaries* into a public repository keeps the download
anonymous without publishing the code.

## What gets published here

| Asset | Description |
|---|---|
| `MomentMark-Transcription-Helper-Setup-x64.exe` | Windows installer for the local transcription helper |
| `momentmark-mvp.zip` | Packaged unpacked extension |
| `momentmark-release.json` | Release manifest read by the extension |

Assets are published automatically by the release workflow in the source repository when a
`v*` tag is pushed. Nothing here is edited by hand.

## Reporting problems

Open issues against the
[source repository](https://github.com/RobertoM80/video-bookmarks-chrome-extension/issues),
not here.
