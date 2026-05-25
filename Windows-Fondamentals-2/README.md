# TryHackMe – Windows Fundamentals 2 (Technical Lab Notes)

This documentation summarizes all key actions, Windows admin tools, and technical concepts explored in the "Windows Fundamentals 2" room, following each task.

---

## Task 1: Introduction

Overview of the room objectives.

---

## Task 2: System Configuration & Advanced System Settings

- Used **System Configuration (msconfig)** for troubleshooting and startup diagnostics.
    - Access via Start Menu: `msconfig`
    - Five main tabs: General, Boot, Services, Startup (uses Task Manager), Tools.
    - "Tools" tab provides access to utilities like System Information, Event Viewer, User Account settings, etc.
- Open Task Manager for startup programs:
    - Run: `taskmgr`
- Checked advanced system settings via:
    - Right-click **This PC** > Properties > Advanced system settings.

---

## Task 3: Advanced System Settings (Performance & Recovery)

- Explored **Performance Options**:
    - Adjusted visual effects, processor scheduling, paging file (virtual memory).
- Viewed/edit crash dump settings under Startup and Recovery.
    - Example dump settings: Automatic memory dump, Kernel memory dump, etc.
- Noted important environment variables:
    - `%SystemRoot%`, `%TEMP%`, `%PATH%`, `ComSpec` (value: `%SystemRoot%\system32\cmd.exe`)

---

## Task 4: User Account Control & Computer Management

- Reviewed and changed **User Account Control (UAC) settings**:
    - Tool: `UserAccountControlSettings.exe`
    - UAC notification levels: Always notify, Notify for apps, Notify without dimming, Never notify.
- Used **Computer Management (compmgmt.msc)**:
    - Explored Task Scheduler (create automated tasks with triggers/actions)
    - Viewed tasks with `Task Scheduler Library`.
    - Event Viewer: checked Windows logs (Error, Warning, Information, Success/Failure Audit).
    - Shared Folders: managed shared network access.
    - Performance Monitor: `perfmon`
    - Local Users & Groups: `lusrmgr.msc`

---

## Task 5: Device Manager, Storage Management, Services

- Opened **Device Manager** to review hardware and drivers.
- Used Disk Management for viewing and configuring partitions.
- Listed and examined **Windows Services**:
    - Checked properties: Service name, executable path, Startup Type (Automatic, Manual, Disabled).
    - WMI Control and use of Windows Management Instrumentation (WMI).

---

## Task 6: System Information & Environment Variables

- Ran **System Information** with `msinfo32.exe`:
    - Reviewed: Hardware Resources, Components, Software Environment (drivers, services, system variables, running tasks, network).
- Explored and modified **Environment Variables** via Advanced system settings.

---

## Task 7: Resource Monitor & Command Line Tools

- Launched **Resource Monitor** with `resmon.exe`:
    - Analyzed CPU, Memory, Disk, and Network activity and stats.
- Used the **Command Prompt (cmd)** for troubleshooting:
    - Basic system/user commands:
        - `hostname` : Show computer name
        - `whoami`   : Current user
    - Network info and troubleshooting:
        - `ipconfig`         : Show IP configuration
        - `ipconfig /all`    : Detailed info
        - `netstat`          : Active connections
        - `netstat -a/-b/-n` : Parameters
        - `net help` and `net help user` : Help for net subcommands
        - `net user`, `net localgroup`, `net share`, `net session` : List/modify users and shares
        - To clear CMD: `cls`

---

## Task 8: Registry Editor

- Edited the **Windows Registry** with `regedit.exe`:
    - Learned about registry hives: `HKEY_CLASSES_ROOT`, `HKEY_CURRENT_USER`, `HKEY_LOCAL_MACHINE`, `HKEY_USERS`, `HKEY_CURRENT_CONFIG`
    - Warning about changes affecting system/apps/users.

---

## Task 9: Completion

All 9 tasks completed, room finished.

---

## Key Concepts Practiced

- Efficient use of Windows admin tools: msconfig, Computer Management, Task Scheduler, Event Viewer, Device Manager, Services, Disk Management, Resource Monitor, System Info, Registry Editor.
- Familiarity with Windows command-line utilities for troubleshooting and administration.

---

Lab documented by **Oyar12**.
