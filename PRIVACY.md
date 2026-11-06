# CrashSleuth privacy policy

*Last updated: 6 November 2026*

CrashSleuth is a Windows utility made by Steve Moorey (New South Wales, Australia). It works out why a PC crashes and fixes the cause. This policy covers the CrashSleuth app, whether installed from the Microsoft Store or from GitHub.

## What CrashSleuth looks at
To do its job, CrashSleuth reads information that's already on your PC: crash dumps, Windows event logs, drivers, installed programs, services, scheduled tasks, startup entries, Windows Security (Defender) settings, and performance counters. With the background monitor on, it also records memory and resource use, error dialogs (including a screenshot of the dialog), and changes to programs and settings.

## Where it goes
**Everything stays on your PC.** CrashSleuth keeps its history, reports and undo records in `C:\ProgramData\CrashSleuth` and your user folders. It has no accounts, no analytics, no advertising and no telemetry. Nothing about you or your PC is sent to the developer or anyone else.

## The only things it downloads
- **Known-issue rules:** about once a day it checks for an updated, digitally signed rules file at github.com/Moorey79/crashsleuth-rules. Nothing is uploaded. GitHub sees an ordinary download request, under GitHub's own privacy policy.
- **Microsoft's crash analyser (optional):** if a crash dump needs it, and you've allowed it, CrashSleuth downloads Microsoft's debugging tools and symbol files from Microsoft's servers, under Microsoft's privacy policy.

## Sharing reports
CrashSleuth never sends a report by itself. If you choose to email a report to the developer for help, it contains details of your PC (computer name, hardware, installed software, and crash and event history). Only send what you're happy to share. Reports sent to reports@directcompare.dev are used only to help you and to improve CrashSleuth. They're not shared with anyone, and are deleted on request.

## AI assistants
If you connect CrashSleuth to the Claude desktop app (off unless you turn it on), Claude can run scans and read reports on your PC. What Claude does with that information is covered by Anthropic's privacy policy.

## Children
CrashSleuth isn't aimed at children and collects nothing from anyone.

## Contact
Questions or deletion requests: reports@directcompare.dev
