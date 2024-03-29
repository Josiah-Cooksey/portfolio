# Jump to project:
1. ### [Assembly Recorder](#assembly-step-recorder)
2. ### [Colour Profile Manager](#nvidia-colour-profile-manager)
3. ### [Gartic Game-Playing Bot](#discord-gartic-game-player)
4. ### [World Painter Tile Group Saver](#world-painter---tile-group-saver)
5. ### [Automatic Notification Confirmer](#automatic-notification-confirmer-for-the-brave-browser)

___
___
___
___
# Assembly Step Recorder
[-> The Code <-](https://github.com/Josiah-Cooksey/assembly-recorder)

Allows the end-user to record step-by step processes for assembling (or disassembling!) things using a webcam.
- *November 2022*

![webcam main window overview](https://github.com/Josiah-Cooksey/portfolio/assets/108890925/c2d6c033-afa2-4dd9-ba91-22e3715ebfde)

## Features:
- Video recording functionality
- Simple GUI
- Recording preview
- Image snapshots
- First and final frame previews
- Optional ability to add notes for each step
- Customisable output locations and file names using the native file explorer
- Webcam channels switching

## See it in action! Full demo run ---> 
TODO

## Setup
- pip install -r requirements.txt


## Usage
### **Webcam Channels:**
At the top of the GUI, the left and right buttons can be used to switch between webcam channels; although this is almost never necessary, it is useful for those with more than a single webcam connected to their PCs.

![webcam channel switching buttons](https://github.com/Josiah-Cooksey/portfolio/assets/108890925/a3c1da0d-bf61-4738-9bca-83309fd23dc3)

### **Image Snapshots:**
The "Capture Image" button just beneath the channel settings can be used to take a picture - all the images that you capture this way will be added to a queue of images that will be included in the same folder with the video recording when saved.

![capture image button](https://github.com/Josiah-Cooksey/portfolio/assets/108890925/d02618af-d7ac-472f-abeb-611bb882895d)

### **Input Preview:**
Below that, there is a preview of the current input of the selected webcam channel, which you can use to adjust your shot before capturing.

![webcam preview](https://github.com/Josiah-Cooksey/portfolio/assets/108890925/183fd0c8-e1c9-4b36-ba33-a55790bec290)

### **Video Recording:**
Underneath, there are three buttons, "Start", "Pause", and "Stop" recording, respectively; the function of each of these are fairly self-evident, but I will explain them in detail:
- *Start*:
    - Begins recording video input from the selected webcam; don't start until your shot is ready!
- *Pause*:
    - Temporarily stops recording and changes its text to "Resume"; when clicked again, it regains its original text and continues recording webcam input to the same buffer, allowing for more dynamic cuts in a single video.
- *Stop*:
    - Stops recording and switches to the save GUI.

![recording control buttons](https://github.com/Josiah-Cooksey/portfolio/assets/108890925/2c8101d0-776a-4a79-81be-5c7902363996)

### **Saving Input:**
You're probably itching to move on to recording the next step, but hold it right there, buckaroo - you need to save it first.
After you stop recording, the app will show a save GUI.

![save window overview](https://github.com/Josiah-Cooksey/portfolio/assets/108890925/fc6a8f31-4776-45d4-bf06-d5b6581ac9e0)

At the top, in the field labeled "Save To:", you can manually type the directory + filename with no extension to save the output, but if you're not a masochist, click the "Save Data" button to do it in the native file browser.

![save location fields](https://github.com/Josiah-Cooksey/portfolio/assets/108890925/8a62b313-d136-4907-8b0d-c8e898a5eeba)

Next, you can optionally add notes to be saved in a text file alongside the video and images, but if you already have explanations in the video, there's no need.

![note input field](https://github.com/Josiah-Cooksey/portfolio/assets/108890925/986b4e82-4d4c-4681-a99d-3c50789a1d09)

Finally, there are first and final frame previews for a definite confirmation that you captured what you wanted:

![first and last frame previews](https://github.com/Josiah-Cooksey/portfolio/assets/108890925/ed34e29f-7f5e-46f3-90d2-bb50d1260b53)

You can now save the output.

![submit save button](https://github.com/Josiah-Cooksey/portfolio/assets/108890925/22f04b9e-8cb5-42f8-86ac-7d190841d2b1)

However, if you decide that you would like to discard everything and try again, just close and restart the program.


___
___
# Nvidia Colour Profile Manager
[-> The Code <-](https://github.com/Josiah-Cooksey/nvidia-colour-profile-manager)

A tool to quickly switch between several pre-set colour profiles for the Nvidia Control Panel.
- *December 2021*

![sliders adjusting](https://github.com/Josiah-Cooksey/portfolio/assets/108890925/f51ccf67-3afb-49de-a24e-d96c4c55973b)

## Features:
- Convenient hotkeys
- Easy setup
- Simple functionality
- Quick operation
- Low memory usage

## See it in action! Full demo run ---> 
TODO

## Setup
- Requires [AutoHotKey](https://www.autohotkey.com/) installed.
- The Nvidia Control Panel must be open in the "Display" > "Adjust desktop colour settings" tab. (it is not required to be in the foreground, though)

## Usage
### **Startup:**
Double-click the .ahk file to run the script.

### **Hotkeys:**
- F2
    - Resets the colour profile to the default settings.
- F3
    - High gamma, low contrast profile.
- F2
    - High gamma, low contrast, increased brightness profile.

___
___
# Discord Gartic-Game Player
- ### *September 2022*

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
- ### *April 2022*

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
- ### *September 2022*
## Description
Constantly checks several pixels on the screen until all of them match the set colours; when a match occurs, the script clicks on the confirmation button of the dialogue, waiting a second after that so that the notification has time to disappear.

## See it in action!
## Full demo run ---> https://youtu.be/IvkdQABZx0A
### (simulated)
![brave browser notification clicker demo preview](https://user-images.githubusercontent.com/108890925/18901 4810-6bf6ca01-dc70-4c91-91db-31e819e525aa.gif)


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
