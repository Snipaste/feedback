# FAQ

1. Snipaste cannot start / crashes / is not responding / settings are not saved ……

  Please refer to [troubleshooting](https://docs.snipaste.com/#/troubleshooting).

1. Mac version / Linux version / scrolling capture / GIF recording ……

  The progresses are updated [here](https://github.com/liulex/Snipaste-Feedback/issues/282).

1. Does Snipaste have to stay in the background? Can it be run only when I need to take a screenshot and exit automatically afterwards?

  Sorry, Snipaste has to stay in background, because it is indeed a 'paste' tool, which requires it to keep running.

  You may use it just for snipping, but you cannot demand it to be a pure snipping tool.

1. What does 'paste' mean in Snipaste? It does not seem like the usual paste.

   The general 'paste' means grab content from the clipboard and present it in another way. The way the content is presented should depend on the application.

   For an text editor, paste means to insert the content to the editor.

   In Snipaste, however, paste means to (try to) convert the content into an image and make it an topmost floating window. This functionality has great potential to help you work more efficiently, after you get familiar with it.

1. There are too many options and I don't know what each means.

  For most users, for the first time you start Snipaste, you may want to enable the "Run on system boot" option, and change the global hotkeys to your favorites. Leave all other options unchanged.

  Only when you find anything inconvenient, you need to check if there are any options that suit you. Almost every option shows its detailed explanation when you hover over it. If you cannot understand a certain option, you probably do not need it. Just use its default value.

1. To start annotating on an image window, do I have to choose from its context menu? It looks like very inconvenient.

  You can also press <kbd>Space</kbd> to start annotating.

1. Can I adjust the translucency of individual image window?

  Sure. Use <kbd>Ctrl</kbd> + <kbd>Mouse scroll</kbd>.

1. The tray icon looks like broken! Is it a bug?

  ![snipaste_clickthough](https://cloud.githubusercontent.com/assets/2010459/22327737/aaaa2fa2-e3f3-11e6-87eb-791d913d1f4f.png) This icon means you have enabled the click-through mode, i.e. all image windows will be unclickable by the mouse.

  The default hotkey is <kbd>F4</kbd>. Press it again to turn off the click-through mode.

  For example, you can use this feature to start copying a painting, by making the image window semi-transparent first, then enabling click-through.

1. All the image windows cannot be moved. The context menu also cannot show up.

  Same as above.

1. How to end text input?

  <kbd>Right click</kbd> (actually all annotations can be ended this way).

1. Can I adjust the translucency of the annotations?

  Sure. Press the bigger color button on the toolbar. In the color dialog, adjust the value of "Alpha channel" (0 means transparent and 255 is opaque).

  Note: The marker pen owns an independent translucency, while all other pens share an translucency.

1. How to Quick Save?

  Press <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>S</kbd> or <kbd>Shift</kbd> + the "Save" button. Then the image will be saved to the Quick Save folder.

1. What is the difference between "Close" and "Destroy" for an image window?

   Please find the explanation here: [Getting Started](https://github.com/liulex/Snipaste-Feedback/wiki/Getting-Started).

1. How to choose the quality of the output image?

  `-1` means to use auto values. `0` means small and fully compressed, while `100` means large and uncompressed.

  When you save the image as PNG, `-1` is a good choice. If you set it to `100`, the file would be too large.

  For JPG, however, `-1` could result in a blurred image. In this case, you set it to `100`, or just find a suitable value yourself (by saving the same image with different values).

  As for the image copied to the clipboard, there is no way to tweak its quality yet.

1. When is disabling the smooth scaling of an image useful?

  When the image contains scaled text. 

  For example, snip a text image on a normal screen and paste it as an image window on a HiDPI screen. Normally, you would need to scale the image to 200%, but the text is likely to be blurred. By disabling smooth scaling, the text will be sharp and clear again.

1. How to close an image group?

  Open the tray menu and find the name of the image group and right click on it.

  ![snipaste_close_group](https://cloud.githubusercontent.com/assets/2010459/22327735/aa575ff2-e3f3-11e6-9736-305c9afa3133.png)

1. Can I drag the image window beyond the top border of the screen?

  Sure, with the following system setting:
  
 * `System Properties` - `Advanced` - `Performance settings` - `Visual effects` - Check `Show window contents while window dragging` - `OK`

    ![](https://cloud.githubusercontent.com/assets/2010459/20704971/25d64640-b65c-11e6-9287-b42309145359.png)
