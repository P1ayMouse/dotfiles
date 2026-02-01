# dotfiles

My Zsh configuration managed with `chezmoi`.

## What is included
- `.zshrc` (Zinit + productivity plugins)

## Setup on a clean macOS profile

1) Install Homebrew:
```bash
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

2) 	Install chezmoi:
```bash
  brew install chezmoi
```

3) Init and apply dotfiles:
```bash
  chezmoi init P1ayMouse (your github username)
  chezmoi apply
```

4) Install zinit (plugin manager):
```bash
  bash -c "$(curl -fsSL https://raw.githubusercontent.com/zdharma-continuum/zinit/HEAD/scripts/install.sh)"
```

5) Install tools used in .zshrc:
```bash
  brew install fzf starship vivid
  $(brew --prefix)/opt/fzf/install
```

6) Reload shell:
```bash
  exec zsh
```