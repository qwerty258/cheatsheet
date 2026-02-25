Windows Environment Variables
=============================

User environment variables are stored in the registry key below:

```reg
HKEY_CURRENT_USER\Environment
```

System environment variables are stored in the registry key below:

```reg
HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Session Manager\Environment
```

|Environment Variables          |Values                                                                                                 |
|-------------------------------|-------------------------------------------------------------------------------------------------------|
|%ALLUSERSPROFILE%              |`C:\ProgramData`                                                                                       |
|%APPDATA%                      |`C:\Users\<user name>\AppData\Roaming`                                                                 |
|%CD%                           |(command prompt only) Current directory full path.                                                     |
|%CMDCMDLINE%                   |(command prompt only) Returns exact command line used to start current cmd.exe session.                |
|%CMDEXTVERSION%                |(command prompt only) Number of current command processor extensions.                                  |
|%COMPUTERNAME%                 |The computer name of the current local system.                                                         |
|%COMSPEC%                      |`C:\Windows\System32\cmd.exe`                                                                          |
|%CommonProgramFiles%           |`C:\Program Files\Common Files`                                                                        |
|%CommonProgramFiles(x86)%      |`C:\Program Files (x86)\Common Files`                                                                  |
|%CommonProgramW6432%           |`C:\Program Files\Common Files`                                                                        |
|%DATE%                         |(command prompt only) Current date in format determined by Date command.                               |
|%DriverData%                   |`C:\Windows\System32\Drivers\DriverData`                                                               |
|%ERRORLEVEL%                   |(command prompt only) Number defining exit status of previous command or program.                      |
|%HOMEDRIVE%                    |`C:`                                                                                                   |
|%HOMEPATH%                     |`\Users\<user name>`                                                                                   |
|%LOCALAPPDATA%                 |`C:\Users\<user name>\AppData\Local`                                                                   |
|%LOGONSERVER%                  |`\\MicrosoftAccount`                                                                                   |
|%NUMBER_OF_PROCESSORS%         |8                                                                                                      |
|%OS%                           |`Windows_NT`                                                                                           |
|%OneDrive%                     |Current OneDrive folder location.                                                                      |
|%PATH%                         |`C:\WINDOWS;C:\WINDOWS\system32;C:\WINDOWS\System32\Wbem;C:\WINDOWS\System32\WindowsPowerShell\v1.0`   |
|%PATHEXT%                      |`.COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC`                                                |
|%PROCESSOR_ARCHITECTURE%       |AMD64                                                                                                  |
|%PROCESSOR_IDENTIFIER%         |Intel64 Family 6 Model 60 Stepping 3, GenuineIntel                                                     |
|%PROCESSOR_LEVEL%              |6                                                                                                      |
|%PROCESSOR_REVISION%           |3c03                                                                                                   |
|%PROMPT%                       |(command prompt only) Code for current command prompt format. Code is usually `$P$G`.                  |
|%PSModulePath%                 |`C:\Windows\system32\WindowsPowerShell\v1.0\Modules\`                                                  |
|%PUBLIC%                       |`C:\Users\Public`                                                                                      |
|%ProgramData%                  |`C:\ProgramData`                                                                                       |
|%ProgramFiles%                 |`C:\Program Files`                                                                                     |
|%ProgramFiles(x86)%            |`C:\Program Files (x86)`                                                                               |
|%ProgramW6432%                 |`C:\Program Files`                                                                                     |
|%RANDOM%                       |(command prompt only) To get random number between 0 and 32767.                                        |
|%SessionName%                  |When logging on directly to machine, returns "Console". When client connects via terminal server session, is combination of connection name, followed by pound symbol {#} and session number.|
|%SystemDrive%                  |`C:`                                                                                                   |
|%SystemRoot%                   |`C:\Windows`                                                                                           |
|%TEMP%                         |`C:\Users\<user name>\AppData\Local\Temp`                                                              |
|%TIME%                         |(command prompt only) Current time in format determined by Time command.                               |
|%TMP%                          |`C:\Users\<user name>\AppData\Local\Temp`                                                              |
|%USERDOMAIN%                   |The network domain name associated with the current user.                                              |
|%USERDOMAIN_ROAMINGPROFILE%    |The network domain name associated with the current roaming profile.                                   |
|%USERNAME%                     |`<user name>`                                                                                          |
|%USERPROFILE%                  |`C:\Users\<user name>`                                                                                 |
|%WINDIR%                       |`C:\Windows`                                                                                           |
