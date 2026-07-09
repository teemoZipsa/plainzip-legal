# PlainZip Privacy Policy

Last updated: 2026-07-09

PlainZip is a local Windows archive utility. It previews, extracts, and creates archive files on your device.

## Data PlainZip Accesses

PlainZip accesses files and folders that you choose through drag and drop, file dialogs, Windows file association launches, or supported command-line/startup actions. This can include archive file names, folder paths, archive entry names, file sizes, and archive metadata needed to preview or extract archives.

PlainZip may process archive passwords that you enter for encrypted archives. Passwords are used only to run the current archive operation.

## Data PlainZip Stores Locally

PlainZip stores app settings locally, such as theme, output-folder preferences, and supported shell-action preferences.

Settings are stored next to the executable in portable mode when that location is writable. If that location is not writable, settings are stored under:

```text
%LOCALAPPDATA%\PlainZip\settings.json
```

When command-line or supported shell-action jobs fail or need user-visible follow-up, PlainZip may write local diagnostic logs under:

```text
%LOCALAPPDATA%\PlainZip\logs\
```

Logs may include local file paths, archive names, archive entry names, and error messages. PlainZip masks archive passwords in UI and logs.

## Data Collection And Transmission

PlainZip does not upload, sell, or share your files, archive contents, passwords, settings, or logs.

PlainZip does not include advertising, analytics, telemetry, tracking SDKs, or cloud sync. Archive operations run locally on your device using the bundled 7-Zip command-line runtime.

## Password Handling

When an archive password is entered, PlainZip sends it to the bundled 7-Zip process through stdin for the active operation. PlainZip does not intentionally save archive passwords to disk. The password exists in process memory while the operation is running.

## Third-Party Components

PlainZip includes the 7-Zip command-line runtime to provide archive support. 7-Zip runs locally on your device. Its license text is included with PlainZip and in this repository at:

```text
src-tauri/licenses/7zip-license.txt
```

## User Controls

You can remove PlainZip's local settings and logs by deleting:

```text
%LOCALAPPDATA%\PlainZip\
```

If you use portable mode and settings are stored next to the executable, delete the adjacent `settings.json` file.

The Microsoft Store MSIX build does not declare Explorer context-menu integration in its package manifest.

## Changes

This privacy policy should be updated when PlainZip adds features that collect, store, transmit, or share additional data.

## Contact

For privacy questions, contact:

Use the support or contact option listed on PlainZip's Microsoft Store product page.
