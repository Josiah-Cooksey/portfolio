# Jump to project:
1. ### [Gartic Game-Playing Bot](#discord-gartic-game-player)
2. ### [World Painter Tile Group Saver](#world-painter---tile-group-saver)
3. ### [Automatic Notification Confirmer](#automatic-notification-confirmer-for-the-brave-browser)

___
___
# Discord Gartic-Game Player

## Description
Detects embedded images sent by the gartic bot, screenshots them, hashes the screenshot, and checks if that hash corresponds to an answer in its database.

## Features
- Automatic Answer-Logging Mode
- Automatic Playing Mode
- Manual Answer-Saving Button
- A screen showing the current image that the program has captured
- Audio cues for ease of use

## See it in action!
## Full demo run ---> https://youtu.be/WjEUmETBV7o
![answer](https://user-images.githubusercontent.com/108890925/195712379-630ebe65-c6be-478e-91f5-92bed9e0a7fa.gif)


## Prerequisites
- [Java 15]()

## Usage
- The "Static" button can be toggled between its current state and "Scrolling", in which mode it automatically scrolls up in a Discord channel, searching for answers to Gartic prompts and logging them along with the hash of the corresponding image.
    Because the mouse is automatically moved by the program during the "Scrolling" stage, you can also press F2 to switch back to the "Static" mode.
![scroll](https://user-images.githubusercontent.com/108890925/195712490-d4799bcc-45ee-49d7-8357-99766099e38f.gif)

- The "Save" button allows you to manually save the image's hash with whatever custom answer input you desire - useful for logging answers while playing the game yourself.
![save](https://user-images.githubusercontent.com/108890925/195712505-b5189fb1-aa73-4ab7-bdbe-5369991c5115.gif)

- The "Silent" button can be toggled between its current state and "Answering", in which mode it will automatically type out the answer to the prompt if known; there is a bell-ringing sound when this is the case so that the user knows that nothing must be manually typed.
![answer](https://user-images.githubusercontent.com/108890925/195712516-836ebc7d-d558-4ea2-b7eb-73388c4c43a4.gif)
___
___
# World Painter - Tile Group Saver

## Description
Loops over the tiles of an open minecraft map, saving sections of 3x3 (not hard-set - customisable) tiles with varying names in the same folder.

## See it in action!
## Full demo run ---> https://youtu.be/2DZo5fS-Qxk
![demo](https://user-images.githubusercontent.com/108890925/187715685-14bdbd1b-2734-4c83-b5d3-d84e0147aadd.gif)

## Prerequisites
- [AutoHotKey](https://autohotkey.com)
(after installing, you can just double click any `.ahk` file to run it)

## Setup
- Shift F1 - opens a dialogue box for you to input the dimensions (in tiles) that the map is.
![setup step 1 - dimensions and section names](https://user-images.githubusercontent.com/108890925/187714490-7d8a4566-fbd1-4a42-834f-90d019b26e46.gif)
- Shift F2 - logs the coordinates of the upper left corner of the tilemap. (place the centre pointer on that tile beforehand)
- Shift F3 - logs the coordinates of the lower right corner of the tilemap. (place the centre pointer on that tile beforehand)
![setup steps 2 and 3 - mark corners](https://user-images.githubusercontent.com/108890925/187714568-a9f11440-55cd-4b4d-b8b7-90564287aaa3.gif)

## Usage
- Shift F4 - starts the automated export!

- Windows Key P  - pauses the program; you can resume operation by pressing the key combination again.

Hotkeys can be edited to your liking but I've set them so to reduce interference with built-in hotkeys and other programs.

___
___
# Automatic Notification Confirmer for the Brave Browser

## Description
Constantly checks several pixels on the screen until all of them match the set colours; when a match occurs, the script clicks on the confirmation button of the dialogue, waiting a second after that so that the notification has time to disappear.

## See it in action!
## Full demo run ---> https://youtu.be/IvkdQABZx0A
### (simulated)
![brave browser notification clicker demo preview](https://user-images.githubusercontent.com/108890925/189014810-6bf6ca01-dc70-4c91-91db-31e819e525aa.gif)


## Prerequisites
- [AutoHotKey](https://autohotkey.com)
(after installing, you can just double click any `.ahk` file to run it)

## Setup
- Double click the file to run.

## Usage
- Right click to pause or resume execution.
- Shift F2 - Exits the program completely.
- Shift F3 - Reloads the script, effectively closing then restarting itself.

___
___
