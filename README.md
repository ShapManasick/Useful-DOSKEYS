# Useful-DOSKEYs

```
@echo off
doskey ls=dir $*
doskey cdc=c:
doskey mv=move $*
doskey cp=copy $*
doskey cat=type $*
doskey clear=cls
doskey vi=notepad $*
doskey rm=del /f $*
doskey grep=findstr $*
doskey ifconfig=ipconfig $*
doskey myip=ipconfig $B findstr IPv4
doskey ip=curl ifconfig.ovh
doskey ss=netstat -ano
doskey ps=tasklist
doskey kill=taskkill /IM $*
doskey locate=dir "\$**" /s
doskey pwd=cd

doskey fridap=frida-ps -Uia $B findstr $*
doskey fridas=frida -U --no-pause -l SSLRoot.js -f $*
doskey fridass=frida -U --no-pause -l $1 -f $*
doskey obj=objection explore -g $*

doskey adb=<PATH>\NoxPlayer\Nox\bin\nox_adb.exe $*
doskey adbn=<PATH>\NoxPlayer\Nox\bin\nox_adb.exe connect 127.0.0.1:62001
doskey adbf=<PATH>\NoxPlayer\Nox\bin\nox_adb.exe shell "/system/bin/sh -c '/data/local/tmp/frida-server &'"

doskey viewdos="C:\Program Files (x86)\Notepad++\notepad++.exe" <PATH>\.cmds\cmds.bat
```

### Setup
```
reg add "HKCU\Software\Microsoft\Command Processor" /v Autorun /d "doskey /macrofile=\"<PATH>\macros.doskey\"" /f
reg query "HKCU\Software\Microsoft\Command Processor" /v Autorun
```
