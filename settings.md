## Settings

All of the settings you can configure in Authme.

## Launch on startup

?> Windows only

Start the app after the operating system loaded. The app will start on the tray.

-   Default: Off

## Close app to tray

?> Windows only

If you close the app it will not quit. You can open the app from the tray menu.

-   Default: Off

## Reset search after copy

After you copy the code the search bar and the search results will reset.

-   Default: On

## Show 2FA names

The QR codes store a name field. You can turn it on, after restart on the main page you will see the name is the stored QR codes.

-   Default: Off

## Shortcuts

You can modify the not global shortcuts. After you done, restart the app to make the new shortcuts work.

Supported modifiers:

-   Control (Command)
-   Alt (Option)
-   Shift

Shortcuts in the app supports only a modifier and a key (CommandOrControl+s). If you want to use two modifier and a key take a look at the: [Advanced Configuration](settings.md?id=advanced-configuration).

Default shortcuts:

-   Show app: <kbd>CommandOrControl</kbd> + <kbd>Q</kbd>
    <br>
    <br>
-   Show settings: <kbd>CommandOrControl</kbd> + <kbd>S</kbd>
    <br>
    <br>
-   Exit app: <kbd>CommandOrControl</kbd> + <kbd>W</kbd>
    <br>
    <br>
-   Open Authme Web: <kbd>CommandOrControl</kbd> + <kbd>A</kbd>
    <br>
    <br>
-   Show import: <kbd>CommandOrControl</kbd> + <kbd>I</kbd>
    <br>
    <br>
-   Show export: <kbd>CommandOrControl</kbd> + <kbd>E</kbd>
    <br>
    <br>
-   Open releases: <kbd>CommandOrControl</kbd> + <kbd>R</kbd>
    <br>
    <br>
-   Open issues: <kbd>CommandOrControl</kbd> + <kbd>P</kbd>
    <br>
    <br>
-   Open Docs: <kbd>CommandOrControl</kbd> + <kbd>D</kbd>
    <br>
    <br>
-   Open licenses: <kbd>CommandOrControl</kbd> + <kbd>L</kbd>
    <br>
    <br>
-   Check for update: <kbd>CommandOrControl</kbd> + <kbd>U</kbd>
    <br>
    <br>
-   About Authme: <kbd>CommandOrControl</kbd> + <kbd>O</kbd>

## Gobal shortcuts

Global shortcuts work from everywhere, not only in the app.

Supported modifiers:

-   Control (Command)
-   Alt (Option)
-   Shift

Shortcuts in the app supports only a modifier and a key (CommandOrControl+s). If you want to use two modifier and a key take a look at the: [Advanced Configuration](settings.md?id=advanced-configuration).

Default shortcuts:

-   Open/Close app: <kbd>CommandOrControl</kbd> + <kbd>Shift</kbd> + <kbd>A</kbd>
    <br>
    <br>
-   Exit app: <kbd>CommandOrControl</kbd>+ <kbd>Shift</kbd> + <kbd>S</kbd>
    <br>
    <br>
-   Open/Close import page: <kbd>CommandOrControl</kbd>+ <kbd>Shift</kbd> + <kbd>D</kbd>

## Advanced configuration

Settings file location:

-   Windows: `C:\Users\<username>\AppData\Roaming\Levminer\Authme`

-   Linux: `/home/<username>/Levminer/Authme`

Settings format:

```json
{
	"version": {
		"tag": "<your_version>"
	},

	"settings": {
		"launch_on_startup": false,
		"close_to_tray": false,
		"show_2fa_names": false,
		"click_to_reveal": false,
		"reset_after_copy": true
	},

	"security": {
		"require_password": null,
		"password": null
	},

	"shortcuts": {
		"show": "CommandOrControl+q",
		"settings": "CommandOrControl+s",
		"exit": "CommandOrControl+w",
		"web": "CommandOrControl+a",
		"import": "CommandOrControl+i",
		"export": "CommandOrControl+e",
		"release": "CommandOrControl+r",
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
	}
}
```

Supported shortcut modifiers and key codes:

-   View Supported modifiers on Electron docs: [Modifiers](https://www.electronjs.org/docs/api/accelerator#available-modifiers)

-   View Supported key codes on Electron docs: [Key codes](https://www.electronjs.org/docs/api/accelerator#available-key-codes)
