# Item Infos

Item Infos is a data pack for Minecraft: Java Edition which displays information based on the player's currently held item. It is designed to work as an immersive alternative to the F3 debug screen.

## About 

### Features

* Compass display with coordinates and direction
    * Detailed compass display with more specific coordinates and rotations
* Clock display with current time
    * Detailed clock display with in-game day and tick
    * 24-hour time config option
* Daylight detector display with current light level
    * Different colors for whether mobs can spawn (based on light level)
* Custom color configuration
* Custom item configuration
* Support for off-hand

### Other

I know the name is grammatically incorrect. It's just the style I chose :grin:

## Usage

Information is displayed based on what item you are holding and whether you are sneaking.

Holding a compass while not sneaking:
![Compass display with coordinates and direction](https://i.imgur.com/MAzekQl.png)

Holding a compass while sneaking:
![Detailed (sneaking) compass display with coordinates and rotations](https://i.imgur.com/FxA2qPw.png)

Holding a clock while not sneaking:
![Clock display with time in 12-hour time at sunrise](https://i.imgur.com/hzB05Ew.png)
![Clock display with time in 12-hour time at sunset](https://i.imgur.com/Jaf3V1W.png)

Holding a clock while sneaking:
![Detailed (sneaking) clock display with day and time in ticks](https://i.imgur.com/VKlyNR8.png)

Holding a daylight detector:
![Daylight detector display with current light level of 3](https://i.imgur.com/rUKMFoV.png)
![Daylight detector display with current light level of 9](https://i.imgur.com/ddLnwXM.png)

## Installation
### Step 1 - Download

(If you are on a Unix-based operating system, run `wget $(curl -s https://api.github.com/repos/SmoochyPit/Item-Infos/releases/latest | grep 'browser_' | cut -d\" -f4)` in the datapacks folder of your world)

1. Click [releases](https://github.com/SmoochyPit/Item-Infos/releases)
2. Find the latest release
3. Under assets, click "item-infos-vX.X.zip" to download the data pack. *This file **should not** be unzipped before installation*
4. Select one of the following methods for installing the data pack:

### Step 2 - Data pack menu (New singleplayer worlds) (Very Easy)

1. In the Singleplayer menu, click "Create New World"
2. Click "Data Packs"
3. Drag the downloaded file onto your Minecraft window (toggle fullscreen with F11)
4. Click "Yes"
5. Hover over Warp Pads in the menu and click the right arrow to add it to the list of selected data packs
6. Click "Done" and change any other world options you want
7. Click "Create New World"

### Step 2 - Manual installation (Existing singleplayer or multiplayer worlds) (Easy)

1. Place the downloaded file into the `[worldname]\datapacks` folder on your server or singleplayer world (located at `C:\Users\[user]\AppData\Roaming\.minecraft\saves\[worldname]\datapacks` by default in Windows)
2. Either restart the world or server, or run the `/reload` command.

At this point, Item Infos will now be installed in your Minecraft world.

### Support

Supports Minecraft: Java Edition 1.16-1.16.5. I plan to maintain this data pack for the 1.17 snapshots.

### Uninstalling

There is currently no way of cleanly uninstalling this data pack. Removing it will leave behind objectives. I plan to add an uninstallation function in the near-future.

### Configuration

Configuration is handled by Trident during compilation. To compile the modified version of the data pack, you will need either [Trident UI](https://github.com/Energyxxer/Trident-UI) or [Trident Language](https://github.com/Energyxxer/Trident-Language).

1. Download and extract the source code
    * If using Trident UI, place this folder in your workspace folder
2. Change the output location in the file `.tdnproj`
    * If using Trident UI, this option is found under `File > Project Properties > Output > Data Pack Output` (Make sure to select the project in the explorer panel)
3. Config is located at `datapack\data\smoochypit\functions\iteminfos\config.tdn`
4. Compile the project (Alt-Shift-X in Trident UI)

## Credits

Created with http://energyxxer.com/trident/. (https://github.com/Energyxxer/Trident-UI)

Made with love by @SmoochyPit