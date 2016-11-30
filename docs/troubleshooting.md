# Troubleshooting

## Windows

### "The program can't start because **api-ms-win-crt-runtime-l1-1-0.dll** is missing"
* Please install the correct version (32-bit/64-bit) of [Visual C++ Redistributable for VS 2015](https://www.microsoft.com/en-us/download/details.aspx?id=48145).
* If for some reason you are unable to install VC2015, you can also download this zip file ([32-bit](https://dl.snipaste.com/vc2015-dll-x86) | [64-bit](https://dl.snipaste.com/vc2015-dll-x64)). Unzip it and put all the dll files into the Snipaste directory.

### "Not a valid 32-bit application" when running on Windows XP 32-bit
* Please [download](https://www.snipaste.com/download.html) the pack for XP.

### "Network Error: 99" when checking for updates
* It's usually due to lack of libeay32.dll and ssleay32.dll in the Snipaste directory. Please download the full pack and unzip it completely.

### After restarting Snipaste, the settings are automatically reset to the defaults
* Reason: Snipaste cannont write into config.ini under the same folder as Snipaste.exe
* The solution is thus straghtforward: make config.ini writable.
  * Do not put Snipaste into the C:\Program Files\ or C:\Program Files(x86\. Files in such directories need admin privilege for write permission.
  * Maybe there are some problem with your disk permissions (possibly caused by system upgrade). Please google it yourself because the situation depends.
  * If the problem still exists, running Snipaste as an Admin should do the trick.

### Cannot set the hotkey to some key combinations (e.g. keys with <kbd>Win</kbd>)
* Some of the key combinations with <kbd>Win</kbd> are occupied by the system.
* Similarly, keys occupied by other programs cannot be used by Snipaste. Please unset the hotkeys in other programs.

### Sometimes the global hotkeys have no response
* If Snipaste is not run as admin, while the current active window is run as admin, the hotkeys will be ineffective.
* Solutions:
  * Click on the taskbar or any other non-admin window BEFORE you press the hotkey.
  * Or, run Snipaste as admin too.

### "Run on system startup" fails
* Did you have "Run this program as an administrator" checked in the Properties Dialog of Snipaste.exe?
  * Upgrade to the latest Snipaste. Startup as admin on system boot is supported since v1.10.0.

### UI elements in the Chrome browser cannot be automatically detected when snipping
* Please enable the `Global accessibility mode` in [chrome://accessibility/](chrome://accessibility/).
  * You need to enable this flag every time you launch Chrome.
  * If you wish to enable `Global accessibility mode` automatically, you can launch Chrome with the `--force-renderer-accessibility` flag.
* Firefox and IE naturally support this feature and need no further settings.

### The code has syntax highlight in the code editor, but after pasted by Snipaste, the syntax highlight is lost in the image window
* It is because the code you copied is pure text and not in HTML format.
* If you want the text be syntax highlighted, please use code editors that support HTML copy.
 * I personally recommend using Visual Studio. With "Productivity Power Tools" extension installed and the extension's "HTML Copy" feature enabled, the pasted image shall be rendered the same as the editor.

### The image window cannot be moved across the top border of the screen
 * `System Properties` - `Advanced` - `Performance settings` - `Visual effects` - **Check** `Show window contents while window dragging` - `OK`

![](https://cloud.githubusercontent.com/assets/2010459/20704971/25d64640-b65c-11e6-9287-b42309145359.png)
