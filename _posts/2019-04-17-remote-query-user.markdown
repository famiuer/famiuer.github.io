---
layout: post
title:  "Remote Query User"
date:   2019-04-17 14:24:00 +0800
categories: blog
---

Today a colleague asked me if I was logging on a workstation remotely when I was not. She got the answer and asked others. I thought there must be a tool or method to check the remote login status without logging in via remote desktop.

I searched and found that using PowerShell and _quser.exe_ can achieve the purpose within a company domain.

Open PowerShell and run following commands after replacing the COMPUTERNAME

    Enter-PSSession -ComputerName COMPUTERNAME
    quser

[Quser](https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/quser) will show the information about user sessions on a Remote Desktop Session Host. You may use the ID and log it off in PowerShell by

    logoff ID
