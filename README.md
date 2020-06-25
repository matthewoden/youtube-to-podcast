# youtube-to-podcast

A quick script I created when the Critical Role podcast backlog kept getting removed from podbean.

## Usage

`youtube-to-podcast` takes a single argument - a youtube url. It downloads the best audio available, and then converts it to an mp3. 

If the source is already downloaded, it only downloads once. So if you have a ffmpeg conversion hiccup, you can just delete the mp3 and run it again.
``` bash
# outputs:
#
# m4a (youtube source) - Clash at Daxio _ Critical Role RPG Episode 77.m4a
# mp3 - Clash at Daxio - Critical Role RPG Episode 77.mp3
./youtube-to-podcast https://www.youtube.com/watch?v=43gRUYn4x_M
```

## Requirements

ffmpeg, and youtube-dl.

On mac, run:

```
brew install ffmpeg youtube-dl
```

...Or, install from the source:

- [youtube downloader](https://github.com/ytdl-org/youtube-dl)

- [fmpeg](https://github.com/FFmpeg/FFmpeg)

## TODO
- stop being lazy with bash, and optimize this to handle multiple files concurrently.
