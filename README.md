# Windows 11 Master Setup Guide
--------------------------------------------------------------
# Windows Settings

*TODO*

--------------------------------------------------------------
# Packages (programs)

## Winget

```
winget install Microsoft.Powershell;
winget install Microsoft.Powertoys;
winget install Zen-team.Zen-Browser;
winget install 9NBLGGH5R558;
winget install XPFM5P5KDWF0JP;
```

## Scoop

#### Install Scoop
```
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser;
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```

#### Packages
```
scoop bucket add extras;
scoop bucket add versions;
scoop install 7zip autohotkey wezterm neovim git lazygit zoxide xh jq fzf zig nodejs pnpm yazi mpv fd ffmpeg poppler pandoc ripgrep unar steam spotify discord telegram onlyoffice-desktopeditors xnviewmp jpegview glazewm godot syncthing parsec cursor everything qbittorrent pia-desktop hwinfo obsidian
```

(check if zebar is installed alongside glazewm)

--------------------------------------------------------------
# Configs (dotfiles)

## Powershell

*TODO*

## Wezterm

*TODO*

## Neovim

*TODO*

## IdeaVim

*TODO*

## GlazeWM & Zebar

*TODO*

## Yazi

*TODO*

## Lazygit

*TODO*

## MPV

*TODO*

--------------------------------------------------------------
# Other

*TODO*
