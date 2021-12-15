## Settings

All of the settings you can configure in Authme.

## Launch on startup

Start Authme after your computer started. Authme will start on the system tray.

-   Default: On

## Close app to tray

When closing Authme the app will not quit. You can open Authme from the system tray.

-   Default: On

## Window capture (Windows, Mac)

Allows screenshots and screen capture. You can record or screenshot the app until you restart Authme.

-   Default: off

## Hardware acceleration

Uses GPU for smoother experience. Enable this option if you experience frame drops or lags.

-   Default: off

## Codes description

The saved codes description will be visible. You can copy it after clicking it.

-   Default: Off

## Blur codes

Blur the saved codes. You can still copy it or hover over it to reveal.

-   Default: Off

## Search history

Save the latest code you searched for. Works even after restart.

-   Default: On

## Reset search after copy

Reset the search bar after you copied a code. Useful if you copy and search for a lot of codes.

-   Default: Off

## Shortcuts

You can modify the shortcuts in the settings at the Shortcuts tab.

Supported modifiers:

-   Control (Command)
-   Alt (Option)
-   Shift

Default shortcuts:

-   Show/Hide App: <kbd>CommandOrControl</kbd> <kbd>Q</kbd>
    <br>
    <br>
-   Settings: <kbd>CommandOrControl</kbd> <kbd>S</kbd>
    <br>
    <br>
-   Exit App: <kbd>CommandOrControl</kbd> <kbd>W</kbd>
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
-   Edit Codes: <kbd>CommandOrControl</kbd> <kbd>T</kbd>
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
-   Release Notes: <kbd>CommandOrControl</kbd> <kbd>N</kbd>
    <br>
    <br>
-   Support Development: <kbd>CommandOrControl</kbd> <kbd>P</kbd>
    <br>
    <br>
-   Show Licenses: <kbd>CommandOrControl</kbd> <kbd>L</kbd>
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

-   Show/Hide App: <kbd>CommandOrControl</kbd> <kbd>Shift</kbd> <kbd>A</kbd>
    <br>
    <br>
-   Settings: <kbd>CommandOrControl</kbd> <kbd>Shift</kbd> <kbd>S</kbd>
    <br>
    <br>
-   Exit App: <kbd>CommandOrControl</kbd> <kbd>Shift</kbd> <kbd>D</kbd>

## Settings format

You can modify the settings file. See [folders](settings.md?id=folders) for more information.

```json
{
	info: {
		version: <ex. 2.7.4>,
		build: <ex. release.211214.153017>,
		date: <ex. 2021. December 14.>,
	},
	settings: {
		launch_on_startup: true,
		close_to_tray: true,
		codes_description: false,
		blur_codes: false,
		reset_after_copy: false,
		search_history: true,
		hardware_acceleration: true,
		search_filter: {
			name: true,
			description: false,
		},
		default_display: 1,
	},
	experimental: {
		sort: null,
		screen_capture: false,
	},
	security: {
		require_password: null,
		password: null,
		key: null,
	},
	shortcuts: {
		show: "CmdOrCtrl+q",
		settings: "CmdOrCtrl+s",
		exit: "CmdOrCtrl+w",
		zoom_reset: "CmdOrCtrl+0",
		zoom_in: "CmdOrCtrl+1",
		zoom_out: "CmdOrCtrl+2",
		edit: "CmdOrCtrl+t",
		import: "CmdOrCtrl+i",
		export: "CmdOrCtrl+e",
		release: "CmdOrCtrl+n",
		support: "CmdOrCtrl+p",
		docs: "CmdOrCtrl+d",
		licenses: "CmdOrCtrl+l",
		update: "CmdOrCtrl+u",
		info: "CmdOrCtrl+o",
	},
	global_shortcuts: {
		show: "CmdOrCtrl+Shift+a",
		settings: "CmdOrCtrl+Shift+s",
		exit: "CmdOrCtrl+Shift+d",
	},
	quick_shortcuts: {},
	search_history: {
		latest: null,
	},
	statistics: {
		opens: 0,
		rated: null,
		feedback: null,
	},
}
```

## Folders

Settings file location:

-   Windows: `C:\Users\<username>\AppData\Roaming\Levminer\Authme`

-   Linux: `/home/<username>/.config/Levminer/Authme`

-   Mac: `/Users/<username>/Library/Application Support/Levminer/Authme`

Cache file location:

-   Windows: `C:\Users\<username>\AppData\Roaming\Authme`

-   Linux: `/home/<username>/.config/Authme`

-   Mac: `/Users/<username>/Library/Application Support/Authme`

## Experimental features

Some experimental features under development.

!> These features are unstable, use it at your own risk!

-   Use webcam for import

You can import QR code(s) directly from you camera.

-   Sort codes

By default codes sorted by uploading order, you can set it to A-Z or Z-A.
