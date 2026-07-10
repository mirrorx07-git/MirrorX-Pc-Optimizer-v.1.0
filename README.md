# 🚀MirrorX PC Optimizer v1.0

<div align="center">
Version
Platform
License
Language
Status

A powerful, lightweight, all-in-one Windows optimization and cleanup utility

Boost your PC performance with a single click

Features • Installation • Usage • Menu Options • FAQ

</div>
📖 Overview
MirrorX PC Optimizer is a professional-grade Windows batch utility designed to clean, optimize, and speed up your PC. Built with compatibility in mind, it works flawlessly across Windows 7, 8, 10, and 11 — including the latest builds where legacy tools like wmic are deprecated.

Whether you need a quick one-click cleanup or a detailed optimization report, MirrorX has you covered.

✨ Features

🎯 Interactive Menu System — Easy-to-use numbered options
⚡ All-in-One Quick Mode — Run all optimizations in seconds
📄 Detailed Report Generation — Full report saved to Desktop
🧹 Deep System Cleanup — Removes temp, cache, and prefetch files
💾 Disk Space Recovery — Disable hibernation to reclaim GBs
🌐 DNS Cache Flush — Fix network resolution issues
🗑️ Recycle Bin Cleaner — Free up disk space instantly
🔒 Admin Auto-Elevation — Automatically requests admin rights
🎨 Colorful CLI Interface — Clean, professional terminal UI
✅ Universal Compatibility — Works on Windows 7/8/10/11
🛡️ Safe Operations — Only removes junk files, never system files

🖥️ System Requirements
↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓
Requirement Details:
OS - Windows 7, 8, 8.1, 10, 11
Architecture - x86 / x64 / ARM64
Privileges - Administrator (auto-requested)
Dependencies - PowerShell 3.0+ (pre-installed on Windows 7+)
Disk Space - < 100 KB
RAM - Any

📥 Installation
Method 1: Direct Download
Download the MirrorX_Optimizer.bat file
Save it to any folder (e.g., C:\Tools\)
Right-click the file → Run as Administrator

Method 2: Clone from Repository
Bash
git clone https://github.com/yourusername/mirrorx-optimizer.git
cd mirrorx-optimizer
Then double-click MirrorX_Optimizer.bat.

🚀 Usage
Quick Start

text

1. Right-click MirrorX_Optimizer.bat
2. Select "Run as Administrator"
3. Choose an option from the menu (0-8)
4. Wait for completion

First-Time Recommendation

💡 Tip: For your first run, choose Option 2 (Full Optimize with Report) to see all the details of what was cleaned. After that, use Option 1 (All-in-One) for quick regular maintenance.

📋 Menu Options

text

==================================================
MirrorX PC Optimizer v1.0
==================================================

[1] All-in-One Quick Optimize (No Report)
[2] Full Optimize with Report on Desktop
[3] Clean Temporary Files Only
[4] Clean Cache Files Only
[5] Empty Recycle Bin Only
[6] Flush DNS Cache Only
[7] Disable Hibernation (Free Disk Space)
[8] Show System Memory & Disk Info
[0] Exit

==================================================
Detailed Option Breakdown

1 Runs all cleanup tasks in one click

2 Full cleanup + generates report on Desktop

3 Cleans only Windows/User temp folders

4 Clears cache, prefetch & thumbnail files

5 Empties the Recycle Bin

6 Flushes DNS resolver cache

7 Disables hibernation & deletes hiberfil.sys

8 Displays RAM and disk usage information

0 Exit the program

🔧 What Gets Cleaned

🗂️ Temporary Files
%TEMP% (User temp folder)
%SystemRoot%\Temp (Windows temp folder)
%USERPROFILE%\AppData\Local\Temp

🧠 Cache Files
Windows Update download cache (SoftwareDistribution\Download)
Prefetch files (Windows\Prefetch)
Explorer thumbnail cache (thumbcache\_\*.db)

💾 System Optimizations
Hibernation file removal (C:\hiberfil.sys)
Recycle Bin contents (all drives)
DNS resolver cache

🔄 Services Managed
Windows Update (wuauserv) — stopped temporarily during cleanup
Background Intelligent Transfer Service (bits) — restarted after cleanup

📊 Report File
When using Option 2, a detailed report is generated at:

text

C:\Users\<YourName>\Desktop\MirrorX_Report.txt
Sample Report Content
text

============================================
MirrorX PC Optimizer v1.0 - Report
============================================
Report Generated: 2025-01-15 14:32:10
Computer Name : DESKTOP-XYZ123
User : MirrorX
============================================

SECTION 1 - SYSTEM INFO (BEFORE)
Total RAM (MB) : 16384
Free RAM (MB) : 8192
Disk Usage:
Drive C: | Free: 120.45 GB | Total: 465.76 GB

