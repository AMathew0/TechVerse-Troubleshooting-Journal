# [Git Error] touch is not recognized by PowerShell

## Date:
- 2025-05-01

## Description:
- Tried to use the `touch` command in PowerShell to create a file but received an error.

## Environment:
- Local Laptop (Windows 11) using PowerShell

## Tools Involved:
- PowerShell, Git

## Troubleshooting Steps Taken:
1. Typed `touch README.md` in PowerShell.
2. Received: `'touch' is not recognized as the name of a cmdlet, function...`
3. Researched and found `touch` is a UNIX command not available in Windows PowerShell.

## Resolution:
- Used the Windows equivalent:
  ```powershell
  New-Item README.md

  Lessons Learned:
PowerShell has different command syntax; use New-Item instead of touch.

References:
https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.management/new-item
