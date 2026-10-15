# LUcker
LUcker is an autocklicker by Lubijbi
# LUcker – Auto Clicker

LUcker is a free Windows desktop clicker and mouse macro recorder. Actions and settings stay on this PC; the app has no telemetry, network access, sign-in, or administrator requirement.

English is the default interface language. You can switch to German in **Settings → Appearance → Language**; the choice is saved locally.

## Run

Download `dist/LUcker.exe` from this release folder and open it. The app stores settings and macros in `%LOCALAPPDATA%\LUcker`. No installation is needed.

## Features

- Left, right, and middle click; interval, optional limit, and an ordered list of fixed screen positions with a per-position delay.
- Start/stop with F6 and emergency stop with F9.
- Mouse-only macro recording (movement and clicks), playback repeats, preview, rename, and delete. No keyboard text is recorded.
- F7 toggles recording; F8 plays the selected macro. In Settings, click **Set hotkey** and press any key or key combination (for example Ctrl+Alt+K) to change a binding. Press **Esc** in the capture dialog to disable that binding. Conflicts with another application are reported, and the old bindings remain active.
- Macro recordings are stored locally as versioned `.lucker` files. Use the Macro page to import or export those files.
- Dark and light themes.

## Build on Windows

The source targets .NET Framework 4.0 WinForms and uses only Windows system libraries. From PowerShell on Windows:

```bat
.\build.ps1
```

The build embeds the supplied multicolor mouse emblem as the EXE and window icon. It uses the Windows .NET Framework already present on Windows 10/11. No third-party runtime packages are required.

## Safety

Mouse automation can affect the active application. Use the visible emergency stop or F9 to stop all activity. LUcker records only mouse movement and mouse buttons while its recording mode is visibly active. It does not record keyboard input.

## License

MIT. See [LICENSE](LICENSE).
