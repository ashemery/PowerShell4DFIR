# Windows DFIR
Repository for different Windows DFIR related CMDs, PowerShell CMDlets, etc, plus workshops that I did for different conferences or events.

### Timestamps in UTC
```Get-ChildItem \<PATH\> -Force | Select-Object FullName, CreationTimeUTC, LastAccessTimeUTC, LastWriteTimeUTC```
  
### Timestamps in local time
```Get-ChildItem \<PATH\> -Force | Select-Object FullName, CreationTime, LastAccessTime, LastWriteTime```

### Hash Values (MD5, SHA1, and SHA256)
```Get-FileHash \<PATH\> -Algorithm MD5 | Format-List```

```Get-FileHash \<PATH\> -Algorithm SHA1 | Format-List```

```Get-FileHash \<PATH\> -Algorithm SHA256 | Format-List```

### Find location of executable in PATH (similar to which on Linux Systems)
```where executablename```

### Merge two CSV files
```Get-Content LNK_User1.csv, LNK_User2.csv | Select-Object -Unique | Set-Content -Encoding ASCII LNK_Users.csv```

### Create Symbolic Links to Multiple files. Useful to process files that reside in Known Folders
- Check the file "createSymLinks.ps1" and from where it was found.
- More info about Known Folders: [URL](https://docs.microsoft.com/en-us/windows/win32/shell/known-folders)

## Workshops
- BSides Amman 2021, all files here: [URL](https://github.com/ashemery/WindowsDFIR/tree/master/Workshops/BSidesAmman21)
