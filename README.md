# Emby for Kodi — Drivemby edition

This is a modified version of [Emby for Kodi Next Gen](https://github.com/MediaBrowser/plugin.video.emby) by quickmic and the MediaBrowser team. It adds compatibility with [Drivemby](https://drivemby.com), a cloud service with an Emby-compatible API.

What it changes for Drivemby:

- Login, session handshake, request bodies and boolean query parameters follow what Drivemby accepts
- Rate-limited requests (HTTP 429) back off and retry
- Library sync works without file paths and without missing metadata fields, and expands box sets into their movies
- Item IDs are handled as strings, since Drivemby IDs are not numeric
- Playback progress is reported with a Drivemby-issued play session, so resume points sync back

It still works with a regular Emby server. The `drivemby` branch follows upstream's `next-gen-dev-python3` branch, so upstream fixes can be merged in.

Licensed under the GNU GPL v3, the same as upstream (see `LICENSE.txt`). Not affiliated with Emby or Drivemby.

___

# Emby for Kodi

[![EmbyKodi_Banner](https://i.imgur.com/hx4cx41.png)](https://emby.media/community/index.php?/forum/99-kodi/)

[![Wiki](https://img.shields.io/badge/get%20started-wiki-brightgreen.svg)](https://github.com/MediaBrowser/plugin.video.emby/wiki) 
[![Forums](https://img.shields.io/badge/report%20issues-forums-3960C1.svg)](https://emby.media/community/index.php?/forum/99-kodi/)
[![Emby for Kodi objects](https://img.shields.io/badge/patch-objects-3960C1.svg)](https://github.com/MediaBrowser/plugin.video.emby.objects)
[![Emby](https://img.shields.io/badge/server-emby-52b54b.svg)](https://emby.media/)

___
**A whole new way to manage and view your media library.**

The Emby for Kodi add-on combines the best of Kodi - ultra smooth navigation, beautiful UIs and playback of any file under the sun, and Emby - the most powerful open source multi-client media metadata indexer and server. You can now retire your MySQL setup in favor of a more flexible setup.

Synchronize your media on your Emby server to the native Kodi database, browsing your media at full speed, while retaining the ability to use other Kodi add-ons to enhance your experience. In addition, you can use any Kodi skin you'd like!
___

### Supported

The add-on supports a hybrid approach. You can decide which Emby libraries to sync to the Kodi database. Other libraries and features are accessible dynamically, as a plugin listing.
- Library types available to sync:
  + Movies and sets
  + TV shows
  + Music videos
  + Music
- Other features supported:
  + Simple Live TV presentation
  + Home Videos & photos
  + Playlists
  + Theme media
- Direct play and transcode
- A 2-way watched and resume state between your server and Kodi. This is a near instant feature.
- Remote control your Kodi; send play commands from your Emby web client or Emby mobile apps.
- Extrafanart (rotating backgrounds) for skins that support it
- Offer to delete content after playback
- Backup your emby kodi profile. See the [Emby backup option](https://github.com/MediaBrowser/plugin.video.emby/wiki/Create-and-restore-from-backup)
- and more...

### Install Emby for Kodi
Get started with the [wiki guide](https://github.com/MediaBrowser/plugin.video.emby/wiki)

### Known limitations
- ~~Chapter images are missing unless native playback mode is used.~~
- Certain add-ons that depend on seeing where your content is located will not work unless native playback mode is selected.

___
### Help translate
Check [Transifex](https://www.transifex.com/emby-for-kodi/emby-for-kodi/stringspo/) to help translate this project. Thank you!
