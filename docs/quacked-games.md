# Quacked games

## Install quacked games

There is two methods for installing quacked games: using Steam or using Lutris. I prefer the one using Steam because it is way easier.

1. Switch to `Desktop` mode
2. Download the repack installer of the game
3. Unzip it if needed
4. Do one of the following methods (step 5 or 6)
5. **Steam method**
    1. Open Steam
    2. Click on `Add a game` in the bottom left corner
    3. Click on `Add a non-Steam game`
    4. Click on `Browse`
    5. Select the installer's executable
    6. Click on `Add selected programs`
    7. Right click on the game in the library
    8. Click on `Properties`
    9. Click on `Compatibility`
    10. Check `Force the use of a specific Steam Play compatibility tool`
    11. Select `Proton Experimental`
    12. Click on `Close`
    13. Run the app
6. **Lutris method**
    1. Create a folder as `~/prefixes/<game_slug>`. It will be the prefix folder containing the pseudo windows file tree.
    2. Open Lutris
    3. Click on `Add Game
    4. Click on `Install a Windows game from an executable`
    5. Put the game's name
    6. Click on `Install`
    7. Click on `Install` again
    8. Put the folder path that you created in the first step
    9. Click on `Create a Steam shortcut`
    10. Click on `Continue`
    11. Browser to the installer's executable
    12. Click on `Install
7. Then follow the installer's instructions. 
    - You should install the game in the `Z:` drive (e.g: `Z:\home\deck\Games\<your_game_name>`)
    - If using *fitgirl-repacks* for example, make sure to uncheck all the extra actions starting with "Update" after the installation.
8. Tada 🎉

## Play quacked games

Just launch them from Steam if you've added them as shortcuts, or from Lutris directly.

## Access save files

If installed following the Steam method, save files of non steam Games are located in `~/.local/share/Steam/steamapps/compatdata/<id>/pfx/drive_c/<regular_windows_save_location_path>`.

Either, they'll be located in the prefix folder you created if you followed the Lutris method.

## Helpers

### Shortix

[Shortix](https://github.com/Jannomag/shortix) is a script that creates humand readable symlinks for Proton/Wine game prefixes of Steam.