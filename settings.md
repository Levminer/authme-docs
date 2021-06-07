## Settings

All of the settings you can configure in Authme.

## Launch on startup

Start the app after the operating system loaded. The app will start on the tray.

-   Default: Off

## Close app to tray

On closing the app will not quit. You can open the app from the tray menu.

-   Default: Off

## Disable window capture

Disables screenshots and screen capture. You can't record or screenshot the app.

-   Default: On

## Show 2FA names

The QR codes store a name field. You can turn it on, after restart on the main page you will see the name is the stored QR codes.

-   Default: Off

## Reveal code

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

-   Show app: <kbd>CommandOrControl</kbd> <kbd>Q</kbd>
    <br>
    <br>
-   Show settings: <kbd>CommandOrControl</kbd> <kbd>S</kbd>
    <br>
    <br>
-   Exit app: <kbd>CommandOrControl</kbd> <kbd>W</kbd>
    <br>
    <br>
-   Open Authme Web: <kbd>CommandOrControl</kbd> <kbd>B</kbd>
    <br>
    <br>
-   Show import: <kbd>CommandOrControl</kbd> <kbd>I</kbd>
    <br>
    <br>
-   Show export: <kbd>CommandOrControl</kbd> <kbd>E</kbd>
    <br>
    <br>
-   Open releases: <kbd>CommandOrControl</kbd> <kbd>R</kbd>
    <br>
    <br>
-   Open issues: <kbd>CommandOrControl</kbd> <kbd>P</kbd>
    <br>
    <br>
-   Open Docs: <kbd>CommandOrControl</kbd> <kbd>D</kbd>
    <br>
    <br>
-   Open licenses: <kbd>CommandOrControl</kbd> <kbd>L</kbd>
    <br>
    <br>
-   Check for update: <kbd>CommandOrControl</kbd> <kbd>U</kbd>
    <br>
    <br>
-   About Authme: <kbd>CommandOrControl</kbd> <kbd>O</kbd>

## Gobal shortcuts

Global shortcuts work from everywhere, not only in the app.

Supported modifiers:

-   Control (Command)
-   Alt (Option)
-   Shift

Default shortcuts:

-   Open/Close app: <kbd>CommandOrControl</kbd> <kbd>Shift</kbd> <kbd>A</kbd>
    <br>
    <br>
-   Exit app: <kbd>CommandOrControl</kbd> <kbd>Shift</kbd> <kbd>S</kbd>
    <br>
    <br>
-   Open/Close import page: <kbd>CommandOrControl</kbd> <kbd>Shift</kbd> <kbd>D</kbd>

## Settings format

You can modify the settings file. See [folders](settings.md?id=folders) for more informations.

```json
{
	"version": {
		"tag": "<version>"
	},
	"settings": {
		"launch_on_startup": false,
		"close_to_tray": false,
		"show_2fa_names": false,
		"click_to_reveal": false,
		"reset_after_copy": false,
		"save_search_results": true,
		"disable_window_capture": true
	},
	"advanced_settings": {
		"offset": null
	},
	"security": {
		"require_password": null,
		"password": null
	},
	"shortcuts": {
		"show": "CommandOrControl+q",
		"settings": "CommandOrControl+s",
		"exit": "CommandOrControl+w",
		"web": "CommandOrControl+b",
		"import": "CommandOrControl+i",
		"export": "CommandOrControl+e",
		"release": "CommandOrControl+n",
		"issues": "CommandOrControl+p",
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
	"search_history": {
		"latest": null
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
