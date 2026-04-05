# SyndWarsFX Config -- custom settings

Custom configuration for SyndWarsFX 0.3.8.3830 (open-source port of Syndicate Wars).
Based on GOG Galaxy edition with additional gfx/sfx/levels packages from GitHub.

## How to launch

    syndwarsfx.exe /g -q

- `/g` -- campaign mode
- `-q` -- skip intro video

Fullscreen by default. Add `-W` for windowed mode.

## Changes from defaults

### config.ini

| Setting | Default | Custom | Notes |
|---------|---------|--------|-------|
| ResGameHi | 640x480x8 | 1920x1080x8 | Full HD gameplay |
| ResGameLo | 320x200x8 | 320x200x24 | 24-bit for compatibility |
| ResMenu | 640x480x8 | 640x480x8 | unchanged |
| ResFMVVidHi | 640x480x8 | 640x480x8 | unchanged |
| ResFMVidLo | 320x200x8 | 320x200x8 | unchanged |

### conf/rules.ini

| Setting | Default | Custom | Notes |
|---------|---------|--------|-------|
| ZoomMin | 145 | 1 | maximum zoom out range |
| ZoomMax | 263 | 100 | limits zoom in (less claustrophobic) |

## Keyboard controls (in-mission)

### Movement & agents
- Arrow keys -- move agents
- TAB -- cycle agent
- 1-4 -- select agent 1-4
- 5-0 -- select weapon 1-6
- LCTRL -- fire
- LALT -- change weapon (secondary slot)
- RCTRL -- go to point
- Z -- drop weapon
- D -- self destruct agent

### Camera
- +/- -- zoom out/in (rebind via Controls menu if HOME/END don't work)
- DELETE -- rotate camera left
- PGDOWN -- rotate camera right
- INSERT -- tilt camera up
- PGUP -- tilt camera down
- F -- camera perspective toggle (keep OFF for best view at 1080p)

### Visual
- CTRL+F6 -- Deep Radar (transparent buildings, toggle)
- B (hold) -- buildings invisible while held
- CTRL+F4 -- advanced lights toggle
- CTRL+F10 -- hide/show HUD panel
- F8 -- change resolution in-game
- H -- object line color
- J -- object surface color
- M -- screenshot

### Audio
- NUM7/NUM1 -- SFX volume +/-
- NUM8/NUM2 -- danger/tension volume +/-
- NUM9/NUM3 -- CD music volume +/-
- NUM5 -- music track
- NUM0 -- danger track

### Game
- NUM+ / NUM- -- game speed +/-
- P -- pause
- R -- restart mission
- SPACE -- skip menu animations

## Command line arguments

- `/g` -- campaign mode
- `-q` -- skip intro
- `-W` -- windowed mode
- `-d toc` -- debug mode (things/objectives/collision)
- `-m 1,48` -- start at specific mission
- `-H -q` -- high resolution mode
- `-S` -- no stretch for 320x200

## Editable config files (conf/)

- `rules.ini` -- zoom, scanner, research speed, revenue
- `weapons.ini` -- damage, range, cost, weight per weapon
- `cybmods.ini` -- cybernetic modifications
- `cities.ini` -- world map cities
- `miss000-099.ini` -- campaign paths and rewards
- `people.ini` -- base character stats

## Installation

Requires GOG edition of Syndicate Wars installed.
Port binary + DLLs from: https://github.com/swfans/syndwarsfx/releases
Additional packages: syndwarsfx-gfx, syndwarsfx-sfx, syndwarsfx-levels

## Links

- SyndWarsFX source: https://github.com/swfans/swars
- SyndWarsFX releases: https://github.com/swfans/syndwarsfx/releases
- Wiki: https://github.com/swfans/swars/wiki
