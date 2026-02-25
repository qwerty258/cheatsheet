Windows Shell Commands
======================

A shell command can be typed in the Run (Windows+R) dialog, search, File Explorer address bar, and Internet Explorer address bar to open a Windows shell folder.

You can find the shell command listed in the Name string value data for each CLSID (GUID) key number at the registry location below.

```reg
HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\FolderDescriptions
```

You can create a shortcut with a shell command by adding `explorer` in front of the shell command or invoke in cmd directly.

For example:

```bat
explorer <shell:command>
```

|Shell Command                                      |Path                                                                                           |
|---------------------------------------------------|-----------------------------------------------------------------------------------------------|
|shell:3D Objects                                   |%UserProfile%\3D Objects                                                                       |
|shell:::{2559a1f3-21d7-11d4-bdaf-00c04f60b9f0}     |Run dialog box                                                                                 |
|shell:AccountPictures                              |%AppData%\Microsoft\Windows\AccountPictures                                                    |
|shell:AddNewProgramsFolder                         |Control Panel\All Control Panel Items\Get Programs                                             |
|shell:Administrative Tools                         |%AppData%\Microsoft\Windows\Start Menu\Programs\Administrative Tools (Windows 10)              |
|shell:Administrative Tools                         |%AppData%\Microsoft\Windows\Start Menu\Programs\Windows Tools (Windows 11)                     |
|shell:AppData                                      |%AppData%                                                                                      |
|shell:AppUpdatesFolder                             |Control Panel\All Control Panel Items\Programs and Features\Installed Updates (Windows 10)     |
|shell:AppUpdatesFolder                             |Installed Updates (Windows 11)                                                                 |
|shell:Application Shortcuts                        |%LocalAppData%\Microsoft\Windows\Application Shortcuts                                         |
|shell:AppsFolder                                   |applications                                                                                   |
|shell:CD Burning                                   |%LocalAppData%\Microsoft\Windows\Burn\Burn                                                     |
|shell:Cache                                        |%LocalAppData%\Microsoft\Windows\INetCache                                                     |
|shell:Camera Roll                                  |%UserProfile%\Pictures\Camera Roll                                                             |
|shell:CameraRollLibrary                            |Libraries\Camera Roll                                                                          |
|shell:Captures                                     |%UserProfile%\Videos\Captures                                                                  |
|shell:ChangeRemoveProgramsFolder                   |Control Panel\All Control Panel Items\Programs and Features                                    |
|shell:Common Administrative Tools                  |%ProgramData%\Microsoft\Windows\Start Menu\Programs\Administrative Tools (Windows 10)          |
|shell:Common Administrative Tools                  |%ProgramData%\Microsoft\Windows\Start Menu\Programs\Windows Tools (Windows 11)                 |
|shell:Common AppData                               |%ProgramData%                                                                                  |
|shell:Common Desktop                               |%Public%\Desktop                                                                               |
|shell:Common Documents                             |%Public%\Documents                                                                             |
|shell:Common Downloads                             |%Public%\Downloads                                                                             |
|shell:Common Music                                 |%Public%\Music                                                                                 |
|shell:Common Pictures                              |%Public%\Pictures                                                                              |
|shell:Common Programs                              |%ProgramData%\Microsoft\Windows\Start Menu\Programs                                            |
|shell:Common Ringtones                             |%ProgramData%\Microsoft\Windows\Ringtones                                                      |
|shell:Common Start Menu                            |%ProgramData%\Microsoft\Windows\Start Menu                                                     |
|shell:Common Startup                               |%ProgramData%\Microsoft\Windows\Start Menu\Programs\Startup                                    |
|shell:Common Templates                             |%ProgramData%\Microsoft\Windows\Templates                                                      |
|shell:Common Video                                 |%Public%\Videos                                                                                |
|shell:CommonDownloads                              |%Public%\Downloads                                                                             |
|shell:CommonMusic                                  |%Public%\Music                                                                                 |
|shell:CommonPictures                               |%Public%\Pictures                                                                              |
|shell:CommonRingtones                              |%ProgramData%\Microsoft\Windows\Ringtones                                                      |
|shell:CommonVideo                                  |%Public%\Videos                                                                                |
|shell:ConflictFolder                               |Control Panel\All Control Panel Items\Sync Center\Conflicts                                    |
|shell:ConnectionsFolder                            |Control Panel\All Control Panel Items\Network Connections                                      |
|shell:Contacts                                     |%UserProfile%\Contacts                                                                         |
|shell:ControlPanelFolder                           |Control Panel\All Control Panel Items                                                          |
|shell:Cookies                                      |%LocalAppData%\Microsoft\Windows\INetCookies                                                   |
|shell:Cookies\low                                  |%LocalAppData%\Microsoft\Windows\INetCookies\low                                               |
|shell:CredentialManager                            |%AppData%\Microsoft\Credentials                                                                |
|shell:CryptoKeys                                   |%AppData%\Microsoft\Crypto                                                                     |
|shell:Desktop                                      |Desktop                                                                                        |
|shell:Device Metadata Store                        |%ProgramData%\Microsoft\Windows\DeviceMetadataStore                                            |
|shell:DocumentsLibrary                             |Libraries\Documents                                                                            |
|shell:Downloads                                    |%UserProfile%\Downloads                                                                        |
|shell:Favorites                                    |%UserProfile%\Favorites                                                                        |
|shell:Fonts                                        |%WinDir%\Fonts                                                                                 |
|shell:GameTasks                                    |%LocalAppData%\Microsoft\Windows\GameExplorer                                                  |
|shell:Games                                        |Games (removed in version 1803)                                                                |
|shell:History                                      |%LocalAppData%\Microsoft\Windows\History                                                       |
|shell:HomeGroupCurrentUserFolder                   |Homegroup\(user-name)                                                                          |
|shell:HomeGroupFolder                              |Homegroup                                                                                      |
|shell:ImplicitAppShortcuts                         |%AppData%\Microsoft\Internet Explorer\Quick Launch\User Pinned\ImplicitAppShortcuts            |
|shell:InternetFolder                               |Internet Explorer                                                                              |
|shell:Libraries                                    |Libraries                                                                                      |
|shell:Links                                        |%UserProfile%\Links                                                                            |
|shell:Local AppData                                |%LocalAppData%                                                                                 |
|shell:Local Documents                              |This PC > Documents                                                                            |
|shell:Local Downloads                              |This PC > Downloads                                                                            |
|shell:Local Music                                  |This PC > Music                                                                                |
|shell:Local Pictures                               |This PC > Pictures                                                                             |
|shell:Local Videos                                 |This PC > Videos                                                                               |
|shell:LocalAppDataLow                              |%UserProfile%\AppData\LocalLow                                                                 |
|shell:MusicLibrary                                 |Libraries\Music                                                                                |
|shell:My Music                                     |%UserProfile%\Music                                                                            |
|shell:My Pictures                                  |%UserProfile%\Pictures                                                                         |
|shell:My Video                                     |%UserProfile%\Videos                                                                           |
|shell:MyComputerFolder                             |This PC                                                                                        |
|shell:NetHood                                      |%AppData%\Microsoft\Windows\Network Shortcuts                                                  |
|shell:NetworkPlacesFolder                          |Network                                                                                        |
|shell:OneDrive                                     |OneDrive                                                                                       |
|shell:OneDriveCameraRoll                           |%UserProfile%\OneDrive\Pictures\Camera Roll                                                    |
|shell:OneDriveDocuments                            |%UserProfile%\OneDrive\Documents                                                               |
|shell:OneDriveMusic                                |%UserProfile%\OneDrive\Music                                                                   |
|shell:OneDrivePictures                             |%UserProfile%\OneDrive\Pictures                                                                |
|shell:Personal                                     |%UserProfile%\Documents                                                                        |
|shell:PicturesLibrary                              |Libraries\Pictures                                                                             |
|shell:PrintHood                                    |%AppData%\Microsoft\Windows\Printer Shortcuts                                                  |
|shell:PrintersFolder                               |All Control Panel Items\Printers                                                               |
|shell:Profile                                      |%UserProfile%                                                                                  |
|shell:ProgramFiles                                 |%ProgramFiles%                                                                                 |
|shell:ProgramFilesCommon                           |%ProgramFiles%\Common Files                                                                    |
|shell:ProgramFilesCommonX64                        |%ProgramFiles%\Common Files (64-bit Windows only)                                              |
|shell:ProgramFilesCommonX86                        |%ProgramFiles(x86)%\Common Files (64-bit Windows only)                                         |
|shell:ProgramFilesX64                              |%ProgramFiles% (64-bit Windows only)                                                           |
|shell:ProgramFilesX86                              |%ProgramFiles(x86)% (64-bit Windows only)                                                      |
|shell:Programs                                     |%AppData%\Microsoft\Windows\Start Menu\Programs                                                |
|shell:Public                                       |%Public%                                                                                       |
|shell:PublicAccountPictures                        |%Public%\AccountPictures                                                                       |
|shell:PublicGameTasks                              |%ProgramData%\Microsoft\Windows\GameExplorer                                                   |
|shell:PublicLibraries                              |%Public%\Libraries                                                                             |
|shell:Quick Launch                                 |%AppData%\Microsoft\Internet Explorer\Quick Launch                                             |
|shell:Recent                                       |%AppData%\Microsoft\Windows\Recent                                                             |
|shell:RecordedTVLibrary                            |Libraries\Recorded TV                                                                          |
|shell:RecycleBinFolder                             |Recycle Bin                                                                                    |
|shell:ResourceDir                                  |%WinDir%\Resources                                                                             |
|shell:Retail Demo                                  |%ProgramData%\Microsoft\Windows\RetailDemo                                                     |
|shell:Ringtones                                    |%ProgramData%\Microsoft\Windows\Ringtones                                                      |
|shell:Roamed Tile Images                           |%LocalAppData%\Microsoft\Windows\RoamedTileImages                                              |
|shell:Roaming Tiles                                |%AppData%\Microsoft\Windows\RoamingTiles                                                       |
|shell:SavedGames                                   |%UserProfile%\Saved Games                                                                      |
|shell:SavedPictures                                |%UserProfile%\Pictures\Saved Pictures                                                          |
|shell:SavedPicturesLibrary                         |Libraries\Saved Pictures                                                                       |
|shell:Screenshots                                  |%UserProfile%\Pictures\Screenshots                                                             |
|shell:SearchHistoryFolder                          |%LocalAppData%\Microsoft\Windows\ConnectedSearch\History                                       |
|shell:SearchHomeFolder                             |search-ms:                                                                                     |
|shell:SearchTemplatesFolder                        |%LocalAppData%\Microsoft\Windows\ConnectedSearch\Templates                                     |
|shell:Searches                                     |%UserProfile%\Searches                                                                         |
|shell:SendTo                                       |%AppData%\Microsoft\Windows\SendTo                                                             |
|shell:Start Menu                                   |%AppData%\Microsoft\Windows\Start Menu                                                         |
|shell:StartMenuAllPrograms                         |StartMenuAllPrograms                                                                           |
|shell:Startup                                      |%AppData%\Microsoft\Windows\Start Menu\Programs\Startup                                        |
|shell:SyncCenterFolder                             |Control Panel\All Control Panel Items\Sync Center                                              |
|shell:SyncResultsFolder                            |Control Panel\All Control Panel Items\Sync Center\Sync Results                                 |
|shell:SyncSetupFolder                              |Control Panel\All Control Panel Items\Sync Center\Sync Setup                                   |
|shell:System                                       |%WinDir%\System32                                                                              |
|shell:SystemCertificates                           |%AppData%\Microsoft\SystemCertificates                                                         |
|shell:SystemX86                                    |%WinDir%\SysWOW64                                                                              |
|shell:Templates                                    |%AppData%\Microsoft\Windows\Templates                                                          |
|shell:ThisDeviceFolder                             |This Device                                                                                    |
|shell:ThisPCDesktopFolder                          |Desktop                                                                                        |
|shell:ThisPCDesktopFolder                          |This PC > Desktop                                                                              |
|shell:User Pinned                                  |%AppData%\Microsoft\Internet Explorer\Quick Launch\User Pinned                                 |
|shell:UserProfiles                                 |%HomeDrive%\Users                                                                              |
|shell:UserProgramFiles                             |%LocalAppData%\Programs                                                                        |
|shell:UserProgramFilesCommon                       |%LocalAppData%\Programs\Common                                                                 |
|shell:UsersFilesFolder                             |%UserProfile%                                                                                  |
|shell:UsersLibrariesFolder                         |Libraries                                                                                      |
|shell:VideosLibrary                                |Libraries\Videos                                                                               |
|shell:Windows                                      |%WinDir%                                                                                       |
|shell:Windows                                      |%WinDir%                                                                                       |
|shell:desktop                                      |Desktop                                                                                        |
|shell:device Metadata Store                        |%ProgramData%\Microsoft\Windows\DeviceMetadataStore                                            |
|shell:documentsLibrary                             |Libraries\Documents                                                                            |
|shell:downloads                                    |%UserProfile%\Downloads                                                                        |
|shell:dpapiKeys                                    |%AppData%\Microsoft\Protect                                                                    |

