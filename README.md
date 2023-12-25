# VirusTotal Console Checker

It is free-to-use CMD-wrapper over official VirusTotal console utility intended for convenient and fast check the selected file on VirusTotal through context menu.

It can upload file for checking and display:
 - Engine names and its detection
 - Database & engine version 
 - Detailed log (on demand)

It supports both viewing an already verified file and uploading a new one to VT.

![ScreenShot](https://github.com/SafeZone-cc/Virustotal-Console-Checker/assets/19956568/1aa210bb-f17c-4152-bd25-7c6ea7835611)

**Usage:**
 - Press right mouse click on desired file => Choose "Send" * => VT_Con_Checker
 - Console will show you the names of engines, detections and overall statistics.
 - By clicking on button 1, a log with a more detailed analysis will open.
 - Also, this wrapper may be very handy for **Developers** to implement in their building system as a last stage, e.g. call cmd.exe /c "VT_Con_Checker.cmd "file"" as post-build script for the automatic check on VT.
 
**Note:** if you own Windows 11, you'll have to select "Show additional parameters" or apply a [special tweak](https://www.safezone.cc/threads/tvik-na-raskrytie-polnogo-kontekstnogo-menju.42190/post-323101).

**Note 2:** when you launch it for the first time, you'll be asked for an API key; you can obtain it by [registering](https://www.virustotal.com/gui/join-us) on virustotal.com. Next, log into your VirusTotal account, and in the upper right corner, click on your name => **API Key**, copy the 64-character value and paste it into the console, then press ENTER. This will only need to be done once.

**Installation:**
 - Download the archive, unpack it to a convenient place that you will not touch, for instance, in C:\tools\vt_checker\
 - Place the vt.exe file in the same folder (it is open-sourced [vt-cli utility by VirusTotal](https://support.virustotal.com/hc/en-us/articles/360002160598-Does-VirusTotal-have-a-command-line-tool-)). It can be found in the archive of [releases page](https://github.com/VirusTotal/vt-cli/releases) (**Windows64.zip** - for 64-bit OS, or **Windows32.zip** for 32-bit OS).
 - Create a shortcut to the file **VT_Con_Checker.cmd** and put this shortcut in the Shell:SendTo folder, which you'll find as follows: press **Win + R** and enter:
```
explorer Shell:Sendto
```
 - click ok; A folder should open where you need to put the shortcut.