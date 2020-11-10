# Mac Terminal Customized Config

## Demo:
![](https://i.imgur.com/xi4PH3i.png)

## Get Started

### `Preferences setting`
![](https://i.imgur.com/HRsjtth.png)

### `font`
SauceCodePro Nerd Font

### `.zshrc`

```bash=
# Fix prompt at the bottom of the terminal window
printf '\n%.0s' {1..100}
alias cl='clear &&  printf "\n%.0s" {1..100}'
```

### `.p10k.zsh`

customize p10k dir color and `source ~/.p10k.zsh`

```
typeset -g POWERLEVEL9K_DIR_MAX_LENGTH=20

.
.
.

  ##################################[ dir: current directory ]##################################
  # Current directory background color.
  typeset -g POWERLEVEL9K_DIR_BACKGROUND=4
  # Default current directory foreground color.
  typeset -g POWERLEVEL9K_DIR_FOREGROUND=254
  typeset -g POWERLEVEL9K_DIR_FOREGROUND=0
  # If directory is too long, shorten some of its segments to the shortest possible unique
  # prefix. The shortened directory can be tab-completed to the original.
  typeset -g POWERLEVEL9K_SHORTEN_STRATEGY=truncate_to_unique
  # Replace removed segment suffixes with this symbol.
  typeset -g POWERLEVEL9K_SHORTEN_DELIMITER=
  # Color of the shortened directory segments.
  typeset -g POWERLEVEL9K_DIR_SHORTENED_FOREGROUND=250
  typeset -g POWERLEVEL9K_DIR_SHORTENED_FOREGROUND=232
  # Color of the anchor directory segments. Anchor segments are never shortened. The first
  # segment is always an anchor.
  typeset -g POWERLEVEL9K_DIR_ANCHOR_FOREGROUND=255
  typeset -g POWERLEVEL9K_DIR_ANCHOR_FOREGROUND=232
  # Display anchor directory segments in bold.
  typeset -g POWERLEVEL9K_DIR_ANCHOR_BOLD=false
  # Don't shorten directories that contain any of these files. They are anchors.
```
