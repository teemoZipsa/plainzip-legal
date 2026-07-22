# PlainZip Privacy Policy

Last updated: 2026-07-22

PlainZip is a local Windows archive utility. It previews, extracts, and creates archive files on your device.

## Data PlainZip Accesses

PlainZip accesses files and folders that you choose through drag and drop, file dialogs, Windows file association launches, or supported command-line/startup actions. This can include archive file names, folder paths, archive entry names, file sizes, and archive metadata needed to preview or extract archives.

PlainZip may process archive passwords that you enter for encrypted archives. Passwords are used only to run the current archive operation.

## Data PlainZip Stores Locally

PlainZip stores app settings locally, such as theme, output-folder preferences, supported shell-action preferences, saved compression profiles, ordered extraction-conflict rules, up to 12 Quick Workflows, and—when enabled—up to 100 workflow-history records. A workflow record can include source and output paths, counts, sizes, duration, warning counts, completion status, and non-secret options needed to prepare the same inputs again. A Quick Workflow copies only its source paths and non-secret repeat setup. Neither includes archive passwords, filename-encryption state, or file contents.

Settings are stored locally under:

```text
%LOCALAPPDATA%\PlainZip\settings.json
```

When command-line or supported shell-action jobs fail or need user-visible follow-up, PlainZip may write local diagnostic logs under:

```text
%LOCALAPPDATA%\PlainZip\logs\
```

Logs may include local file paths, archive names, archive entry names, and error messages. PlainZip masks archive passwords in UI and logs.

Users can explicitly export workflow history or one completed workflow as JSON or CSV to a file location they choose. PlainZip does not upload those reports.

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

Workflow history can also be disabled or cleared directly in PlainZip Settings. Quick Workflows remain independent from history and can be removed individually in the Workflow Center. Saved JSON and CSV reports remain wherever you chose to save them and must be deleted from that location separately.

PlainZip 0.6.7 can receive paths selected through its packaged Windows 11 Explorer context-menu command. Explorer passes those paths locally to the installed PlainZip app only after you invoke the command. This does not upload or share file paths, file contents, passwords, settings, or logs.

## Changes

This privacy policy should be updated when PlainZip adds features that collect, store, transmit, or share additional data.

## Contact

For privacy questions, contact:

Use the support or contact option listed on PlainZip's Microsoft Store product page.
