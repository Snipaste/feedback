# Commnad Line Options

Command line options is supported since v1.10.0, which can be used to call some of the functions of Snipaste.

Since 'Paste' is Snipaste's major feature, currently all options require a Snipaste instance running in background.

In other words, if Snipaste is not running in the background, all the command line options will be ignored. After Snipaste is started, start another Snipaste instance (which will exit right away) with the command line options, then the corresponding functions will be executed.

# Usage
    snipaste.exe [OPTION]

> For example：

> Set the target of a shortcut (.lnk) to `/path/to/your/Snipaste.exe --snip-full`, or just run the command from another program, Snipaste will enter fullscreen capture mode.

> Note: Combining the 'Snip Options' and 'Paste Options' are not supported for the moment.

# Snip Options

    --snip                            Start snipping
    --snip X Y WIDTH HEIGHT           Start snipping with the snipping area's top-left corner
                                      set to (X, Y) and size set to WIDTH x HEIGHT
    --snip WIDTH HEIGHT               Start snipping with the snipping area's size being
                                      WIDTH x HEIGHT and its center being the cursor position
    --snip-full                       Start snipping with the snipping area set to fullscreen
    --snip-last                       Start snipping with the snipping area being the same as
                                      the last successful snipping
    --snip-delay                      Start delayed snipping
    --snip-delay TIME                 Start snipping after TIME seconds

# Paste Options

    --paste                           Paste the clipboard content as an image window
    --paste-text TEXT                 Treat TEXT as plain text and paste it to the screen
                                      (double quote the text if it contains spaces)
    --paste-html TEXT                 Treat TEXT as HTML and paste it to the screen
                                      (double quote the text if it contains spaces)
    --paste-files FILE1 FILE2 ...     Paste image file FILE1, FILE2... to the screen
    --paste-files FOLDER1 FILE1       Paste image file FILE1, FILE2, FILE3... to the screen 
      FILE2 FOLDER2 FILE3 ...         If FILE1 is a relative path, then it it relative to
                                      FOLDER1, while FILE3 is relative to FOLDER2.
                                      A FOLDER path should end with '/' or '\'.
    --images-toggle                   Show/Hide all image windows
    --images-show                     Show all image windows
    --images-hide                     Hide al image windows
    --switch-next                     Switch to the next image group
    --switch GROUPNAME                Switch to the first group named GROUPNAME
                                      (double quote the name if it contains spaces)
    --click-through-toggle            Enable/Disable the click-through mode for image windows
    --click-through-enable            Enable the click-through mode for image windows
    --click-through-disable           Disable the click-through mode for image windows

