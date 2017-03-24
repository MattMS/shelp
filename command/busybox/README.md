# busybox

> The Swiss Army Knife of Embedded Linux

Contains many of the most common commands.

	busybox ls -l

This performs the `ls -l` command.

For `[` and `[[`, see [test](../test/).


## App

- [cal](../cal/)


## Compression

- ar

- bunzip2 bzcat bzip2

- [gunzip](../gunzip/)
  [gzip](../gzip/)

- lzcat lzma

- [md5sum](../md5sum/)

- [sha1sum](../sha1sum/)
  sha256sum sha512sum

- [tar](../tar/)

- uncompress unlzma unxz
  [unzip](../unzip/)
  uudecode uuencode

- xz xzcat

- zcat


## File/folder

- basename

- [chgrp](../chgrp/)
  [chmod](../chmod/)
  [chown](../chown/)
  cmp
  [cp](../cp/)
  cpio

- [dd](../dd/)
  dirname

- [find](../find/)

- [ln](../ln/)
  [ls](../ls/)
  [mv](../mv/)

- [mkdir](../mkdir/)
  mkfifo mknod mkswap mktemp
  [mount](../mount/)
  mt

- pivot_root
  [pwd](../pwd/)

- readlink
  [rm](../rm/)
  [rmdir](../rmdir/)

- stat swapoff swapon switch_root

- [touch](../touch/)

- umount

- watch


### View file contents

- [cat](../cat/)

- [head](../head/)
  [hexdump](../hexdump/)

- [less](../less/)

- [more](../more/)

- [od](../od/)

- [tac](../tac/)
  [tail](../tail/)
  [tee](../tee/)


## Network

- arp arping

- [brctl](../brctl/)

- dnsdomainname

- ftpget ftpput

- hostid hostname httpd

- ifconfig ifdown ifup
  [ip](../ip/)
  ipcalc

- nameif
  [nc](../nc/)
  netstat nslookup

- [ping](../ping/)
  ping6

- route

- telnet telnetd tftp traceroute traceroute6

- vconfig

- wget


### DHCP

- dumpleases

- udhcpc udhcpd


## Processes

- env

- [fuser](../fuser/)

- ionice

- [kill](../kill/)
  killall

- [lsof](../lsof/)

- pidof
  [ps](../ps/)

- renice

- setsid

- [time](../time/)
  timeout
  [top](../top/)

- uptime

- [which](../which/)


## Resources

- [df](../df/)
  [du](../du/)

- fdisk
  [free](../free/)

- taskset


## System

- depmod dmesg
  [dpkg](../dpkg/)
  dpkg-deb

- init insmod

- klogd

- logger losetup lsmod

- modinfo modprobe

- rmmod rpm rpm2cpio

- setkeycodes start-stop-daemon static-sh sync sysctl syslogd

- uname

- watchdog


### Power

- halt

- [poweroff](../poweroff/)

- reboot


## Text processing

- [awk](../awk/)

- [cut](./cut/)

- [diff](../diff/)
  dos2unix

- [ed](../ed/)
  [egrep](../grep/)
  expand

- [fgrep](../grep/)
  fold

- [grep](../grep/)

- patch

- rev

- [sed](../sed/)
  [split](../split/)
  sort

- tr

- unexpand uniq unix2dos

- vi

- [wc](../wc/)


### Text output

- [echo](../echo/)

- printf

- seq
  strings

- yes


## Users

- chpasswd chroot

- groups

- id

- last logname

- passwd

- who whoami


### Scripting

- crond
  [crontab](../crontab/)

- [date](../date/)
  [dc](../dc/)

- expr

- false

- getopt

- run-parts

- sleep

- [test](../test/)
  true

- xargs


### Terminal

- [ash](../ash/)

- chvt
  clear

- getty

- login

- openvt

- reset

- sh stty su sulogin

- tty


## More

- blockdev

- cttyhack

- deallocvt dumpkmap

- freeramdisk

- hwclock

- loadfont loadkmap logread

- mdev microcom

- rdate

- tunctl


## System functions

- adjtimex

- realpath

- usleep


## Links

- [BusyBox on Wikipedia](https://en.wikipedia.org/wiki/BusyBox)
