# Useful-DOSKEYs

```
ls=dir $*
cdc=c:
mv=move $*
cp=copy $*
cat=type $*
clear=cls
vi=notepad $*
rm=del /f $*
grep=findstr $*
ifconfig=ipconfig $*
myip=ipconfig $B findstr IPv4
ip=curl ifconfig.ovh
ss=netstat -ano
ps=tasklist
kill=taskkill /IM $*
locate=dir "\$**" /s
pwd=cd

fridap=frida-ps -Uia $B findstr $*
fridas=frida -U --no-pause -l SSLRoot.js -f $*
fridass=frida -U --no-pause -l $1 -f $*
obj=objection explore -g $*

adb=<PATH>\NoxPlayer\Nox\bin\nox_adb.exe $*
adbn=<PATH>\NoxPlayer\Nox\bin\nox_adb.exe connect 127.0.0.1:62001
adbf=<PATH>\NoxPlayer\Nox\bin\nox_adb.exe shell "/system/bin/sh -c '/data/local/tmp/frida-server &'"

viewdos="<PATH>\Notepad++\notepad++.exe" <PATH>\cmds.bat
```

### Setup
```
reg add "HKCU\Software\Microsoft\Command Processor" /v Autorun /d "doskey /macrofile=\"<PATH>\macros.doskey\"" /f
reg query "HKCU\Software\Microsoft\Command Processor" /v Autorun
```
