This repository serves as a collection of assets from inside the game ARC Raiders.

## $100 Item Image Bounty

There is a **$100 bounty** for the first person to get the rest of all item images.

## Repository Note

The original creator of this repository, `astroval0`, chose to archive it. This version was reopened so the asset collection can keep being updated and remain useful to the community.

Personal note from OskarSuu: I think it is weird behavior to close something like this when it matters so much to other people.

The `.blend` files have packed textures and are made for Blender 5.0 and above. There may be issues opening them in older Blender versions.

The goal is to make ARC Raiders assets easy to access and use. This repository will not include unreleased assets.

Suggestions and pull requests are welcome.

# How To Rip ARC Raiders Assets With Ninja Ripper

> Ripping assets from a live game can come with account or anti-cheat risk. Use this method at your own risk.

## Requirements

- Ninja Ripper. This guide was written around version 2.12.
- The Ninja Ripper Blender import plugin.
- Steam fully closed before starting.

## Step 1: Close Steam

Fully exit Steam before starting Ninja Ripper.

Right-click Steam in your system tray and select **Exit**.

## Step 2: Launch Steam Through Ninja Ripper

Open Ninja Ripper and use it to launch `steam.exe`.

This makes Steam, and then ARC Raiders, run through Ninja Ripper.

## Step 3: Add The ARC Raiders Launch Argument

In Steam, open the ARC Raiders game properties and add this launch argument:

```text
-nothreadtimeout
```

This helps prevent the game from timing out while Ninja Ripper pauses or hangs during capture.

## Step 4: Launch ARC Raiders

Launch ARC Raiders normally through Steam.

Once the game is running, go to the area or menu that contains the asset you want to capture.

## Step 5: Capture The Assets

While in game, press your Ninja Ripper rip hotkey.

You can adjust Ninja Ripper settings and capture again as needed.

## Step 6: Find The Rip Output

After ripping, check the `PioneerGame.exe` folder inside your Ninja Ripper output directory.

This folder should contain captured models and textures. UI icons and images that were visible on screen during the rip may appear here too.

## Step 7: Import Into Blender

Use the Ninja Ripper Blender plugin to import the captured files.

For ARC Raiders raid captures, use the same FOV as your in-game setting. The maximum in-game FOV is 80.

Set the import resolution to match your game resolution. For example, if you captured in fullscreen at `1920x1080`, import using `1920x1080`.

Lobby captures may use an FOV around 35, but this can vary.

## Notes

Currently, no 3D models are rigged.

![Arc Raiders Queen](queen.png)

Queen model note: the current textures use a basic diffuse and normal setup instead of the full in-game shader setup, so the model may look different from how it appears in game.
