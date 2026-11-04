# CrashSleuth

Finds out why a Windows PC crashes, freezes or shows error pop-ups, explains it in plain English, and fixes what it safely can, with an undo button.

**[Download the latest version](https://github.com/Moorey79/crashsleuth/releases/latest)** (Windows 10/11, 64-bit)

## What it does

- Reads Windows' own crash records: blue screen crash dumps, event logs and error reports, and names the driver, device or program behind the crashes.
- Checks drivers, startup programs, antivirus settings, drives, the CPU and BIOS for known problems, including malware hiding its tracks.
- Offers fixes you choose yourself. Before changing anything it makes a System Restore point, and every fix can be undone.
- Optionally watches in the background (a coloured dot by the clock) to catch crashes that happen while you're away.

It never deletes your files, never clears Windows' logs, doesn't "clean the registry" and doesn't install drivers.

## Installing

Run `CrashSleuth-Setup-x.y.z.exe`. This is a test version and isn't code-signed yet, so Windows may show **"Windows protected your PC"**: click **More info**, then **Run anyway**.

## Privacy

Nothing about your PC is sent anywhere. Reports stay on your PC (Documents > CrashSleuth Reports). CrashSleuth downloads Microsoft's free crash analyser (WinDbg) the first time it finds crash dumps, and small updates to its list of known problems.

## Testing it?

Thanks! After a scan, send the newest report from **Documents > CrashSleuth Reports** to whoever gave you CrashSleuth, plus a line on what actually turned out to be wrong if you found out.
