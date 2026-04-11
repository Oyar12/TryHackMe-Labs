# TryHackMe – Windows Fundamentals 1

**Room**: [Windows Fundamentals 1](https://tryhackme.com/room/windowsfundamentals1xbx)  
**Goal**: Understand the basics of the Windows operating system – interface, NTFS, UAC, user management, Task Manager, etc.

## What I learned

- **NTFS**: journaling file system, supports files >4GB, permissions, EFS, Alternate Data Streams (ADS).
- **Windows editions**: Home vs Pro (BitLocker available only on Pro).
- **Desktop components**: Desktop, Start Menu, Taskbar, Notification Area.
- **User Account Control (UAC)**: protects administrators from unintended high‑privilege executions.
- **User management**: Administrator / Standard accounts, user profiles, local groups (`lusrmgr.msc`).
- **System tools**: Settings, Control Panel, Task Manager (shortcut `Ctrl+Shift+Esc`).
- **Environment variables**: `%windir%` points to the Windows folder.

## Key commands / concepts

| Concept | Details |
|---------|---------|
| `lusrmgr.msc` | Local Users and Groups management |
| `Ctrl+Shift+Esc` | Open Task Manager directly |
| `%windir%` | Path to Windows folder (e.g., `C:\Windows`) |
| `BitLocker` | Disk encryption – only on Windows Pro |
| `UAC` | Prompt for elevated actions |

## Room answers (for personal reference)

- Encryption missing on Home: **BitLocker**
- Other user account: `tryhackmebilly`
- Groups of that user: `Remote Desktop Users, Users`
- Built‑in guest account: `Guest`
- Account description: `window$Fun1!`
- Task Manager keyboard shortcut: `Ctrl+Shift+Esc`

## Completion

- Room completed on [date]
- Points earned: 104
- Streak: +1

---

*Part of my SOC Analyst training – documented live.*<img width="1091" height="526" alt="Screenshot 2026-04-08 113847" src="https://github.com/user-attachments/assets/84444679-786a-4346-9a3e-fcc7bf246304" />
