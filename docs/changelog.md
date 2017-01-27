# Changelog

## v1.11.3
> 2017.01.27

### New:
* [FAQ](https://www.snipaste.com/faq.html)
* Vietnamese translation (thanks to **evildeepblue**)

### Fixed:
* Rendering error when "Auto detect widnows" is disabled [#317](https://github.com/liulex/Snipaste-Feedback/issues/317)
* Some minor bugs

## v1.11.2
> 2017.01.17

### Fixed:
* Sometimes the updater dialog does not appear when an update is available [#298](https://github.com/liulex/Snipaste-Feedback/issues/298)

## v1.11.1
> 2017.01.15

### New:
* Option: Max number of history snipping areas
* Option: Loop through history snipping areas
* Portuguese (Portugal) translation (thanks to **Luis Neves**)

### Fixed:
* Possible restart failure after version update, when startup as admin (thanks to **Fubuki**)
* Short-time interface freeze when checking for update for the first time since launched
* Text of some widgets in the Preferences Dialog is not updated when switching languages
* Problems on the image borders after mirroring the image [#248](https://github.com/liulex/Snipaste-Feedback/issues/248)

### Improved:
* Faster response for the first snipping since launched
* Instant response for moving the image window by holding the mouse left button and pressing <kbd>W</kbd> <kbd>A</kbd> <kbd>S</kbd> <kbd>D</kbd> [#315](https://github.com/liulex/Snipaste-Feedback/issues/315)
  * Note: this operation has problems on Windows XP
* Translated the color dialog, font dialog, etc.
* Improvements to many details :)

## v1.11.0
> 2017.01.01

### New:
* Remember more than one snipped area [#249](https://github.com/liulex/Snipaste-Feedback/issues/249)
  * Switch between them by pressing multiple times of <kbd>R</kbd> or <kbd>Shift</kbd> + <kbd>R</kbd>
  * The number is the same as the max number of history snipping records
* Add an alternative update feed source
* Add a "Recheck" button in the updater dialog
* [Command Line Options](https://docs.snipaste.com/command-line-options): `--snip-whiteboard` whiteboard mode
* Option: Customize the action of <kbd>Enter</kbd> for snipping
* Option: Zoom at mouse cursor [#277](https://github.com/liulex/Snipaste-Feedback/issues/277)
* Option: 'Reset image' also works in thumbnail mode [#280](https://github.com/liulex/Snipaste-Feedback/issues/280)
* Option: Preserve the original image window for drag-and-drop
* Dutch translation (thanks to **Stephan Paternotte**)

### Fixed:
* Detecting elements in Nsight causes its crash [#290](https://github.com/liulex/Snipaste-Feedback/issues/290)
* Under certain conditions, the <kbd>Win</kbd> key is not unhooked after snipping is finished [#272](https://github.com/liulex/Snipaste-Feedback/issues/272)
* The first press of <kbd>Tab</kbd> has no effect
* Some logical errors when checking for updates

### Improved:
* Now you can toggle the toolbar by <kbd>Space</kbd> even in edit mode
* Let the hue value for achromatic colors be 0 instead of -1
* Improvements to many details :)

## v1.10.5
> 2016.12.10

### New:
* Add HSV and HSI to the color card

### Fixed:
* Text copied from Chrome has rendering problems after pasted to the text edit [#257](https://github.com/liulex/Snipaste-Feedback/issues/257)
* Text copied from Android Studio loses its format after converted to an image [#266](https://github.com/liulex/Snipaste-Feedback/issues/266)
* Cannot capture topmost windows if Snipaste is started under some special conditions [#269](https://github.com/liulex/Snipaste-Feedback/issues/269)
* Sometimes the z-orders of image windows are not correctly restored

### Improved:
* If "Start on system boot" is checked and the startup shortcut is found lost when Snipaste is starting, try to regenerate one

## v1.10.4
> 2016.12.05

### Fixed:
* Adding/Removing screens is not detected under some conditions [#233](https://github.com/liulex/Snipaste-Feedback/issues/233)
* Drag-and-drop operation for GIF files [#260](https://github.com/liulex/Snipaste-Feedback/issues/260)
* Missing magnifier under some conditions
* Infinite update notification under some conditions

## v1.10.3
> 2016.12.01

### New:
* Check out our brand new [documentation site](https://docs.snipaste.com)!
  * Generated using <a href="https://docsify.js.org" target="_blank">docsify</a>
  
### Fixed:
* When the system setting "Show indow contents while dragging" is not enabled, the image windows cannot be moved
* Cannot copy the text from a pasted file path
* Hold <kbd>Shift</kbd> and drag the anchor of line shapes has no shifted effect
* [#253](https://github.com/liulex/Snipaste-Feedback/issues/253)

### Improved:
* Cancel the moving operation for pencil / mosaic / eraser, to avoid unintended moving for continuous drawing

## v1.10.2
> 2016.11.28

### New:
* Easy text re-edit
* Allow to move shapes as a whole, including line strip / pencil / mosaic / eraser
* Hold <kbd>Mouse left button</kbd> + <kbd>W</kbd> <kbd>A</kbd> <kbd>S</kbd> <kbd>D</kbd> to move the image window by pixel [#211](https://github.com/liulex/Snipaste-Feedback/issues/211)
* [Command Line Options](https://docs.snipaste.com/command-line-options): `--paste-files` accepts directories now
* [Advanced Configs](https://docs.snipaste.com/advanced-configs): snip/exclude_from_detection
* [Advanced Configs](https://docs.snipaste.com/advanced-configs): snip/crashes

### Fixed:
* After startup on system boot, a manual update check will cause the Preferences Dialog unresponsive [#242](https://github.com/liulex/Snipaste-Feedback/issues/242)
* If elevated, Snipaste cannot respond to command line options [#240](https://github.com/liulex/Snipaste-Feedback/issues/240)
* Window detection is not working if snipping is started under some special condition [#123](https://github.com/liulex/Snipaste-Feedback/issues/123)

### Improved:
* Various details improvement

## v1.10.1
> 2016.11.22

### Fixed:
* Application crashes once started (for a few users)
* Incorrect display when replaying snipping history
* The "Update Success" notification doesn't pop up after online update

## v1.10.0
> 2016.11.22

### New:
* Support [Command Line Options](https://docs.snipaste.com/command-line-options)
* When snipping, allow to adjust the snipping area when in edit mode [#211](https://github.com/liulex/Snipaste-Feedback/issues/211)
* All edit shapes now support <kbd>Shift</kbd> toggling
* "Line strip" now has a "Line" mode: click and hold <kbd>Mouse left button</kbd>, then move the mouse to draw a single line
* "Help" menu in the tray menu
* Press <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>C</kbd> on the image window to directly copy the plain text (if this image is converted from text)
* Click the balloon after a Quick Save to reveal the file in Windows Explorer [#220](https://github.com/liulex/Snipaste-Feedback/issues/220)
* "Show in folder" action in the context menu of image window [#223](https://github.com/liulex/Snipaste-Feedback/issues/223)
* Option: Startup as admin on system boot
  * So that you can use hotkeys even if the active window is run as admin
* Option: Proxy server settings
* Option: Delay time for update checking after startup
* Option: Check for updates every a few hours
* Option: Include beta builds when checking for updates
* Option: Disable text-to-image conversion

### Improved:
* **Greatly improved performance when snipping**
* Redraw all icons and use no icon fonts
* The shortcut for "Pin to screen" when snipping has been changed to <kbd>Ctrl</kbd> + <kbd>T</kbd> (previously <kbd>Ctrl</kbd> + <kbd>W</kbd>)
* Refine the painting of the magnifier
* Better adjustment strategy for the position of the toolbar when snipping
* Better adjustment strategy for the position of the resolution label when snipping

### Fixed:
* In the enhanced tray menu, "Show/Hide all images" performs an incorrect action [#202](https://github.com/liulex/Snipaste-Feedback/issues/202)
* Fast switching between image groups may cause no new images can be pasted [#199](https://github.com/liulex/Snipaste-Feedback/issues/199)
* Many minor bugs

## v1.9.2
> 2016.10.31

### Fixed:

* After transferring an image to another group, the images in that group are lost (a bug of v1.9.0 and v1.9.1)
* After transferring an image to another group created by an much earlier version of Snipaste, the application crashes
  * **After this update, please switch into each image group to ensure history records are upgraded**
* Possible incorrect image counts after an image is transferred

### Improved:

* Make the newly transferred image on top of other images

## v1.9.1
> 2016.10.27

### Fixed:

* User configs of 'Image Operations' are lost after upgrade

### Improved:

* Apply the file name pattern to the file save dialog (except for the suffix, which will be the same as your last saved image)

## v1.9.0
> 2016.10.27

### New:

* Allow to customize the pattern of image file names [#98](https://github.com/liulex/Snipaste-Feedback/issues/98)
* Delayed snip [#181](https://github.com/liulex/Snipaste-Feedback/issues/181)
* When the magnifier is visible, press <kbd>Shift</kbd> to toggle the color formats [#187](https://github.com/liulex/Snipaste-Feedback/issues/187)
* When dragging to resize the snipping area, hold <kbd>Space</kbd> to move the area [#192](https://github.com/liulex/Snipaste-Feedback/issues/192)
* Brazilian Portuguese translation（thanks to **Igor Rückert**）
* Polish translation（thanks to **Wirus deleted my username**）

### Fixed:

* Another bug that causes application crash when switching image groups in a row
* In the Preferences Dialog, the text-to-image preview is not updated when the related settings are changed
* Possible incorrect color is applied after a "redo"
* Several logic errors

### Improved:

* Guarantee the atomicity of history record files (even for application crash or pow failure)
* Greatly improved efficiency when switching image groups in a row
* Disable <kbd>Shift </kbd>+ <kbd>Left button</kbd> for customizable image operations (due to conflict with image window attaching)
* Show file path in the balloon when image is saved via Quick Save
* Remember the position and current tab for Preferences Dialog
* Show animation when the size of Preferences Dialog is changed

## v1.8.8
> 2016.10.16

### Fixed:

* Incorrect processing for Quick Save path (the upper directory was used instead, affecting 1.8.6 and 1.8.7)
* The previous arrow/text scaling is not restored after Snipaste is restarted
* When the magnifier shows up, the first frame shows the old content

## v1.8.7
> 2016.10.15

### Fixed:

* Fail to play the sound effect

## v1.8.6
> 2016.10.15

### New:

* Option: Play a sound effect after snipping
* When editing, press Alt+C to pick the screen color into the painting pen

### Improved:

* Auto switch to the corrseponding edit mode after "Redo", to make it easier for re-edit
* Support relative path for Quick Save directory

## v1.8.5
> 2016.10.13

### New:

* Support global hotkeys containing <kbd>PrtSc</kbd>

### Improved:

* Change the name of "Meta" key to "Win"

## v1.8.4
> 2016.10.12

### New:

* Option: Customize the mouse operation for image windows
 * Note: 'Close image' has been reset to 'Double click' and 'Toggle thumbnail mode' is now 'Win + Left click'
 * Change them yourself if you don't like the defaults
* Option: Customize the output image quality
* The Internal Hotkeys Dialog is updated and added with a 'Copy' button
* Press Ctrl+Shift+P on an image window to open the Preferences Dialog
* [Advanced Configs](https://docs.snipaste.com/advanced-configs): General/high_process_priority
* [Advanced Configs](https://docs.snipaste.com/advanced-configs): snip/do_not_omit_synthesized_c
* Japanese translation (Thanks to **鳳凰院カミ**)

### Fixed:

* Crash when switching image groups in a row
* The thumbnail images cannot flash their borders
* When the default opacity for image windows is less than 100, image duplication check does not work properly

### Improved:

* No more omit all synthesized keys when snipping (so that synthesized keys by ahk etc. still work)
* Even when "Auto detect UI elements" is not checked, you can press 'Tab' to start element detection
* Images with small width/height can be easily moved now

## v1.8.3
> 2016.10.02

### Fixed:

* Wrong snip history folder is used (a bug of v1.8.2)
* Snipaste mistakenly exits due to double click on the tray icon

### Improved:

* The theme color will now be applied to the shadow of the active image window

## v1.8.2
> 2016.09.30

### New:

* [Advanced Configs](https://docs.snipaste.com/advanced-configs): General/history_dir 

### Fixed:

* Snipaste fails to restart after auto update, for some users
* After closing a group from the tray menu, the menu does not hide itself

### Improved:

* Remove "Restart" from enhanced tray mene
* Check and remove unused group folders in the history directory on startup

## v1.8.1
> 2016.09.29

### Fixed:

* Some user-modified settings are not correctly applied after restar
* (XP) Fail to create startup link for non-English system

### Improved:

* Show notification if config.ini is not writable

## v1.8
> 2016.09.28

### New:

* Thumbnail mode for the image windows (double click on it)
* Option: Thumbnail size
* "Restore Defaults" buttons in Preferences Dialog
* The alpha channel can be applied to marker pen now

### Fixed:

* Window detection for maximized windows and fullscreen windows
* Again, window detection problems on HiDPI screens
* Dual screen (when primary screen is at bottom and screen borders are not aligned) problems of snipping
* Shape controllers are unexpectedly drawn when saving to an image
* Rectangle/Ellipse/LineStrip/Pencil drawing when using semi-transparent colors

### Improved:

* The alpha value is now saved for small colors buttons too

## v1.7.3
> 2016.09.19

### Fixed:
* Taskbar area is not included if the detected window is fullscreen
* (XP) kernel32.dll error
* (XP) Unable to set global hotkeys

### Improved:
* Remember the arrow size for next edit
* Restore the arrow sizes and text sizes after Snipaste is restarted
* Make Quick Save folder path editable
* Ignore transparent window from window detection
* (XP) Remove window animation for the first snipping after started

## v1.7.2
> 2016.09.17

### Fixed:
* Task bar icon for the snipping windows is noticable
* Snipping area is set automatically on entering snipping (under some conditions)
* Cursor shape is not updated as it should when snipping
* Image window attaching is not working (by holding Shift key, then move the image window to align to another window and then release the mouse button)

## v1.7.1
> 2016.09.15

### Fixed:
* Some message boxes are obscured by the option dialog
* Lack of msvcr120.dll for some Win 7 x64 users

### Improved:
* Remove the delay for directly pasting the screenshot to the screen

## v1.7
> 2016.09.15

### New:

* Auto updater
* Press <kbd>Tab</kbd> to toggle between picking a window/ picking an UI element when snipping
* Press <kbd>3</kbd> <kbd>4</kbd> to flip the image on an image window
* Option: General: Enhanced tray menu
* Option: Snip: Capture the cursor (You can also press <kbd>`</kbd> to toggle when you are snipping)
* Option: Snip: Pin to screen by clicking the mid-button [#63](https://github.com/liulex/Snipaste-Feedback/issues/63)
* Option: Snip & Paste: Copy as Windows Bitmap [#20](https://github.com/liulex/Snipaste-Feedback/issues/20)
  * If you cannot paste the image into some apps (like Skype and UWP Wechat), check it. But in the meantime the alpha channel is lost
* Option: Snip: Border width
* Option: Snip: Show mask in the magnifier
* Option: Snip: Show border in the magnifier
* Option: Snip: Auto show cross lines
* Option: Snip: Quit snipping if any other window is activated
* Option: Paste: Default opacity [#96](https://github.com/liulex/Snipaste-Feedback/issues/96)
* Option: Paste: Mnemonics on the context menu
* Option: Paste: Flash after switching to another group

### Fixed:

* The conflict with some translation programs (Tested on Bing Dictionary, Youdao Dictionary and QTranslate) [#64](https://github.com/liulex/Snipaste-Feedback/issues/64)
* Snipaste becomes unresponsive when detecting some UI elements [#95](https://github.com/liulex/Snipaste-Feedback/issues/95) [#116](https://github.com/liulex/Snipaste-Feedback/issues/116)
* UI element detection is not working for some users [#61](https://github.com/liulex/Snipaste-Feedback/issues/61)
* Failed to obtain keyboard focus on entering snipping, under certain conditions [#114](https://github.com/liulex/Snipaste-Feedback/issues/114)
* Possible crashes when pasting the screenshot to the screen directly [#119](https://github.com/liulex/Snipaste-Feedback/issues/119)
* Slowing down the machine when trying to paste a huge file as an image window [#102](https://github.com/liulex/Snipaste-Feedback/issues/102)
* Unable to snip with fingers on a touch screen
* <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>S</kbd> sometimes has no effect [#42](https://github.com/liulex/Snipaste-Feedback/issues/42)
* Press <kbd>Shift</kbd> when drawing an rectangle or ellipse, the icons on the paint bar are not consistent [#53](https://github.com/liulex/Snipaste-Feedback/issues/53)
* Blurry image on some HiDPI screens with some settings [#74](https://github.com/liulex/Snipaste-Feedback/issues/74)
* Incorrect scaling on image windows for some HiDPI screens with some settings [#74](https://github.com/liulex/Snipaste-Feedback/issues/74)
* Incorrect rendering for semi-transparent text
* Incorrect rendering for eraser and mosaic on semi-transparent background
* Duplicated image windows under certain conditions
* The image window is not activated (with the corresponding option checked) when it is pasted directly from snipping
* The borders are incorrectly taken into the screenshot for some users

### Improved:

* No more rotation when dragging the text box, unless you hold <kbd>Ctrl</kbd>
* The last postfix is remembered and applied when you save an image from a file save dialog
* Fix the arrow size instead of adjusting according to its length, but the user can change its size by <kbd>Mouse scrolling</kbd> or pressing <kbd>1</kbd> <kbd>2</kbd>
* Merge the Quick Save Folder for Snip and Paste
* Now you can click on the group name in the tray menu to switch to that group. To rename or close a group, right click on the group name.
* Add a rainbow corner on the bigger color button to indicate it can be used to pick a color (By Fubuki)
* "Hide" a single image is now called "Close", in order to distinguish with "Hide all images"
* In case you get stuck in snipping, now you can click on the tray icon to force exit Snipaste when you are snipping
* When you text box is empty, double click on it will also trigger a screenshot
* The magnifier will auto adjust its size according to the screen DPI

## v1.6
> 2016.08.10

### New:

* Option: Copy the Hex value without '#'
* A hollow arrow style

### Fixed:

* Incorrect window size detection for Windows standard style windows
* Incorrect image conversion from HTML text with some specified format
* Incorrect color button size for a 150% DPI screen
* Obvious lagging for the magnifier on the image window

### Improved:

* Some of the icons have been updated (Thanks to **shejimiao**)

## v1.5
> 2016.08.08

### New:

* Quick save folders for snipping and pasting (Press <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>S</kbd>, or <kbd>Shift</kbd> + `"Save" button`)* New: When detecting the UI elements in snipping, press <kbd>Space</kbd> to use the current area
* Cross lines at the cursor position (nedd to press <kbd>Alt</kbd>)
* Press <kbd>Ctrl</kbd> + <kbd>A</kbd> when snipping, the snipping area will be set to fullscreen
* "Internal hotkeys" window (under "Hotkeys" tab in the option dialog)
* Send the screenshot/image to the printer (no buttons, only via <kbd>Ctrl</kbd> + <kbd>P</kbd>)
* Option: Show usage tips on the magnifier (enbaled by default)
* Option: Use Hex value for color picker
* German translation (Thanks to **Samuel Marcius**)
* Greek translation (Thanks to **geogeo.gr**)
* Swedish translation (Thanks to **Åke Engelbrektson**)

### Fixed:

* Some gloabl shortcut has no effect, though it is marked as success
    * Except for <kbd>PrtScr</kbd> and hotkeys occupied by the system or other programs, most shorcuts should be ok now.
* The default global hotkeys may still be possessed after the user changes the keys
* When in dual-screen (the primary on the right), the eraser/mosaic/blur effects are not painted correctly
* Snipaste may crash when detecting UI elements
* The color dialogs are not translated
* Press <kbd>Alt</kbd> and move the cursor acroos several image windows, some magnifiers do not hide themselves correctly
* The option "Use snipping position" does not affect the `"Paste to screen" button` (or <kbd>Ctrl</kbd> + <kbd>W</kbd>)

### Improved:

* When the color value is copied from an image window, flash the magnifier to indicate the copy is done
* The option “Ignore `Win` when snipping” will only affect the single press of <kbd>Win</kbd>. Combined keys with <kbd>Win</kbd> (e.g. <kbd>Win</kbd> + <kbd>Space</kbd>) will not be affected
* You can now choose different image formats from the save file dialog
* Add a border (of your theme color) for the hotkey editor
* Add an obvious hint of how to delete the current hotkey
* Change the default global hotkeys (e.g. 'Paste' is now <kbd>F3</kbd> instead of <kbd>F2</kbd>)
    * It will only affect new users. Existing users will not lose your own settings.
* User <kbd>↑</kbd> <kbd>←</kbd> <kbd>↓</kbd> <kbd>→</kbd> (instead of <kbd>W</kbd> <kbd>A</kbd> <kbd>S</kbd> <kbd>D</kbd>) to move the image window, in order to be consistent with the behavior of snipping area control
* Use the same color board as mspaint's

## v1.4
> 2016.08.01

### New:

* XP version
* Use <kbd>Backspace</kbd> to delete the current hotkey
* Use <kbd>Esc</kbd> to hide the image window, and <kbd>Shift</kbd> + <kbd>Esc</kbd> to destroy it
* Option: Hide all images if you paste when any image window is flashing

### Fixed:
* Negative numbers appear when using <kbd>Shift</kbd> + <kbd>↑</kbd> <kbd>←</kbd> <kbd>↓</kbd> <kbd>→</kbd> to shrink the snipping area

## v1.3
> 2016.07.29

### New:

* Press <kbd>Shift</kbd> + <kbd>↑</kbd> <kbd>←</kbd> <kbd>↓</kbd> <kbd>→</kbd> to shrink the snipping area
* Traditional Chinese translation (Thanks to **zhtw**)

### Fixed:

* When in dual-screen (the primary on the right), press <kbd>Alt</kbd> and the dashed lines are not drawn correctly
* When in dual-screen, the detected area for a fullscreen program outbounds its screen
* Press <kbd>Alt</kbd> and double-click the image window, the window is hidden but the magnifier is still visible

## v1.2
> 2016.07.29

### Fixed:
* Cannot snip in dual-screen (the primary on the right)
* The tray icon tooltip is not updated after the interface language is changed

## v1.0
> 2016.07.28

* First public release