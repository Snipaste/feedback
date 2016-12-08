# Getting Started

Snipaste consists of three major functionalities: `Snip`, `Image Edit` and `Paste`.

## Snip

#### How to start snipping
* By hotkey (default <kbd>F1</kbd>)
* <kbd>Left click</kbd> on the tray icon

#### What is a _successful snipping_
* Save to clipboard ( ![](https://www.snipaste.com/img/copy16.svg) / <kbd>Ctrl</kbd> + <kbd>C</kbd> / <kbd>Enter</kbd> / <kbd>Double click</kbd> on the snipping area)
* Save to file ( ![](https://www.snipaste.com/img/save16.svg) / <kbd>Ctrl</kbd> + <kbd>S</kbd>)
* Paste to screen ( ![](https://www.snipaste.com/img/pin16.svg) / <kbd>Ctrl</kbd> + <kbd>T</kbd>)
* Quick Save (<kbd>Shift</kbd> + ![](https://www.snipaste.com/img/save16.svg) / <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>S</kbd>)

#### When will the snipping abort
* Press <kbd>Esc</kbd> at any moment
* Click the `X` button at any moment
* Right click when you are not in edit mode
* Any window of other programs is activated at any moment
  * This behavior can be disabled in the Preferences Dialog

#### Replay your snipping history
* Press <kbd>,</kbd> or <kbd>.</kbd> after you start snipping
* Only _successful snippings_ will appear in the snipping history
* The max number of history records can be set in the option dialog

#### Move the cursor by 1 pixel
 * <kbd>W</kbd> <kbd>A</kbd> <kbd>S</kbd> <kbd>D</kbd>

#### Adjust the snipping area by a pixel
* Hold <kbd>Mouse left button</kbd> + <kbd>W</kbd> <kbd>A</kbd> <kbd>S</kbd> <kbd>D</kbd> (**Recommended!** You can move, enlarge and shrink the area in this way.）
* Move the area： <kbd>↑</kbd> <kbd>←</kbd> <kbd>↓</kbd> <kbd>→</kbd>
* Enlarge the area：<kbd>Ctrl</kbd> + <kbd>↑</kbd> <kbd>←</kbd> <kbd>↓</kbd> <kbd>→</kbd>
* Shrink the area：<kbd> Shift</kbd> + <kbd>↑</kbd> <kbd>←</kbd> <kbd>↓</kbd> <kbd>→</kbd>

#### The magnifier
* The magnifier will automatically appear when it should
* If it is not visible when you need it, hold <kbd> Alt</kbd> 

#### Pick and copy the color (in RGB/Hex)
* Press <kbd>C</kbd> when the magnifier is visible. You can then press <kbd>F3</kbd> to paste it as a color card, or press <kbd>Ctrl</kbd> + <kbd>V</kbd> to paste it into other programs
* You can press <kbd>Shift</kbd> to toggle the color format

## Image Edit
#### How to finish editing the current shape manually
* <kbd>Right click</kbd>

#### How to re-edit a finished shape
* Press `Undo` **until the shape you want to edit disappears**, then press `Redo`
* Direct re-edit will be implemented in the future

#### I would like to use my own color instead of those in the color board
* Press the bigger color button

#### How to adjust the arrow size
* <kbd>Mouse scroll</kbd>
* <kbd>1</kbd> <kbd>2</kbd>

#### How to scale the text
* Drag the corners of the text box

#### How to scale the text and also rotate it
 * Hold <kbd>Ctrl</kbd> before you drag the corners of the text box

#### How to make rotated text to be horizontal again
* Hold <kbd>Shift</kbd> before you drag the corners of the text box

## Paste
In most cases, "Paste" is to convert the content in the system clipboard into an image and make it a topmost window.

Therefore, whether an image will come out, or what will appear when you paste, depends on the content in your system clipboard.

#### How to paste
* By hotkey (default <kbd>F3</kbd>)
* <kbd>Middle click</kbd> on the tray icon
* Choose `Paste to screen` when you are snipping

#### When can I paste
* There is an image in the clipboard
* There is color information in the clipboard
 * RGB：three 0~255 integers or three 0~1 float numbers
 * HEX：a valid hex color value starting with #
* There is text in the clipboard
 * Pure text
 * HTML text
* There is a file path in the clipboard (i.e. you copied some file(s))
 * If the file is an image, the image will be pasted
   * If you paste again, the file path will be converted into an image and be pasted
 * If the file is not an image, the file path will be converted into an image and be pasted
 * Starting from v1.5, you can choose never paste file paths in the option dialog

#### Rotate the image window
* <kbd>1</kbd> <kbd>2</kbd>

#### Horizontal/Vertical flip
* <kbd>3</kbd> <kbd>4</kbd>

#### Scale the image window
* <kbd>Mouse scroll</kbd>
* <kbd>+</kbd> <kbd>-</kbd>
* Drag the border of the window

#### Set the transparency of the image window
* <kbd>Ctrl</kbd> + <kbd>Mouse scroll</kbd>
* <kbd>Ctrl</kbd> + <kbd>+</kbd> <kbd>-</kbd>

#### Make all images be mouse click-through
* By hotkey (default <kbd>F4</kbd>)
 * Notice the change in the tray icon ;-)

#### Reset the image to be 100% size and 100% opaque
* <kbd>Middle click</kbd>
 * Customizable since v1.8.4

#### Thumbnail mode
* <kbd>Win</kbd> + <kbd>Left click</kbd> on the image window
 * Customizable since v1.8.4

#### Hide an image window
* <kbd>Esc</kbd>
* <kbd>Double click</kbd>
 * Customizable since v1.8.4
* The hidden image can be recovered by another pasting, unless the max hidden number is reached
* The max hidden number for pasting can be set in the option dialog (default/recommended to be **1**）

#### Hide all image windows
* By hotkey (default <kbd>Shift</kbd> + <kbd>F3</kbd>)
* Press the hotkey again to show all image windows
* Hiding images in this way is **completely different** from the above Single-Image-Hiding, which means hiding all images will not affect the hidden image counting.

#### Destroy the image
* <kbd>Shift</kbd> + <kbd>Esc</kbd>
* Choose `Destroy` in the image window's context menu
* A destroyed image will not be recovered by another pasting
  * But it still comes out if I paste again!
    * It is because there is content in your clipboard. Snipaste just pastes it as a new image.

#### The magnifier
* Just like when you are snipping, hold <kbd>Alt</kbd> to show the magnifier

#### Pick and copy the color (in RGB/Hex)
* Just like when you are snipping, press <kbd>C</kbd> to copy the color value of the pixel