A CLSID is a globally unique identifier that identifies a COM class object.

```bat
explorer shell:::{CLSID key}
explorer /e,::{CLSID key}
```

|CLSID key (GUID)                                                                   |Opens|
|-----------------------------------------------------------------------------------|---|
|{018D5C66-4533-4307-9B53-224DE2ED1FE6}                                             |OneDrive|
|{025A5937-A6BE-4686-A844-36FE4BEC8B6D}                                             |Power Options|
|{025A5937-A6BE-4686-A844-36FE4BEC8B6D}\pageCreateNewPlan                           |Create a power plan|
|{025A5937-A6BE-4686-A844-36FE4BEC8B6D}\pageGlobalSettings                          |System Settings|
|{025A5937-A6BE-4686-A844-36FE4BEC8B6D}\pagePlanSettings                            |Edit Plan Settings|
|{031E4825-7B94-4DC3-B131-E946B44C8DD5}                                             |Libraries|
|{05D7B0F4-2121-4EFF-BF6B-ED3F69B894D9}                                             |Notification Area Icons|
|{05D7B0F4-2121-4EFF-BF6B-ED3F69B894D9}\SystemIcons                                 |System Icons|
|{088E3905-0323-4B02-9826-5D99428E115F}                                             |Downloads (folder)|
|{0907616E-F5E6-48D8-9D61-A91C3D28106D}                                             |Hyper-V Remote File Browsing|
|{0BBCA823-E77D-419E-9A44-5ADEC2C8EEB0}                                             |NVIDIA Control Panel (if installed)|
|{0DB7E03F-FC29-4DC6-9020-FF41B59E513A}                                             |3D Objects (folder)|
|{0DF44EAA-FF21-4412-828E-260A8728E7F1}                                             |Taskbar and Navigation properties|
|{0DF44EAA-FF21-4412-828E-260A8728E7F1}                                             |Taskbar page in Settings|
|{1206F5F1-0569-412C-8FEC-3204630DFB70}                                             |Credential Manager|
|{15EAE92E-F17A-4431-9F28-805E482DAFD4}                                             |Get Programs|
|{17CD9488-1228-4B2F-88CE-4298E93E0966}                                             |Default Programs|
|{17CD9488-1228-4B2F-88CE-4298E93E0966}\pageDefaultProgram                          |Default Apps page in Settings|
|{17CD9488-1228-4B2F-88CE-4298E93E0966}\pageFileAssoc                               |Default Apps page in Settings|
|{1CF1260C-4DD0-4EBB-811F-33C572699FDE}                                             |Music (folder)|
|{1F3427C8-5C10-4210-AA03-2EE45287D668}                                             |User Pinned|
|{208D2C60-3AEA-1069-A2D7-08002B30309D}                                             |Network (WorkGroup)|
|{20D04FE0-3AEA-1069-A2D8-08002B30309D}                                             |This PC|
|{21EC2020-3AEA-1069-A2DD-08002B30309D}                                             |Control Panel (always Icons view)|
|{2227A280-3AEA-1069-A2DE-08002B30309D}                                             |Printers|
|{22877A6D-37A1-461A-91B0-DBDA5AAEBC99}                                             |Recent folders|
|{241D7C96-F8BF-4F85-B01F-E2B043341A4B}                                             |RemoteApp and Desktop Connections|
|{241D7C96-F8BF-4F85-B01F-E2B043341A4B}\PropertiesPage                              |Connection Properties|
|{24AD3AD4-A569-4530-98E1-AB02F9417AA8}                                             |Local Pictures|
|{2559A1F1-21D7-11D4-BDAF-00C04F60B9F0}                                             |Help and Support|
|{2559A1F3-21D7-11D4-BDAF-00C04F60B9F0}                                             |Run|
|{2559A1F5-21D7-11D4-BDAF-00C04F60B9F0}                                             |E-mail (default e-mail program)|
|{2559A1F7-21D7-11D4-BDAF-00C04F60B9F0}                                             |Set Program Access and Computer Defaults|
|{2559A1F8-21D7-11D4-BDAF-00C04F60B9F0}                                             |Search (Windows)|
|{26EE0668-A00A-44D7-9371-BEB064C98683}                                             |Control Panel (always Category view)|
|{26EE0668-A00A-44D7-9371-BEB064C98683}\1                                           |Appearance and Personalization|
|{26EE0668-A00A-44D7-9371-BEB064C98683}\2                                           |Hardware and Sound|
|{26EE0668-A00A-44D7-9371-BEB064C98683}\3                                           |Network and Internet|
|{26EE0668-A00A-44D7-9371-BEB064C98683}\5                                           |System and Security|
|{26EE0668-A00A-44D7-9371-BEB064C98683}\6                                           |Clock and Region|
|{26EE0668-A00A-44D7-9371-BEB064C98683}\7                                           |Ease of Access|
|{26EE0668-A00A-44D7-9371-BEB064C98683}\8                                           |Programs|
|{26EE0668-A00A-44D7-9371-BEB064C98683}\9                                           |User Accounts|
|{26EE0668-A00A-44D7-9371-BEB064C98683}\10                                          |System and Security|
|{28803F59-3A75-4058-995F-4EE5503B023C}                                             |Bluetooth Devices|
|{289AF617-1CC3-42A6-926C-E6A863F0E3BA}                                             |Media Servers|
|{2965E715-EB66-4719-B53F-1672673BBEFA}                                             |Results Folder|
|{2E9E59C0-B437-4981-A647-9C34B9B90891}                                             |Sync Setup Folder|
|{3080F90D-D7AD-11D9-BD98-0000947B0257}                                             |Show Desktop|
|{3080F90E-D7AD-11D9-BD98-0000947B0257}                                             |Task View|
|{323CA680-C24D-4099-B94D-446DD2D7249E}                                             |Favorites|
|{35786D3C-B075-49B9-88DD-029876E11C01}                                             |Portable Devices|
|{374DE290-123F-4565-9164-39C4925E467B}                                             |Downloads (folder)|
|{3936E9E4-D92C-4EEE-A85A-BC16D5EA0819}                                             |Frequent folders|
|{3ADD1653-EB32-4CB0-BBD7-DFA0ABB5ACCA}                                             |Pictures (folder)|
|{3DFDF296-DBEC-4FB4-81D1-6A3438BCF4DE}                                             |Music (folder)|
|{3F6BC534-DFA1-4AB4-AE54-EF25A74E0107}                                             |System Restore|
|{4026492F-2F69-46B8-B9BF-5654FC07E423}                                             |Windows Defender Firewall|
|{4026492F-2F69-46B8-B9BF-5654FC07E423}\PageConfigureSettings                       |Customize Settings|
|{4026492F-2F69-46B8-B9BF-5654FC07E423}\PageRestoreDefaults                         |Restore defaults|
|{4026492F-2F69-46B8-B9BF-5654FC07E423}\pageConfigureApps                           |Allowed apps|
|{40419485-C444-4567-851A-2DD7BFA1684D}                                             |Location Information (Phone and Modem Control Panel)|
|{4234D49B-0245-4DF3-B780-3893943456E1}                                             |Applications|
|{4336A54D-038B-4685-AB02-99BB52D3FB8B}                                             |Public (folder)|
|{437FF9C0-A07F-4FA0-AF80-84B6C6440A16}                                             |Command Folder|
|{450D8FBA-AD25-11D0-98A8-0800361B1103}                                             |My Documents|
|{4564B25E-30CD-4787-82BA-39E73A750B14}                                             |Recent Items Instance Folder|
|{5399E694-6CE5-4D6C-8FCE-1D8870FDCBA0}                                             |Control Panel|
|{58E3C745-D971-4081-9034-86E34B30836A}                                             |Speech Recognition|
|{59031A47-3F72-44A7-89C5-5595FE6B30EE}                                             |%UserProfile%|
|{5B934B42-522B-4C34-BBFE-37A3EF7B9C90}                                             |This Device|
|{5EA4F148-308C-46D7-98A9-49041B1DD468}                                             |Windows Mobility Center|
|{60632754-C523-4B62-B45C-4172DA012619}                                             |User Accounts|
|{60632754-C523-4B62-B45C-4172DA012619}\pageAdminTasks                              |Manage Accounts|
|{60632754-C523-4B62-B45C-4172DA012619}\pageRenameMyAccount                         |Change Your Name|
|{62D8ED13-C9D0-4CE8-A914-47DD628FB1B0}                                             |Region|
|{645FF040-5081-101B-9F08-00AA002F954E}                                             |Recycle Bin|
|{67718415-C450-4F3C-BF8A-B487642DC39B}                                             |Windows Features|
|{679F85CB-0220-4080-B29B-5540CC05AAB6}                                             |Quick access|
|{6C8EEC18-8D75-41B2-A177-8831D59D2D50}                                             |Mouse Properties|
|{6DFD7C5C-2451-11D3-A299-00C04F8EF6AF}                                             |File Explorer Options|
|{6DFD7C5C-2451-11D3-A299-00C04F8EF6AF}                                             |Folder Options|
|{7007ACC7-3202-11D1-AAD2-00805FC1270E}                                             |Network Connections|
|{725BE8F7-668E-4C7B-8F90-46BDB0936430}                                             |Keyboard Properties|
|{74246BFC-4C96-11D0-ABEF-0020AF6B0B7A}                                             |Device Manager|
|{7A9D77BD-5403-11D2-8785-2E0420524153}                                             |User Accounts (netplwiz)|
|{7A9D77BD-5403-11D2-8785-2E0420524153}                                             |netplwiz|
|{7B81BE6A-CE2B-4676-A29E-EB907A5126C5}                                             |Programs and Features|
|{80F3F1D5-FECA-45F3-BC32-752C152E456E}                                             |Tablet PC Settings|
|{863AA9FD-42DF-457B-8E4D-0DE1B8015C60}                                             |Printers|
|{863AA9FD-42DF-457B-8E4D-0DE1B8015C60}                                             |Remote Printers|
|{871C5380-42A0-1069-A2EA-08002B30309D}                                             |Web browser (default)|
|{87D66A43-7B11-4A28-9811-C86EE395ACF7}                                             |Indexing Options|
|{8E0C279D-0BD1-43C3-9EBD-31C3DC5B8A77}                                             |Windows To Go|
|{8E908FC9-BECC-40F6-915B-F4CA0E70D03D}                                             |Network and Sharing Center|
|{8E908FC9-BECC-40F6-915B-F4CA0E70D03D}\Advanced                                    |Advanced sharing settings|
|{8E908FC9-BECC-40F6-915B-F4CA0E70D03D}\ShareMedia                                  |Media streaming options|
|{93412589-74D4-4E4E-AD0E-E0CB621440FD}                                             |Font Settings|
|{9343812E-1C37-4A49-A12E-4B2D810D956B}                                             |Search (File Explorer)|
|{992CFFA0-F557-101A-88EC-00DD010CCC48}                                             |Network Connections|
|{9C60DE1E-E5FC-40F4-A487-460851A8D915}                                             |AutoPlay|
|{9C73F5E5-7AE7-4E32-A8E8-8D23B85255BF}                                             |Sync Center|
|{9C73F5E5-7AE7-4E32-A8E8-8D23B85255BF}\::{F1390A9A-A3F4-4E5D-9C5F-98F3BD8D935C}    |Sync Setup|
|{9FE63AFD-59CF-4419-9775-ABCC3849F861}                                             |Recovery|
|{A0275511-0E86-4ECA-97C2-ECD8F1221D08}                                             |Infared (if installed)|
|{A0953C92-50DC-43BF-BE83-3742FED03C9C}                                             |Videos (folder)|
|{A3DD4F92-658A-410F-84FD-6FBBBEF2FFFE}                                             |Internet Options (Internet Explorer)|
|{A6482830-08EB-41E2-84C1-73920C2BADB9}                                             |Removable Storage Devices|
|{A8A91A66-3A7D-4424-8D24-04E180695C7A}                                             |Devices and Printers|
|{A8CDFF1C-4878-43BE-B5FD-F8091C1C60D0}                                             |Documents (folder)|
|{AFDB1F70-2A4C-11D2-9039-00C04F8EEB3E}                                             |Offline Files Folder|
|{B155BDF8-02F0-451E-9A26-AE317CFD7779}                                             |delegate folder that appears in Computer|
|{B2C761C6-29BC-4F19-9251-E6195265BAF1}                                             |Color Management|
|{B4BFCC3A-DB2C-424C-B029-7FE99A87C641}                                             |Desktop (folder)|
|{B98A2BEA-7D42-4558-8BD1-832F41BAC6FD}                                             |Backup and Restore (Windows 7)|
|{BB06C0E4-D293-4F75-8A90-CB05B6477EEE}                                             |System|
|{BB64F8A7-BEE7-4E1A-AB8D-7D8273F7FDB6}                                             |Security and Maintenance|
|{BB64F8A7-BEE7-4E1A-AB8D-7D8273F7FDB6}\Settings                                    |Change Security and Maintenance settings|
|{BB64F8A7-BEE7-4E1A-AB8D-7D8273F7FDB6}\pageAdvSettings                             |Advanced Problem Reporting Settings|
|{BB64F8A7-BEE7-4E1A-AB8D-7D8273F7FDB6}\pageProblems                                |Problem Reports|
|{BB64F8A7-BEE7-4E1A-AB8D-7D8273F7FDB6}\pageReliabilityView                         |Reliability Monitor|
|{BB64F8A7-BEE7-4E1A-AB8D-7D8273F7FDB6}\pageReliabilityView                         |Reliability Monitor|
|{BB64F8A7-BEE7-4E1A-AB8D-7D8273F7FDB6}\pageReportDetails                           |Problem Details|
|{BB64F8A7-BEE7-4E1A-AB8D-7D8273F7FDB6}\pageSettings                                |Problem Reporting Settings|
|{BB64F8A7-BEE7-4E1A-AB8D-7D8273F7FDB6}\pageSettings                                |Problem Reporting Settings|
|{BD84B380-8CA2-1069-AB1D-08000948F534}                                             |Fonts (folder)|
|{C58C4893-3BE0-4B45-ABB5-A63E4B8C8651}                                             |Troubleshooting|
|{C58C4893-3BE0-4B45-ABB5-A63E4B8C8651}\applications                                |Troubleshoot problems - Programs|
|{C58C4893-3BE0-4B45-ABB5-A63E4B8C8651}\devices                                     |Troubleshoot problems - Hardware and Sound|
|{C58C4893-3BE0-4B45-ABB5-A63E4B8C8651}\historyPage                                 |History|
|{C58C4893-3BE0-4B45-ABB5-A63E4B8C8651}\listAllPage                                 |All Categories|
|{C58C4893-3BE0-4B45-ABB5-A63E4B8C8651}\network                                     |Troubleshoot problems - Network and Internet|
|{C58C4893-3BE0-4B45-ABB5-A63E4B8C8651}\raPage                                      |Remote Assistance|
|{C58C4893-3BE0-4B45-ABB5-A63E4B8C8651}\resultPage                                  |Additional Information|
|{C58C4893-3BE0-4B45-ABB5-A63E4B8C8651}\searchPage                                  |Search Troubleshooting|
|{C58C4893-3BE0-4B45-ABB5-A63E4B8C8651}\settingPage                                 |Change Settings|
|{C58C4893-3BE0-4B45-ABB5-A63E4B8C8651}\system                                      |Troubleshoot problems - System and Security|
|{D17D1D6D-CC3F-4815-8FE3-607E7D5D10B3}                                             |Text to Speech|
|{D20EA4E1-3957-11D2-A40B-0C5020524153}                                             |Administrative Tools|
|{D3162B92-9365-467A-956B-92703ACA08AF}                                             |Documents (folder)|
|{D34A6CA6-62C2-4C34-8A7C-14709C1AD938}                                             |Common Places FS Folder|
|{D4480A50-BA28-11D1-8E75-00C04FA31A86}                                             |Add Network Location|
|{D450A8A1-9568-45C7-9C0E-B4F9FB4537BD}                                             |Installed Updates|
|{D555645E-D4F8-4C29-A827-D93C859C4F2A}                                             |Ease of Access Center|
|{D555645E-D4F8-4C29-A827-D93C859C4F2A}\pageEasierToClick                           |Make the mouse easier to use|
|{D555645E-D4F8-4C29-A827-D93C859C4F2A}\pageEasierToReadAndWrite                    |Make it easier to focus on tasks|
|{D555645E-D4F8-4C29-A827-D93C859C4F2A}\pageEasierToSee                             |Make the computer easier to see|
|{D555645E-D4F8-4C29-A827-D93C859C4F2A}\pageEasierWithSounds                        |Use text or visual alternatives for sounds|
|{D555645E-D4F8-4C29-A827-D93C859C4F2A}\pageFilterKeysSettings                      |Set up Filter Keys|
|{D555645E-D4F8-4C29-A827-D93C859C4F2A}\pageKeyboardEasierToUse                     |Make the keyboard easier to use|
|{D555645E-D4F8-4C29-A827-D93C859C4F2A}\pageMouseKeysSettings                       |Set up Mouse Keys|
|{D555645E-D4F8-4C29-A827-D93C859C4F2A}\pageNoMouseOrKeyboard                       |Use the computer without a mouse or keyboard|
|{D555645E-D4F8-4C29-A827-D93C859C4F2A}\pageNoVisual                                |Use the computer without a display|
|{D555645E-D4F8-4C29-A827-D93C859C4F2A}\pageQuestionsCognitive                      |Get recommendations to make your computer easier to use (cognitive)|
|{D555645E-D4F8-4C29-A827-D93C859C4F2A}\pageQuestionsEyesight                       |Get recommendations to make your computer easier to use (eyesight)|
|{D555645E-D4F8-4C29-A827-D93C859C4F2A}\pageRepeatRateSlowKeysSettings              |Set up Repeat and Slow Keys|
|{D555645E-D4F8-4C29-A827-D93C859C4F2A}\pageStickyKeysSettings                      |Set up Sticky Keys|
|{D9EF8727-CAC2-4E60-809E-86F80A666C91}                                             |BitLocker Drive Encryption|
|{E2E7934B-DCE5-43C4-9576-7FE4F75E7480}                                             |Date and Time|
|{E342F0FE-FF1C-4C41-BE37-A0271FC90396}                                             |Intel Rapid Storage Technology (if installed)|
|{E9950154-C418-419E-A90A-20C5287AE24B}                                             |Location Settings|
|{ECDB0924-4208-451E-8EE0-373C0956DE16}                                             |Work Folders|
|{ED228FDF-9EA8-4870-83B1-96B02CFE0D52}                                             |Games Explorer|
|{ED50FC29-B964-48A9-AFB3-15EBB9B97F36}                                             |printhood delegate folder|
|{ED7BA470-8E54-465E-825C-99712043E01C}                                             |Control Panel (All Tasks)|
|{ED834ED6-4B5A-4BFE-8F11-A626DCB6A921}                                             |Personalization|
|{ED834ED6-4B5A-4BFE-8F11-A626DCB6A921}\pageColorization                            |Color and Appearance|
|{ED834ED6-4B5A-4BFE-8F11-A626DCB6A921}\pageWallpaper                               |Desktop Background|
|{F02C1A0D-BE21-4350-88B0-7367FC96EF3C}                                             |Network|
|{F2DDFC82-8F12-4CDD-B7DC-D4FE1425AA4D}                                             |Sound|
|{F5FB2C77-0E2F-4A16-A381-3E560C68BC83}                                             |Removable Drives|
|{F6B6E965-E9B2-444B-9286-10C9152EDBC5}                                             |File History|
|{F82DF8F7-8B9F-442E-A48C-818EA735FF9B}                                             |Pen and Touch|
|{F86FA3AB-70D2-4FC7-9C99-FCBF05467F3A}                                             |Videos (folder)|
|{F8C2AB3B-17BC-41DA-9758-339D7DBF2D88}                                             |Previous Versions Results Folder|
|{F942C606-0914-47AB-BE56-1321B8035096}                                             |Storage Spaces|
