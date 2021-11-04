## Settings

All of the settings you can configure in Authme.

## Launch on startup

Start the app after the operating system loaded. The app will start on the tray.

-   Default: Off

## Close app to tray

On closing the app will not quit. You can open the app from the tray menu.

-   Default: Off

## Window capture (Windows, Mac)

Disables screenshots and screen capture. You can't record or screenshot the app.

-   Default: off

## Hardware acceleration

Uses GPU for smoother experience. Enable this option if you experience frame drops or lags.

-   Default: off

## Show 2FA descriptions

The QR codes store a name field. You can turn it on, after restart on the main page you will see the name is the stored QR codes.

-   Default: Off

## Blur codes

Blurs the code, but you can still copy it.

-   Default: Off

## Reset search after copy

After you copy the code the search bar and the search results will reset.

-   Default: Off

## Save search history

Keep your search history.

-   Default: On

## Shortcuts

You can modify the shortcuts in the settings at the Shortcuts tab.

Supported modifiers:

-   Control (Command)
-   Alt (Option)
-   Shift

Default shortcuts:

-   Show/Hide app: <kbd>CommandOrControl</kbd> <kbd>Q</kbd>
    <br>
    <br>
-   Settings: <kbd>CommandOrControl</kbd> <kbd>S</kbd>
    <br>
    <br>
-   Exit app: <kbd>CommandOrControl</kbd> <kbd>W</kbd>
    <br>
    <br>
-   Reset: <kbd>CommandOrControl</kbd> <kbd>0</kbd>
    <br>
    <br>
-   Zoom in: <kbd>CommandOrControl</kbd> <kbd>1</kbd>
    <br>
    <br>
-   Zoom out: <kbd>CommandOrControl</kbd> <kbd>2</kbd>
    <br>
    <br>
-   Edit codes: <kbd>CommandOrControl</kbd> <kbd>T</kbd>
    <br>
    <br>
-   Import: <kbd>CommandOrControl</kbd> <kbd>I</kbd>
    <br>
    <br>
-   Export: <kbd>CommandOrControl</kbd> <kbd>E</kbd>
    <br>
    <br>
-   Documentation: <kbd>CommandOrControl</kbd> <kbd>D</kbd>
    <br>
    <br>
-   Release notes: <kbd>CommandOrControl</kbd> <kbd>N</kbd>
    <br>
    <br>
-   Support development: <kbd>CommandOrControl</kbd> <kbd>P</kbd>
    <br>
    <br>
-   Show licenses: <kbd>CommandOrControl</kbd> <kbd>L</kbd>
    <br>
    <br>
-   Update: <kbd>CommandOrControl</kbd> <kbd>U</kbd>
    <br>
    <br>
-   About: <kbd>CommandOrControl</kbd> <kbd>O</kbd>

## Global shortcuts

Global shortcuts work from everywhere, not only in the app.

Supported modifiers:

-   Control (Command)
-   Alt (Option)
-   Shift

Default shortcuts:

-   Show/Hide app: <kbd>CommandOrControl</kbd> <kbd>Shift</kbd> <kbd>A</kbd>
    <br>
    <br>
-   Settings: <kbd>CommandOrControl</kbd> <kbd>Shift</kbd> <kbd>S</kbd>
    <br>
    <br>
-   Exit: <kbd>CommandOrControl</kbd> <kbd>Shift</kbd> <kbd>D</kbd>

## Settings format

You can modify the settings file. See [folders](settings.md?id=folders) for more information.

```json
{
		"version":{
			"tag": "<ex. 2.7.2>",
			"build": "<ex. release.211012.162030>"
		},
		"settings": {
			"launch_on_startup": false,
			"close_to_tray": true,
			"show_2fa_names": false,
			"click_to_reveal": false,
			"reset_after_copy": false,
			"save_search_results": true,
			"disable_window_capture": true,
			"disable_hardware_acceleration": true
		},
		"experimental":{
			"sort": null,
			"webcam": "null"
		},
		"security": {
			"require_password": null,
			"password": null,
			"new_encryption": null,
			"key": null
		},
		"shortcuts": {
			"show": "CommandOrControl+q",
			"settings": "CommandOrControl+s",
			"exit": "CommandOrControl+w",
			"zoom_reset": "CommandOrControl+0",
			"zoom_in": "CommandOrControl+1",
			"zoom_out": "CommandOrControl+2",
			"edit": "CommandOrControl+t",
			"import": "CommandOrControl+i",
			"export": "CommandOrControl+e",
			"release": "CommandOrControl+n",
			"support": "CommandOrControl+p",
			"docs": "CommandOrControl+d",
			"licenses": "CommandOrControl+l",
			"update": "CommandOrControl+u",
			"info": "CommandOrControl+o"
		},
		"global_shortcuts": {
			"show": "CommandOrControl+Shift+a",
			"settings": "CommandOrControl+Shift+s",
			"exit": "CommandOrControl+Shift+d"
		},
		"quick_shortcuts:": {},
		"search_history": {
			"latest": null
		},
		"statistics": {
			"opens": 0,
			"rated": null,
			"feedback": null
		}
	}
```

## Folders

Settings file location:

-   Windows: `C:\Users\<username>\AppData\Roaming\Levminer\Authme`

-   Linux: `/home/<username>/Levminer/Authme`

-   Mac: `/Users/<username>/Levminer/Authme`

Cache file location:

-   Windows: `C:\Users\<username>\AppData\Roaming\authme`

-   Linux: `/home/<username>/.config/authme`

-   Mac: `/Users/<username>/Library/Application Support/authme`

## Experimental features

Some experimental features under development.

!> These features are unstable, use it at your own risk!

-   Use webcam for import

You can import QR code(s) directly from you camera.

-   Sort codes

By default codes sorted by uploading order, you can set it to A-Z or Z-A.
