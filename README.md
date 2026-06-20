<p align="center">
  <img src="https://raw.githubusercontent.com/developic/developic/refs/heads/main/images/chubby-cute.gif" width="600" alt="Banner Cat">
</p>

# fzf-tab

Fish shell completion using fzf (simple, no bullshit, and fast as hell)

## Requirements

- Fish
- fzf
- eza (optional, for directory previews)
- bat (optional, for file previews)

## Installation

Install with [Fisher](https://github.com/jorgebucaran/fisher):

```fish
fisher install developic/fzf-tab
```

Simple installation without Fisher:

```fish
curl https://gist.githubusercontent.com/developic/643a0384bd911ec09d43850cddf45688/raw/9c1932b9eb25c4bf83a79a29a3473fdd3149de32/fzf-tab.fish -o ~/.config/fish/functions/__fzf_complete.fish && echo 'bind \t __fzf_complete' >> $XDG_CONFIG_HOME/fish/config.fish
```

## Usage

Press `Tab` to open the fzf completion menu.

Select an entry and press `Enter` to insert it.

## Configuration

You can set `$fzf_complete_opts` for extra fzf flags:

```fish
set -g fzf_complete_opts --border --cycle --info=inline
```
