# Factorio Space Exploration (SE) Setup

## Basic setup

1. Create a new folder somewhere ( Desktop, my documents, anywhere )

- For these instruction, I'll use `D:\Factorio Server` as an example.

2. Download this repository there
   - On github, click the green _Code_ button, coohse _Download ZIP_
   - Extract the zip file so that the files are at the root of your new folder.
     - This means that you would have `D:\Factorio Server\start-server.ps`

## Getting the software

You "can" run the server using the installed steam version, but this will clash with you playing the game.

The easiest way to run a server is to download a new copy off the game.

1. Go to https://www.factorio.com/download
2. Download the zip version for windows.
3. Extract the zip files into the repository so that they're at the root.
   - This means that you will have `D:\Factorio Server\bin\x64\factorio.exe`
4. Run the game once by clicking the exe at `D:\Factorio Server\bin\x64\factorio.exe`. Let it load fully.

Congrats! Your software is ready to run the server! Let's get your mods ready.

## Setting up the mods

Factorio doesn't allow sharing modlists easily, but youy can "sync-up" to a save file. That's what we'll do to get your mods ready.

1. Boot Up your factorio server by clicking the exe.
2. In the game, follow the following menus
   _Single Player_ > _Load Game_ > _Factorio SE Mod Sync_ > _Load_ > _Sync Mods and load_
3. Uncheck _Load save after sync_
4. Click _Confirm_
5. Wait for downloads, Game will restart automatically when ready

Done! You now have all the mods ready to create a new map

## Creating a SE map

This is really easy. There's just a single thing to watch out for.

1. Create a new single player game.
2. In the _Map Generator_ Menu, at the top, change the settings from "Vanilla Default" to "Space Exploration Default".
3. Choose your other options.
4. Generate a map.
5. Save the game as soon as it starts.
6. Go to the saves folder and note the save name.
7. Right click and Edit `D:\Factorio Server\start-server.ps1`, write in your save file name

You're ready to play! Close the Game and get ready to run the server.

## Running the server

The script `start-server.ps1` will run thinbgs for you.

1. Right click `start-server.ps1` > Run with Power Shell
2. Go to your router settings and port-forward the server.
   - The server runs on port "34197" by default.
3. Connect to your server by runnning the game through steam.
   - Choose _Multiplayer_ > _Connect to address_ > Enter <your ip>:34197
   - For yourself, use your server laptop's LAN IP (The one you Port-Forwarded to).
   - For others, provide them your public IP by googling "my ip".
