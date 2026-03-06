---
title: Remote Query User
summary: Quick note on checking Remote Desktop sessions with PowerShell.
date: 2019-04-17T14:24:00+08:00
authors:
  - me
tags:
  - windows
  - powershell
aliases:
  - /blog/remote-query-user/
---

A colleague asked if someone was remotely logged into a workstation. I found a simple way to
check this from PowerShell using `quser`.

Run:

```powershell
Enter-PSSession -ComputerName COMPUTERNAME
quser
```

You can then log off a session by ID:

```powershell
logoff ID
```

Reference: [quser docs](https://learn.microsoft.com/windows-server/administration/windows-commands/quser)
