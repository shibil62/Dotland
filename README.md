<div align="center">

# Dotland

**A Dynamic Island for Windows.**

Lightweight. Private. No installer, no account, no internet needed.

![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011-blue)
![Built with](https://img.shields.io/badge/built%20with-C%23%20%7C%20.NET%208%20%7C%20WPF-purple)
![Price](https://img.shields.io/badge/price-free-green)
![Privacy](https://img.shields.io/badge/data-stays%20on%20your%20PC-success)

[**Download the latest version**](https://github.com/shibil62/Dotland/releases/latest)

![Dotland](docs/screenshots/banner.png)

</div>

---

## What is Dotland?

Dotland turns the top of your screen into a small, quiet dark circle. It grows into a pill when something
is happening (music playing, a device connecting, your charger plugged in) and expands into a full panel
when you want quick controls. It is inspired by the iPhone's Dynamic Island, built from scratch for Windows.

No Electron, no browser engine, no cloud, no accounts.

## Download and install

1. Go to the [**Releases** page](https://github.com/shibil62/Dotland/releases/latest).
2. Download `Dotland-v1.0.0-win-x64.zip`.
3. Right-click the zip and choose **Extract All**.
4. Double-click `Dotland.exe`.

There is no installer, and you do **not** need to install .NET. Everything is bundled in the one file.

> **Windows says "Windows protected your PC"?**
> Dotland is a new independent app and is not code-signed (certificates cost money).
> Click **More info**, then **Run anyway**.

**Requirements:** Windows 10 (version 1809 or newer) or Windows 11, 64-bit.

## How it works

| State | What you see |
| --- | --- |
| Idle | A small dark circle |
| Privacy dot | An orange dot (microphone) or green dot (camera) while an app is using it |
| Compact media pill | Album art on the left, a live equalizer on the right while music plays |
| Expanded media panel | Artwork, title, artist, previous, play/pause and next |
| Quick controls | Wi-Fi, Bluetooth and sound buttons, a real volume slider, and your recent apps |
| Alerts | Short pop-ups for Wi-Fi, Bluetooth, volume, charging and battery |

* **Hover** the island and it responds immediately.
* **Click** the idle circle to open quick controls. Click the media pill to jump to the music app.
* **Long press** the island for 0.5 s to open quick controls.
* **Drag** the idle island to place it anywhere. The position is remembered.
* Move the pointer away and it collapses by itself.

![States](docs/screenshots/states.png)

## Features

### Media
* Shows what is playing from any app that talks to Windows media controls.
* Play, pause, previous and next control the real session.

![Media](docs/screenshots/media.png)

### Volume and brightness
* Real Windows volume and mute. Changing volume with your keyboard keys or another app updates the island too.
* Real brightness control on laptops.

![Volume](docs/screenshots/volume.png)

### Wi-Fi and Bluetooth
* Turn Wi-Fi and Bluetooth on or off, see the connected network, and browse available networks.
* A connection animation plays when a Bluetooth device such as earbuds or headphones connects.
* See battery levels of connected Bluetooth devices where Windows provides them.

![Connectivity](docs/screenshots/connectivity.png)

### Battery and charging
* An iPhone-style pop-up when you plug in the charger. The colour follows the charge: green, orange at 20% or less, red at 10% or less.
* Battery level and percentage appear when you hover the pill.

![Charging](docs/screenshots/charging.png)

### Clipboard history
* Keeps your recent copies (text, images and copied files). Click an entry to copy it again.
* History lives in memory only, is never written to disk, and is cleared when you quit.
* Content that password managers mark as sensitive is skipped.

![Clipboard](docs/screenshots/clipboard.png)

### Settings
Start Dotland a second time, and the settings window of the running island opens.

* Island position (nine screen positions), size and opacity
* Accent colour, optional accent rim light, animation speed
* Always on top, start with Windows, dim when idle
* Notification duration, animated equalizer on or off
* Hide the island during fullscreen apps (video only, any fullscreen, or never)
* A status list showing which Windows integrations are working on your PC

![Settings](docs/screenshots/settings.png)

## Privacy

* No account, no login, no analytics, and no internet connection is needed.
* Settings are stored in a small file in `%APPDATA%\DotlandWin`.
* A log file, `app.log`, is stored in the same folder to help with bug reports. It stays on your PC.
* Clipboard history is kept in memory only.

To remove everything, close Dotland, delete the folder you extracted, and delete `%APPDATA%\DotlandWin`.

## Updates

New versions are posted on the [Releases](https://github.com/shibil62/Dotland/releases) page.
Download the newest zip, close Dotland (settings window → **Quit island**), and replace the old `Dotland.exe`.

Click **Watch → Custom → Releases** at the top of this page to be notified of new versions.

## Uninstall

Close Dotland, delete the folder, and turn off **Start with Windows** in settings first if you had it on.

## Known limitations

* Windows only. Windows 10 1809 or newer.
* **Notifications** need a permission Windows usually only gives to packaged apps, so the notification card may show as unavailable in settings on your PC. Dotland never fakes it.
* **Wi-Fi and Bluetooth toggles** need "Let apps control device radios" enabled in Windows privacy settings. If Windows refuses, Dotland opens the matching Windows settings page instead.
* The Wi-Fi network name can require location permission on recent Windows versions.
* The microphone and camera dots read the same privacy information Windows itself uses. Microsoft could change it in a future update.
* The app is unsigned, so Windows shows a warning on first run, and some antivirus tools may flag it by mistake.

## Roadmap

- [ ] Windows installer
- [ ] More island styles and themes
- [ ] Code-signed releases

## Feedback and bugs

Found a bug or have an idea? Please open an [issue](https://github.com/shibil62/Dotland/issues) and include:

1. What you did and what you expected to happen.
2. Your Windows version.
3. The file `%APPDATA%\DotlandWin\app.log`, if it exists.

## Credits

Built with [NAudio](https://github.com/naudio/NAudio) (MIT) and the Windows SDK, on .NET 8 and WPF.
Dotland is an independent project and is not affiliated with Apple or Microsoft.

## License

Dotland is **freeware**. You may download, use and share the unmodified app freely for personal use.
The source code is not public, and modifying, reselling or reverse engineering the app is not permitted.

© 2026 Shibil · [@djonoz.cs](https://instagram.com/djonoz.cs)
