# Windows Settings

- Personalization -> Taskbar
- System -> Power & battery
- System -> Multitasking
- Folder options -> Show hidden files, folders and drives

--------------------------------------------------------------
# Packages

## Winget

```
winget install Microsoft.Powershell;
winget install Microsoft.Powertoys;
winget install Zen-team.Zen-Browser;
winget install Valve.Steam;
winget install XPFM5P5KDWF0JP # viber;
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
scoop install autohotkey wezterm neovim gh lazygit zoxide xh jq fzf zig nodejs pnpm yazi mpv fd ffmpeg poppler pandoc ripgrep unar spotify discord telegram onlyoffice-desktopeditors xnviewmp jpegview glazewm zebar godot syncthing cursor everything qbittorrent pia-desktop hwinfo obsidian firefox;
```


--------------------------------------------------------------
# Configs

First switch to a temp directory like Downloads

```
cd ~\Downloads
```

## Powershell (new)

```
Set-Location (New-Item -ItemType Directory -Path ~\Documents\PowerShell -Force).FullName # powershell config;
git init;
git remote add origin https://github.com/dyejeekis/powershell-config.git;
git fetch origin;
git checkout -b main --track origin/main;
```
## Powershell

```
git clone https://github.com/dyejeekis/powershell-config.git;
Copy-Item ~\Downloads\powershell-config\* ~\Documents\PowerShell\ -Recurse -Force;
cd ~\Documents\PowerShell # powershell config;
cd ~\Downloads;
```

Run this after every zoxide installation or update
```
zoxide init powershell | Out-File -FilePath $PROFILE\..\zoxide_init.ps1 -Encoding UTF8 # zoxide update
```

## Wezterm (new)

```
Set-Location (New-Item -ItemType Directory -Path ~\.config\wezterm -Force).FullName # wezterm config;
git init;
git remote add origin https://github.com/dyejeekis/wezterm-config.git;
git fetch origin;
git checkout -b main --track origin/main;
```
## Wezterm

```
git clone https://github.com/dyejeekis/wezterm-config.git;
Copy-Item ~\Downloads\wezterm-config\* ~\.config\wezterm\ -Recurse -Force;
cd ~\.config\wezterm # wezterm config;
cd ~\Downloads;
```

## Neovim (new)

```
Set-Location (New-Item -ItemType Directory -Path ~\AppData\Local\nvim -Force).FullName # neovim config;
git init;
git remote add origin https://github.com/dyejeekis/neovim-config.git;
git fetch origin;
git checkout -b main --track origin/main;
```

## Neovim

```
git clone https://github.com/dyejeekis/neovim-config.git;
Copy-Item ~\Downloads\neovim-config ~\AppData\Local\nvim\ -Recurse -Force;
cd ~\AppData\Local\nvim # neovim config;
cd ~\Downloads;
```

## IdeaVim (new)

```
Set-Location (New-Item -ItemType Directory -Path ~\.ideavim -Force).FullName # ideavim config;
git init;
git remote add origin https://github.com/dyejeekis/ideavim-config.git;
git fetch origin;
git checkout -b main --track origin/main;
Copy-Item ~\.ideavim\.ideavimrc ~ -Force; # replace ideavim config
```
## IdeaVim

```
git clone https://github.com/dyejeekis/ideavim-config.git;
Copy-Item ~\Downloads\ideavim-config\* ~\.ideavim\ -Recurse -Force;
Copy-Item ~\.ideavim\.ideavimrc ~ -Force;
cd ~\.ideavim # ideavim config;
cd ~\Downloads;
```

## GlazeWM & Zebar (new)

```
Set-Location (New-Item -ItemType Directory -Path ~\.glzr -Force).FullName # glazewm config;
git init;
git remote add origin https://github.com/dyejeekis/glazewm-config.git;
git fetch origin;
git checkout -b glaze-new --track origin/glaze-new;
```

## GlazeWM & Zebar

```
git clone --branch glaze-new --single-branch https://github.com/dyejeekis/glazewm-config.git;
Copy-Item ~\Downloads\glazewm-config\* ~\.glzr\ -Recurse -Force;
cd ~\.glzr # glazewm config;
cd ~\Downloads;
```

## Yazi (new)

```
Set-Location (New-Item -ItemType Directory -Path ~\AppData\Roaming\yazi\config -Force).FullName # yazi config;
git init;
git remote add origin https://github.com/dyejeekis/yazi-config.git;
git fetch origin;
git checkout -b main --track origin/main;
```

## Yazi

```
git clone https://github.com/dyejeekis/yazi-config.git;
Copy-Item ~\Downloads\yazi-config\* ~\AppData\Roaming\yazi\config\ -Recurse -Force;
cd ~\AppData\Roaming\yazi\config # yazi config;
cd ~\Downloads;
```

## Lazygit (new)

```
Set-Location (New-Item -ItemType Directory -Path ~\AppData\Local\lazygit -Force).FullName # lazygit config;
git init;
git remote add origin https://github.com/dyejeekis/lazygit-config.git;
git fetch origin;
git checkout -b main --track origin/main;
```

## Lazygit

```
git clone https://github.com/dyejeekis/lazygit-config.git;
Copy-Item ~\Downloads\lazygit-config\* ~\AppData\Local\lazygit\ -Recurse -Force;
cd ~\AppData\Local\lazygit # lazygit config;
cd ~\Downloads;
```

## MPV (new)

```
Set-Location (New-Item -ItemType Directory -Path ~\scoop\apps\mpv\current\portable_config -Force).FullName # mpv config;
git init;
git remote add origin https://github.com/dyejeekis/mpv-config.git;
git fetch origin;
git checkout -b main --track origin/main;
```

## MPV

```
git clone https://github.com/dyejeekis/mpv-config.git;
Copy-Item ~\Downloads\mpv-config\* ~\scoop\apps\mpv\current\portable_config\ -Recurse -Force;
cd ~\scoop\apps\mpv\current\portable_config # mpv config;
cd ~\Downloads;
```

--------------------------------------------------------------
# Other

*TODO*
