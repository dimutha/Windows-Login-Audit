# Windows Login Audit

A PowerShell script to monitor, log, and analyze Windows server login activities. This tool helps track successful logins, failed attempts, logons using explicit credentials, and user logoffs, making it easier to detect unauthorized access and maintain security compliance.

---

## Features

- Logs **successful logins**, **failed logins**, **explicit credential logons**, and **logoffs**
- Automatically deletes logs older than 30 days to manage storage
- Generates **CSV reports** for easy analysis and tracking
- Can be scheduled using **Windows Task Scheduler** to run automatically

---

## Requirements

- Windows Server or Windows workstation
- PowerShell 5.1 or higher
- Administrative privileges to read Security event logs

---

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/dimutha/Windows-Login-Audit.git

2. Navigate to the Scripts folder:
   ```example
   Example:
           "C:\SysAudit\Scripts\"

3. Update the $Path variable in LoginAudit.ps1 to your preferred log storage location.
   ```example
   Example:
           "C:\SysAudit\Logs\"

---

## Usage

Run the script manually Or schedule it via Task Scheduler to run automatically once per day.
Pictorial guid to Task Scheduler Config has attaced.

The script will generate CSV log files in the specified folder with the following columns:
- TimeCreated – Timestamp of the event
- EventType – Logon, Logoff, LogonFailed, or LogonAttempted
- UserName – User account name
- IPAddress – IP address of the client machine

---

## Contributing

Contributions, suggestions, and bug reports are welcome! Feel free to open an issue or submit a pull request.

---

## License

This project is licensed under the MIT License 

---

## Author

Dimutha Kumara – https://www.linkedin.com/in/dimutha-kumara-16562220/
