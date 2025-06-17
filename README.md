# Spotify.nvim

A Neovim plugin to control Spotify with visual feedback.

## Usage

:SpotifyAuth - Start authentication process

:SpotifyToken <code> - Set auth token (after authenticating)

:SpotifyPlay - Play current track

:SpotifyPause - Pause current track

:SpotifyNext - Skip to next track

:SpotifyPrev - Go to previous track

:SpotifyVolume <0-100> - Set volume

:SpotifyUI - Toggle the Spotify UI window


## Dependencies


Neovim 0.7+

luasocket (for HTTP requests)

lua-cjson or similar JSON library

A web browser for authentication

## Features

- Play/pause/skip tracks
- Volume control
- Now playing display with cover art
- Progress bar
- Device selection

## Installation

Using packer.nvim:

```lua
use {
  'your-username/spotify.nvim',
  config = function()
    require('spotify').setup({
      client_id = "your-client-id",
      client_secret = "your-client-secret"
    })
  end
}
