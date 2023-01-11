# IPFS Integrations tracking
Here we track the application in which we want to support IPFS.

## Submit applications
As a general rule of thumb, any application that can use web resources (http/https) is a potential candidate to integrate IPFS support into.
Create an issue in the issue tracker of this repository to let us know which application needs IPFS integration.

## Completed integrations
These integrations have been fully developed and merged in their upstream projects. A release might or might not have been made yet.
* [FFmpeg](https://ffmpeg.org/) 5.1 has IPFS support.
  * Usage: `ffplay ipfs://<cid>` or your regular `ffmpeg` command where any input source can be an IPFS resource now.
  * Example usecase: Your video encode/transcode can now use input resources from IPFS.
  * Docs can be found [here](https://ffmpeg.org/ffmpeg-protocols.html#ipfs) and the commit enabling IPFS support can be found [here](https://github.com/FFmpeg/FFmpeg/commit/f889837e00d3b2388a24c0a9d075ad62f47da825).
* [MPV](https://mpv.io/)
  * Usage: `mpv ipfs://<cid>`
  * Example usecase: This is purely a mediaplayer on top of FFmpeg. `mpv ipfs://<cid>` would start playing your media.
  * There are no specific `mpv` docs with `IPFS` because it's a protocol passthrough from mpv directly to FFmpeg. The commit enabling IPFS support can be found [here](https://github.com/mpv-player/mpv/commit/3458651010a68c2384a19ba485e81e22c825782f).

## Pending integrations
* [cURL](https://curl.se/) WIP [PR](https://github.com/curl/curl/pull/8805#issuecomment-1179758610)
  * Usage: `curl ipfs://<cid>`
  * Example usecase: Download/access data from cURL. You can use this in scripts or even just as a quick way to download data from IPFS.
