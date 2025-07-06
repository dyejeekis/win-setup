# Windows Settings

- Personalization -> Taskbar
- System -> Power & battery
- System -> Multitasking

--------------------------------------------------------------
# Packages

## Winget

```
winget install Microsoft.Powershell;
winget install Microsoft.Powertoys;
winget install Zen-team.Zen-Browser;
winget install Valve.Steam;
winget install XPFM5P5KDWF0JP;
winget install BillStewart.SyncthingWindowsSetup;
winget install Parsec.Parsec;
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
scoop install autohotkey wezterm neovim lazygit zoxide xh jq fzf zig nodejs pnpm yazi mpv fd ffmpeg poppler pandoc ripgrep unar spotify discord telegram onlyoffice-desktopeditors xnviewmp jpegview glazewm zebar godot syncthing cursor everything qbittorrent pia-desktop hwinfo obsidian firefox;
```


--------------------------------------------------------------
# Configs

First switch to a temp directory like Downloads

```
cd ~\Downloads
```

## Powershell

```
git clone https://github.com/dyejeekis/powershell-config.git;
Copy-Item ~\Downloads\powershell-config\* -Destination ~\Documents\PowerShell -Recurse -Force;
```

Run this after every zoxide installation or update
```
zoxide init powershell | Out-File -FilePath $PROFILE\..\zoxide_init.ps1 -Encoding UTF8 # zoxide update
```

## Wezterm

```
git clone https://github.com/dyejeekis/wezterm-config.git;
Copy-Item ~\Downloads\wezterm-config\* -Destination ~\.config\wezterm -Recurse -Force;
```

## Neovim

```
git clone https://github.com/dyejeekis/neovim-config.git;
Copy-Item ~\Downloads\neovim-config\* -Destination ~\AppData\Local\nvim -Recurse -Force;
```

## IdeaVim

```
git clone https://github.com/dyejeekis/ideavim-config.git;
Copy-Item ~\Downloads\ideavim-config\* -Destination ~\.ideavim -Recurse -Force;
Copy-Item ~\.ideavim\.ideavimrc -Destination ~ -Force;
```

## GlazeWM & Zebar

```
git clone --branch glaze-new --single-branch https://github.com/dyejeekis/glazewm-config.git;
Copy-Item ~\Downloads\glazewm-config\* -Destination ~\.glzr -Recurse -Force;
```

## Yazi

```
git clone https://github.com/dyejeekis/yazi-config.git;
Copy-Item ~\Downloads\yazi-config\* -Destination ~\AppData\Roaming\yazi\config -Recurse -Force;
```

## Lazygit

```
git clone https://github.com/dyejeekis/lazygit-config.git;
Copy-Item ~\Downloads\lazygit-config\* -Destination ~\AppData\Local\lazygit -Recurse -Force;
```

## MPV

```
git clone https://github.com/dyejeekis/mpv-config.git;
Copy-Item ~\Downloads\mpv-config\* -Destination ~\scoop\apps\mpv\current\portable_config -Recurse -Force;
```

--------------------------------------------------------------
# Other

*TODO*
