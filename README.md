# Omniclip 
General clipboard/playlist manager using dmenu.

## Requirements
- dmenu
- yt-dlp

## Features
- Saves items in text files (by default in ```~/.local/share/omniclip/[clipboards or playlists]```) and retrieves them using a simple tag system.
- Built-in link handler to open clipboard items (use the ```-O``` flag to open an item given as first argument).
- Download clipboards items using different presets (use the ```-D``` flag to download an item given as first argument).
- Using a clipboard often? You can use the ```-q``` file to quickly select an item by providing the clipboard and the tag.
- Playlist modes, including play in-order, shuffle play, and "consume" play, which deletes each item after playing.

## Usage
```
omniclip [-gbiodh]
  -g: general mode. prompts user for save, open, download or play the item currently in the system clipboard.
  -b: browse mode. prompts user for either a clipboard or a playlist, and then for the action to perform.
  -i: quick insert a new item taken from the clipboard into a local clipboard or playlist.
  -o: quick open an item from a local clipboard or playlist. 
  -d: quick download an item from a local clipboard or playlist.
  -I: quick insert a new item given as first argument into a local clipboard or playlist.
  -O: quick open an item given as first argument. 
  -D: quick download an item given as first argument
  -q: super-quick selection of a clipboard (first argument) given a tag (second argument)
  -h: prints this help section.
```