...

OPTIMIZATION SUMMARY
[1] Temp Files - Cleaned
[2] Cache Files - Cleared
[3] Prefetch - Cleared
[4] Thumbnail Cache - Cleared
[5] Hibernation - Disabled
[6] Recycle Bin - Emptied
[7] DNS Cache - Flushed
[8] Services - Restarted

⚠️ Important Notes

🛡️ Safety First
MirrorX never touches your personal files, documents, or installed programs
It only removes temporary and cache files that Windows itself recreates automatically
Always run as Administrator for full functionality

💤 About Hibernation (Option 7)
Disabling hibernation frees space equal to your RAM size on C: drive
Desktop users: Safe to disable — hibernation is rarely needed
Laptop users: Consider keeping hibernation if you use it for battery saving
You can re-enable it anytime with: powercfg -h on

🔒 Antivirus Warning
Some antivirus software may flag .bat cleanup scripts as suspicious. This is a false positive. You can verify the script is safe by opening it in Notepad — all commands are visible and legitimate Windows utilities.

🐛 Troubleshooting

<details> <summary><b>❓ "Access Denied" errors during cleanup</b></summary>
Solution: Ensure you're running the script as Administrator. Right-click → Run as Administrator.

</details><details> <summary><b>❓ Script closes immediately after opening</b></summary>
Solution: Open Command Prompt as admin and manually run the script:

cmd

cd C:\Path\To\Script
MirrorX_Optimizer.bat

</details><details> <summary><b>❓ 'wmic' is not recognized error</b></summary>
Solution: This error is fixed in v1.0. If you're using an older version, download the latest release which uses PowerShell CIM commands.

</details><details> <summary><b>❓ Report file not created on Desktop</b></summary>
Solution: Check if you have write permissions to your Desktop folder, or if your Desktop is redirected to OneDrive.

</details><details> <summary><b>❓ Some files couldn't be deleted</b></summary>
Solution: This is normal — files currently in use by Windows cannot be deleted. Restart your PC and run the script again for maximum cleanup.

</details>
📈 Performance Impact
Metric	Typical Improvement
💾 Disk Space Freed	500 MB — 20 GB+
⚡ Boot Time	5–15% faster
🚀 App Launch Speed	Slightly improved
🌐 Network Resolution	Fixed DNS issues
Results vary based on system usage and time since last cleanup.

🗓️ Changelog
v1.0 — Current Release
✅ Initial stable release
✅ Interactive menu system with 8 options
✅ Replaced deprecated wmic with PowerShell CIM
✅ Windows 11 22H2+ compatibility
✅ All-in-One quick optimize mode
✅ Detailed report generation
✅ Hibernation management
✅ Auto-elevation to admin privileges

🛣️ Roadmap

• GUI version (PowerShell-based)
• Scheduled task auto-cleanup
• Browser cache cleanup (Chrome, Edge, Firefox)
• Windows Event Log cleanup
• Multi-language support
• Dark/Light theme toggle
• Custom cleanup profiles
• Backup before cleanup option

🤝 Contributing

Contributions are welcome! If you'd like to improve MirrorX:

Fork the repository

Create a feature branch (git checkout -b feature/AmazingFeature)

Commit your changes (git commit -m 'Add AmazingFeature')

Push to the branch (git push origin feature/AmazingFeature)

Open a Pull Request

📄 License
This project is licensed under the MIT License — see the LICENSE file for details.

text

MIT License - Free to use, modify, and distribute

👨‍💻 Author
MirrorX

📧 Email: mirrorxofficial.07@gmail.com

If MirrorX PC Optimizer helped speed up your PC:

⭐ Star this repository
🐛 Report bugs via Issues
💡 Suggest features for future releases
🔄 Share with friends and colleagues
❓ FAQ

Q: Is MirrorX safe to use?
A: Yes! It only removes temporary/cache files that Windows recreates automatically. No system files or personal data are touched.

Q: How often should I run it?
A: For active users — once a week. For casual users — once a month.

Q: Will it delete my downloads or documents?
A: No. MirrorX never touches user files, downloads, documents, or installed applications.

Q: Can I undo the changes?
A: Deleted temporary files cannot be recovered, but they're not needed. Hibernation can be re-enabled with powercfg -h on.

Q: Does it work on Windows Server?
A: It should work on Windows Server 2012 R2 and newer, but it's designed and tested primarily for desktop Windows.

Q: Why does it need admin privileges?
A: To clean protected system folders like Windows\Temp, Prefetch, and manage services.

<div align="center">
Made with ❤️ by MirrorX Team
⬆ Back to Top

</div>
