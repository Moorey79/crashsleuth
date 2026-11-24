# CrashSleuth privacy policy

*Last updated: 24 November 2026*

CrashSleuth is a Windows utility made by Steve Moorey (New South Wales, Australia). It works out why a PC crashes and fixes the cause. This policy covers the CrashSleuth app, whether installed from the Microsoft Store or from GitHub.

## What CrashSleuth looks at
To do its job, CrashSleuth reads information that's already on your PC: crash dumps, Windows event logs, drivers, installed programs, services, scheduled tasks, startup entries, Windows Security (Defender) settings, and performance counters. With the background monitor on, it also records memory and resource use, error dialogs (including a screenshot of the dialog), and changes to programs and settings. It also notes which programs connect to the internet (where to, when and how much, never what they send), keeps that for 24 hours where only administrators can read it, and leaves out programs that are signed and installed in Windows or Program Files, such as your browser. That's how it spots malware and adware calling home. After a crash it keeps a copy of Windows' full crash dump (which can hold anything that was in memory) for its deeper analysis, where only administrators can read it: the newest two, for 60 days at most, and only when there's plenty of free disk space.

## Where it goes
**Everything stays on your PC.** CrashSleuth keeps its history, reports and undo records in `C:\ProgramData\CrashSleuth` and your user folders. It has no accounts, no analytics, no advertising and no telemetry. Nothing about you or your PC is sent to the developer or anyone else.

## The only things it downloads
- **Known-issue rules:** about once a day it checks for an updated, digitally signed rules file at github.com/Moorey79/crashsleuth-rules. Nothing is uploaded. GitHub sees an ordinary download request, under GitHub's own privacy policy.
- **CrashSleuth's own updates (the GitHub version only; the Store version is updated by the Store):** about once a day, and when you choose Check for updates, it reads a small, digitally signed list of the latest version from github.com/Moorey79/crashsleuth and, if there's a newer one, downloads only the parts that changed. Nothing is uploaded. GitHub sees an ordinary download request, under GitHub's own privacy policy. You can make it ask first, or stop it checking, from the tray menu.
- **Microsoft's crash analyser (optional):** if a crash dump needs it, and you've allowed it, CrashSleuth downloads Microsoft's debugging tools and symbol files from Microsoft's servers, under Microsoft's privacy policy.
- **Driver updates on offer:** once a day a scan asks Windows Update (Windows' own service) which newer drivers it has for this PC. Windows Update contacts Microsoft the same way it does for your normal updates. A driver is installed only if you choose that fix.

## Sharing reports
CrashSleuth never sends a report by itself. Every scan saves a **-shareable** copy with your user names, PC name, email, network and web addresses, and error-dialog screenshots removed (though it still lists installed software). If you choose to email a report to `reports@directcompare.dev`, it is used only to help you and improve CrashSleuth, is never shared with anyone else, and is deleted on request.

## AI assistants
If you connect CrashSleuth to the Claude desktop app (off unless you turn it on), Claude can run scans and read reports on your PC. What Claude does with that information is covered by Anthropic's privacy policy.

## Children
CrashSleuth isn't aimed at children and collects nothing from anyone.

## Contact
Questions or deletion requests: reports@directcompare.dev
