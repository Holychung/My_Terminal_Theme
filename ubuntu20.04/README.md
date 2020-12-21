# WSL Terminal Customized Config

## Demo:
![](https://i.imgur.com/nFPFXgJ.png)

## Get Started

### Manual font installation

Download these four ttf files:

- [MesloLGS NF Regular.ttf](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Regular.ttf)
- [MesloLGS NF Bold.ttf](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold.ttf)
- [MesloLGS NF Italic.ttf](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Italic.ttf)
- [MesloLGS NF Bold Italic.ttf](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold%20Italic.ttf)


### `Terminal Perferances`

![](https://i.imgur.com/aJeGj3L.png)

![](https://i.imgur.com/IcB4ewW.png)


```json=
{
  "name": "Brogrammer",
  "black": "#1f1f1f",
  "red": "#f81118",
  "green": "#85D29A",
  "yellow": "#ecba0f",
  "blue": "#5C97CF",
  "purple": "#4e5ab7",
  "cyan": "#1081d6",
  "white": "#ffffff",
  "brightBlack": "#d6dbe5",
  "brightRed": "#de352e",
  "brightGreen": "#1dd361",
  "brightYellow": "#f3bd09",
  "brightBlue": "#1081d6",
  "brightPurple": "#5350b9",
  "brightCyan": "#0f7ddb",
  "brightWhite": "#ffffff",

  "background": "#2D2D2D",
  "foreground": "#d6dbe5"
}
```


### `.zshrc`

```bash=
alias gs="git status"
alias ga="git add"
alias gb="git branch"
alias gc="git commit"
alias gd="git diff"
alias gl="git log"
alias gco="git checkout"

# Fix prompt at the bottom of the terminal window
printf '\n%.0s' {1..100}
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
```
