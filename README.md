# CrashSleuth

Finds out why a Windows PC crashes, freezes or shows error pop-ups, explains it in plain English, and fixes what it safely can, with an undo button.

**[Download the latest version](https://github.com/Moorey79/crashsleuth/releases/latest)** (Windows 10/11, 64-bit)

Or get it from the Microsoft Store https://apps.microsoft.com/detail/9N7W1RS508CL?hl=en-us&gl=AU&ocid=pdpshare

## What it does

- **Goes past `ntoskrnl.exe`:** Reads blue screen crash dumps, event logs, and error reports—and when Windows blames itself, runs deeper WinDbg checks (`!pool` memory tracing, `!running -it` across CPU cores, `!irp` sleep/wake hangs, and annotated call stacks) to name the real third-party driver behind the crash.
- **Saves your last two full dumps:** Keeps copies of your two newest `MEMORY.DMP` files before Windows overwrites them (respecting disk-space limits) so evidence isn't lost on a second crash.
- **Checks the whole system:** Scans drivers, startup programs, antivirus settings, drive health, temperatures/power history, CPU and BIOS for known problems, including malware hiding its tracks.
- **Offers safe, reversible fixes:** You choose what to apply. Before changing anything it makes a System Restore point, and every fix can be undone.
- **Optional background monitor:** Watches in the background (a coloured dot by the clock) to catch crashes while you're away, slow memory/handle leaks, and programs calling home the way adware and malware do.

It never deletes your files, never clears Windows' logs, doesn't "clean the registry" and doesn't install drivers.

## Installing

Run `CrashSleuth-Setup-x.y.z.exe`. This is a test version and isn't code-signed yet, so Windows may show **"Windows protected your PC"**: click **More info**, then **Run anyway**. (You can verify the download's SHA-256 checksum against the `.sha256.txt` file on the release page.)

OR, if you really don't trust anything with those warnings, you can get it from the Microsoft Store. https://apps.microsoft.com/detail/9N7W1RS508CL?hl=en-us&gl=AU&ocid=pdpshare

## Privacy

Nothing about your PC is sent anywhere automatically. Reports stay on your PC (`Documents > CrashSleuth Reports`) unless you choose to email one. The background monitor notes which programs go online (where to and when, never what they send), leaves out signed programs in Windows and Program Files such as your browser, and keeps it for 24 hours where only administrators can read it. Full details: [privacy policy](PRIVACY.md). CrashSleuth downloads Microsoft's free crash analyser (WinDbg) the first time it finds crash dumps, and small signed updates to its list of known problems.

## Sending a report

Thanks for testing! After a scan, email the newest report ending in **-shareable** from **Documents > CrashSleuth Reports** (the `.txt` or `.html` file) to **reports@directcompare.dev**. That copy has your names, the PC's name, email, network and web addresses and screenshots taken out.

If you found out what was really wrong with the PC, add a line saying so ("CrashSleuth said X, it turned out to be Y"). That's the most useful thing you can send.

Please don't attach reports to GitHub issues: they're public, and even the shareable copy lists installed programs.
