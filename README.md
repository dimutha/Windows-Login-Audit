# Windows Login Audit

A PowerShell script to monitor and log Windows server login activities, including:

- Successful logins
- Failed login attempts
- Logons with explicit credentials
- Logoffs

## Features

- Automatically deletes logs older than 30 days
- Generates CSV files for easy analysis
- Can be scheduled via Task Scheduler

## Usage

1. Update `$Path` in `LoginAudit.ps1` to your preferred log folder.
2. Schedule the script via Task Scheduler (daily recommended):
   ```powershell
   powershell.exe -File "C:\SysAudit\Scripts\LoginAudit.ps1"
   
3. Review generated CSV files in the log folder.
   ```log file path
   "C:\SysAudit\Logs\"
   
4. Once the log files geting older than 30 days, these will be automatically deleted.
