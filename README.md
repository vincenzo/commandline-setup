- Install https://fishshell.com via the Installer on Mac
- Use https://github.com/starship/starship as prompt
- Use https://github.com/Schniz/fnm as Node version manager
- Manually [download and install](https://getcomposer.org/download/) Composer in custom `~/.bin` directory

# Fish Config

```
❯ cat config.fish 
starship init fish | source
fnm env --multi | source
```

# Fish User Path

```
# adds fnm binaries to the executable paths
set -U fish_user_paths ~/.fnm/ $fish_user_paths
# adds a custom ~/.bin to the executable paths
set -U fish_user_paths ~/.bin $fish_user_paths
```
