# MomentMark — Releases

This repository exists only to host **release assets** for
[MomentMark](https://github.com/RobertoM80/video-bookmarks-chrome-extension), the Chrome
extension for timestamped video notes and local transcription.

There is no source code here, and nothing here is edited by hand.

## The downloads are public on purpose

**The download is free. The licence unlocks features at runtime, not access to the file.**

Free and Pro are the **same binary**. The transcription helper verifies an Ed25519 licence
offline, on your own machine, and gates what it will do:

| | Free | Pro |
|---|---|---|
| Model | small | `large-v3-turbo` |
| Length per video | ~15 minutes | unlimited |
| Batch queue | no | yes |

The free tier is meant to be genuinely usable, not a crippled demo.

Putting the installer behind a password would mean authentication infrastructure, expiring
links, support tickets, and a broken auto-updater — for a gate that the licence check
already provides, better and offline.

## Why a separate repository

Release assets on a **private** repository require authentication to download, so an
auto-updater cannot point at them. The MomentMark source repository is private because the
Python helper is proprietary.

A public releases-only repository solves that without publishing any code.

## What gets published here

| Asset | Description |
|---|---|
| `MomentMark-Transcription-Helper-Setup-x64.exe` | Windows installer for the local transcription helper |
| `momentmark-mvp.zip` | Packaged extension |
| `momentmark-release.json` | Release manifest read by the extension |

Assets are published automatically by the release workflow in the source repository when a
`v*` tag is pushed.

## Reporting problems

Open issues against the
[source repository](https://github.com/RobertoM80/video-bookmarks-chrome-extension/issues),
not here.
