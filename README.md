# 2DStarve (WIP)
![Image Capture of the Game](2DStarve.gif)

# About / FAQ
## What is this game about?
This game is a 2D multiplayer survival game focused on using natural resources to make technological advances to make survival easier, and is made by me and a friend (Kirin). While still a WIP due to school, we plan on adding various biomes, such as a forest, snowy mountain, desert, and a volcano, and add all wof their unique set of creatures and armor.
## Why did you make this game?
This game was created to be a fun side project to distract ourselves for school, and not meant to be profitable. We (Kirin & I) thought it would be fun to learn how to work as a team to make a game.
## What experience do you guys have?
I have been programming for 5+ years in robotics, web development, and software development. Kirin has been drawing for 4-5 years, and has been in band for a very long time. We made this game in hopes of broadening our horizons in the fields of network programming and pixel art.
## When will early access be released?
Probably next year; We have school.

# Running the game
## Windows
The game has been tested to run on Windows 10, and should run by simply running the executable.

## Linux
The game has been tested to run on Debian-based distributions, and should run by simply running the executable.


# 2DStarve-MapTutorial

## About
This is a tutorial to help you get started in making maps for 2DStarve v0.5.0 using [Tiled](https://www.mapeditor.org/). Currently, only the placement of dirt and grass tiles, not objects, are able to be done with [Tiled](https://www.mapeditor.org/). The latter will be implemented in a later release.

## Getting Started
![files](MapGuide/Files.PNG)

Firstly, download this project and go to `\Maps` to find the four files listed above. The files' purpose are as follows:
* `Grass_Tiles.png` is the raw image of the tiles.
* `Grass_Tiles.tsx` is the data file Tiled uses to grab them from the file with a few other extra stuff; I parsed them myself. It requires `Grass_Tiles.png`.
* `.tmx` files are the maps themselves. They require a `.tsx` file.

Feel free to view any of the `.tmx` files at your leisure.

To create your own map, go to `File > New Map` in Tiled. Copy the exact settings as shown below and save to wherever you like. The actual `Map Size` of the map doesn't matter; It can be infinite or fixed at any size.

![MapSettings](MapGuide/MapSettings.PNG)

After that, drag in `Grass_Tiles.tsx` into the `Tilesets` window; This will tell Tiled where to look for tile data.

![TilemapDrop](MapGuide/TilemapDrop.gif)


## Creating Maps
Tiled has a bunch of great, advanced tools that can be used for map development. For the purpose of this basic tutorial, I'll only cover the necessities.
* **Stamp Brush** - This is the most *basic* tool you'll use when adding tiles. Simply click on a tile from the tilemap and click on the map to automatically switch to it; Just like a stamp! ![Brush](MapGuide/Brush.gif)
* **Erase** - Erases tiles of a layer completely. ![Erase](MapGuide/Eraser.gif)
* **Terrain Brush** - This is a brush that automatically combines dirt and grass tiles to make drawing nice paths a lot easier. In the tilesets window, click `Terrains` and click the path you want to draw on and draw. **Note: You have to draw over blocks of the opposite type; Drawing over deleted terrain won't create edges.** ![TerrainBrush](MapGuide/TerrainBrush.gif)
* **Selection Tool** - Does exactly what you think it does. ![Selecion](MapGuide/Selection.gif)
* **Fill Tool** - Pretty intuitive; Fills up all "like" tiles. ![Fill](MapGuide/Fill.gif)
