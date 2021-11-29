# Install [Homebrew](https://brew.sh):

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

# Install essentials

Using `brew`:

```sh
brew install fira-code  # Font
brew install fish       # Fish Shell
brew install starship   # Starship prompt
brew install fnm        # Fish Node Manager
brew install php        # PHP
brew install composer   # Composer
brew install golang     # Go
```

# Fish Config

```
❯ cat config.fish
 
if status --is-interactive
  starship init fish | source
  fnm env --multi | source
  eval (/opt/homebrew/bin/brew shellenv)
  set -U fish_user_paths /opt/homebrew/bin $fish_user_paths
  set -U fish_user_paths /opt/homebrew/sbin $fish_user_paths
end
```

# Change default shell

```
chsh -s $(which fish)
```

# Set up macOS terminal

Install the terminal profile under `resources/FishPro.terminal` by double-clicking on it.
