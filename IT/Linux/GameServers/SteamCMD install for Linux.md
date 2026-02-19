---
tags:
  - linux
  - steam
  - game_server
  - games
  - debian
  - public
title: Устанавливаем SteamCMD Debian
---


- Создаем директорию SteamCMD в /opt/
- Устанавливаем 32-битные библиотеки

```
mkdir /opt/SteamCMD
dpkg --add-architecture i386
apt update && apt upgrade -y
apt install -y lib32gcc-s1 lib32stdc++6 libc6-i386 tar
wget http://media.steampowered.com/client/steamcmd_linux.tar.gz
tar xvfz steamcmd_linux.tar.gz\n
./steamcmd.sh
```