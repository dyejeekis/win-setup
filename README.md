# Windows Settings

- Personalization -> Taskbar
- System -> Power & battery
- System -> Multitasking

--------------------------------------------------------------
# Packages (programs)

## Winget

```
winget install Microsoft.Powershell;
winget install Microsoft.Powertoys;
winget install Zen-team.Zen-Browser;
winget instasll Valve.Steam;
winget install XPFM5P5KDWF0JP;
```

## Scoop

#### Install Scoop
```
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser;
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression;
```

#### Packages
```
scoop install git;
scoop bucket add extras;
scoop bucket add versions;
scoop install autohotkey wezterm neovim lazygit zoxide xh jq fzf zig nodejs pnpm yazi mpv fd ffmpeg poppler pandoc ripgrep unar spotify discord telegram onlyoffice-desktopeditors xnviewmp jpegview glazewm zebar godot syncthing parsec cursor everything qbittorrent pia-desktop hwinfo obsidian firefox;
```


--------------------------------------------------------------
# Configs (dotfiles)

First switch to a temp directory like Downloads

```
cd ~\Downloads
```

## Powershell

```
git clone https://github.com/dyejeekis/powershell-config.git;
Copy-Item ~\Downloads\powershell-config -Destination ~\Documents -Recurse -Force;
```

```
zoxide init powershell | Out-File -FilePath $PROFILE\..\zoxide_init.ps1 -Encoding UTF8 # zoxide update
```

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
