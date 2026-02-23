windows user shell folders
==========================

reference: https://www.winhelponline.com/blog/windows-10-shell-folders-paths-defaults-restore

# current user account

```reg
HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\User Shell Folders
```

|Shell Folder Name (Value type: REG_EXPAND_SZ)  |Location                                                                       |
|-----------------------------------------------|-------------------------------------------------------------------------------|
|{374DE290-123F-4565-9164-39C4925E467B}         |%USERPROFILE%\Downloads                                                        |
|AppData                                        |%USERPROFILE%\AppData\Roaming                                                  |
|Cache                                          |%USERPROFILE%\AppData\Local\Microsoft\Windows\INetCache                        |
|Cookies                                        |%USERPROFILE%\AppData\Local\Microsoft\Windows\INetCookies                      |
|Desktop                                        |%USERPROFILE%\Desktop                                                          |
|Favorites                                      |%USERPROFILE%\Favorites                                                        |
|History                                        |%USERPROFILE%\AppData\Local\Microsoft\Windows\History                          |
|Local AppData                                  |%USERPROFILE%\AppData\Local                                                    |
|My Music                                       |%USERPROFILE%\Music                                                            |
|My Pictures                                    |%USERPROFILE%\Pictures                                                         |
|My Video                                       |%USERPROFILE%\Videos                                                           |
|NetHood                                        |%USERPROFILE%\AppData\Roaming\Microsoft\Windows\Network Shortcuts              |
|Personal                                       |%USERPROFILE%\Documents                                                        |
|PrintHood                                      |%USERPROFILE%\AppData\Roaming\Microsoft\Windows\Printer Shortcuts              |
|Programs                                       |%USERPROFILE%\AppData\Roaming\Microsoft\Windows\Start Menu\Programs            |
|Recent                                         |%USERPROFILE%\AppData\Roaming\Microsoft\Windows\Recent                         |
|SendTo                                         |%USERPROFILE%\AppData\Roaming\Microsoft\Windows\SendTo                         |
|Start Menu                                     |%USERPROFILE%\AppData\Roaming\Microsoft\Windows\Start Menu                     |
|Startup                                        |%USERPROFILE%\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup    |
|Templates                                      |%USERPROFILE%\AppData\Roaming\Microsoft\Windows\Templates                      |

 - `{374DE290-123F-4565-9164-39C4925E467B}` represents the Downloads folder.

Overriding registry values

The following items do not exist in a clean install of Windows 10 and Windows 11. They're created only if you redirect those folders to Microsoft OneDrive or DropBox. If the following values exist, the location defined in the following values takes precedence. In case of any conflict, the following values can be deleted so that the defaults (above) are used.

|Value Name (Overrides)                 |Shell folder whose path is Overridden  |
|---------------------------------------|---------------------------------------|
|{3B193882-D3AD-4EAB-965A-69829D1FB59F} |Saved Pictures                         |
|{AB5FB87B-7CE2-4F83-915D-550846C9537B} |Camera Roll                            |
|{B7BEDE81-DF94-4682-A7D8-57A52620B86F} |Screenshots                            |
|{F42EE2D3-909F-4907-8871-4C22FC0BF756} |Local Documents                        |
|{7D83EE9B-2244-4E70-B1F5-5393042AF1E4} |Local Downloads                        |
|{A0C69A99-21C8-4671-8703-7934162FCF1D} |Local Music                            |
|{0DDD015D-B06C-45D5-8C4C-F59713854639} |Local Pictures                         |
|{35286A68-3C57-41A1-BBB1-0EAE73D76C95} |Local Videos                           |
|{24D89E24-2F19-4534-9DDE-6A6671FBB8FE} |OneDrive Documents                     |
|{767E6811-49CB-4273-87C2-20F355E1085B} |OneDrive Camera Roll                   |
|{31C0DD25-9439-4F12-BF41-7FF4EDA38722} |3D Objects                             |
|{754AC886-DF64-4CBA-86B5-F7FBF4FBCEF5} |Desktop                                |

# common special folder (applicable for all users)

```reg
HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\User Shell Folders
```

|Shell Folder Name (Value type: REG_EXPAND_SZ)  |Location                                                       |
|-----------------------------------------------|---------------------------------------------------------------|
|{3D644C9B-1FB8-4f30-9B45-F670235F79C0}         |%PUBLIC%\Downloads                                             |
|Common AppData                                 |%ProgramData%                                                  |
|Common Desktop                                 |%PUBLIC%\Desktop                                               |
|Common Documents                               |%PUBLIC%\Documents                                             |
|Common Programs                                |%ProgramData%\Microsoft\Windows\Start Menu\Programs            |
|Common Start Menu                              |%ProgramData%\Microsoft\Windows\Start Menu                     |
|Common Startup                                 |%ProgramData%\Microsoft\Windows\Start Menu\Programs\Startup    |
|Common Templates                               |%ProgramData%\Microsoft\Windows\Templates                      |
|CommonMusic                                    |%PUBLIC%\Music                                                 |
|CommonPictures                                 |%PUBLIC%\Pictures                                              |
|CommonVideo                                    |%PUBLIC%\Videos                                                |

 - `{3D644C9B-1FB8-4f30-9B45-F670235F79C0}` value represents the Public Downloads folder.
 - The values `CommonMusic`, `CommonPictures`, `CommonVideo` are single words (no space in them).
