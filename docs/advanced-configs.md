# Advanced Configs

These are settings without user interface. Please use them with caution.

## Usage

1. Close Snipaste.
1. Open config.ini with any text editor.
1. Add corresponding lines of settings under the correct group (the name in between square brackets).
  * Note: Text behind the semicolon is only comments.
1. Save and close config.ini.
1. Open Snipaste.


## [General]

    ; Set the history directory (since 1.8.2)
    ; Snipaste will not create the folder for you. Please make sure it exists, otherwise "./history" will be used
    ; Slash should be / or \\
    ; No need to use quotes if there exists spaces in the path; do not support non-English characters
    ; Examples for relative paths:
    ; abc
    ; ./abc
    ; ../abc
    ; Examples for absolute paths:
    ; D:/configs/sphistory
    ; D:\\abc def\\history

**history_dir=c:/abc**

    ; Hide the tray icon (since 1.8)
    ; Valid vaules: true, false

**hide_tray_icon=true**

    ; Run with high process priority (since v1.8.4)
    ; Windows ONLY
    ; Valid values：true, false

**high_process_priority=true**

## [snip]

    ; Do not omit sythesized key 'C' (since v1.8.4)
    ; Some of the dictionary programs sends synthesized Ctrl + C when mouse left button is released,
    ; so Snipaste needs to omit the synthesized 'C' to make snipping work properly.
    ; If this function, on the contrary, annoys you (for example, a GoldenDict user), you may set this option to true
    ; Windows ONLY
    ; Valid vaules：true, false

**do_not_omit_synthesized_c=true**

    ; Exclude the windows of specific programs from window detection (since 1.10.2)
    ; For example, when we use LICEcap for screen recording, the window of LICEcap will be detected and
    ; prevents Snipaste from detecting the window / interface elements beneath the LICEcap window.
    ; You can append 'licecap.exe' (case-insensitive) here to avoid the situation
    ; Use comma to separate the program names
    ; Windows ONLY

**exclude_from_detection=a.exe, b.exe**

    ; Use another interface element detection algorithm for the windows of specific programs (since 1.10.2)
    ; Detecting the interface elements of some programs may cause Snipaste to be unresponsive or even crash
    ; To avoid this, you can put their program names here, Snipaste will use another algorithm for them,
    ; which is not likely to cause a crash, with the disadvantage of less detected elements
    ; Use comma to separate the program names
    ; Windows ONLY

**crashes=a.exe, b.exe**