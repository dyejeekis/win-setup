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

#### Startup
```
$ws=New-Object -ComObject WScript.Shell;
$s=$ws.CreateShortcut("$env:APPDATA\Microsoft\Windows\Start Menu\Programs\Startup\GlazeWM.lnk");
$s.TargetPath="$env:USERPROFILE\scoop\apps\glazewm\current\glazewm";
$s.WorkingDirectory="$env:USERPROFILE\scoop\apps\glazewm\current";
$s.Save();
```

*TODO: start apps like Glaze after creating their startup shortcut?*

--------------------------------------------------------------
# Configs

## Powershell

```
Set-Location (New-Item -ItemType Directory -Path ~\Documents\PowerShell -Force).FullName # powershell config;
git init;
git remote add origin https://github.com/dyejeekis/powershell-config.git;
git fetch origin;
git checkout -b main --track origin/main;
```

Run this after every zoxide installation or update
```
zoxide init powershell | Out-File -FilePath $PROFILE\..\zoxide_init.ps1 -Encoding UTF8 # zoxide update
```

## Wezterm

```
Set-Location (New-Item -ItemType Directory -Path ~\.config\wezterm -Force).FullName # wezterm config;
git init;
git remote add origin https://github.com/dyejeekis/wezterm-config.git;
git fetch origin;
git checkout -b main --track origin/main;
```

## Neovim

```
Set-Location (New-Item -ItemType Directory -Path ~\AppData\Local\nvim -Force).FullName # neovim config;
git init;
git remote add origin https://github.com/dyejeekis/neovim-config.git;
git fetch origin;
git checkout -b main --track origin/main;
```

## IdeaVim

```
Set-Location (New-Item -ItemType Directory -Path ~\.ideavim -Force).FullName # ideavim config;
git init;
git remote add origin https://github.com/dyejeekis/ideavim-config.git;
git fetch origin;
git checkout -b main --track origin/main;
Copy-Item ~\.ideavim\.ideavimrc ~ -Force; # replace ideavim config
```

## GlazeWM & Zebar

```
Set-Location (New-Item -ItemType Directory -Path ~\.glzr -Force).FullName # glazewm config;
git init;
git remote add origin https://github.com/dyejeekis/glazewm-config.git;
git fetch origin;
git checkout -b glaze-new --track origin/glaze-new;
```

## Yazi

```
Set-Location (New-Item -ItemType Directory -Path ~\AppData\Roaming\yazi\config -Force).FullName # yazi config;
git init;
git remote add origin https://github.com/dyejeekis/yazi-config.git;
git fetch origin;
git checkout -b main --track origin/main;
```

## Lazygit

```
Set-Location (New-Item -ItemType Directory -Path ~\AppData\Local\lazygit -Force).FullName # lazygit config;
git init;
git remote add origin https://github.com/dyejeekis/lazygit-config.git;
git fetch origin;
git checkout -b main --track origin/main;
```

## MPV

```
Set-Location (New-Item -ItemType Directory -Path ~\scoop\apps\mpv\current\portable_config -Force).FullName # mpv config;
git init;
git remote add origin https://github.com/dyejeekis/mpv-config.git;
git fetch origin;
git checkout -b main --track origin/main;
```

--------------------------------------------------------------
# Other

## Autohotkey

```
cd ~;
git clone https://github.com/dyejeekis/autohotkey-scripts.git;
Copy-Item ~\autohotkey-scripts\no_taskbar_mouseover.ahk "$env:APPDATA\Microsoft\Windows\Start Menu\Programs\Startup";
cd ~\autohotkey-scripts;
.\no_taskbar_mouseover.ahk;
```
