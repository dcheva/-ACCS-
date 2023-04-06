# Step 1: Update System
```
[symphony3race@vmACCT2 home]$ sudo dnf -y update
...
  Running scriptlet: kernel-tools-4.18.0-483.el8.x86_64                                                                                                                                                                       227/614
error: Couldn't fork %post(kernel-tools-4.18.0-483.el8.x86_64): Cannot allocate memory

Error in POSTIN scriptlet in rpm package kernel-tools
  Upgrading        : python3-libxml2-2.9.7-16.el8.x86_64                                                                                                                                                                      228/614
  Running scriptlet: setroubleshoot-server-3.3.26-5.el8.x86_64                                                                                                                                                                229/614
error: Couldn't fork %prein(setroubleshoot-server-3.3.26-5.el8.x86_64): Cannot allocate memory

Error in PREIN scriptlet in rpm package setroubleshoot-server
  Upgrading        : python3-linux-procfs-0.7.1-1.el8.noarch                                                                                                                                                                  230/614
error: setroubleshoot-server-3.3.26-5.el8.x86_64: install failed
...
...
Installed:
  NetworkManager-initscripts-updown-1:1.40.16-2.el8.noarch grub2-tools-efi-1:2.02-129.el8.x86_64 kernel-4.18.0-483.el8.x86_64 kernel-core-4.18.0-483.el8.x86_64 kernel-modules-4.18.0-483.el8.x86_64 python3-magic-5.33-24.el8.noarch
Failed:
  NetworkManager-1:1.36.0-0.2.el8.x86_64        NetworkManager-1:1.40.16-2.el8.x86_64          WALinuxAgent-2.7.0.6-3.el8.noarch          at-3.1.20-11.el8.x86_64                    audit-3.0-0.17.20191104git1c2f876.el8.x86_64
  authselect-1.2.2-3.el8.x86_64                 authselect-libs-1.2.2-3.el8.x86_64             authselect-libs-1.2.6-1.el8.x86_64         binutils-2.30-111.el8.x86_64               ca-certificates-2021.2.50-82.el8.noarch
  ca-certificates-2022.2.54-80.2.el8.noarch     chrony-4.1-1.el8.x86_64                        chrony-4.2-1.el8.x86_64                    cloud-init-22.1-5.el8.noarch               cockpit-ws-258-1.el8.x86_64
  cockpit-ws-288.2-1.el8.x86_64                 coreutils-common-8.30-12.el8.x86_64            cronie-1.5.2-6.el8.x86_64                  dbus-daemon-1:1.12.8-18.el8.x86_64         dbus-daemon-1:1.12.8-24.el8.x86_64
  device-mapper-event-8:1.02.181-1.el8.x86_64   dnf-4.7.0-5.el8.noarch                         firewalld-0.9.3-11.el8.noarch              grub2-tools-1:2.02-106.el8.x86_64          grub2-tools-1:2.02-129.el8.x86_64
  gzip-1.9-12.el8.x86_64                        initscripts-10.00.15-1.el8.x86_64              iptables-1.8.4-22.el8.x86_64               iptables-1.8.4-24.el8.x86_64               iptables-ebtables-1.8.4-22.el8.x86_64
  iputils-20180629-7.el8.x86_64                 irqbalance-2:1.4.0-6.el8.x86_64                kexec-tools-2.0.20-63.el8.x86_64           kmod-kvdo-6.2.5.72-81.el8.x86_64           kmod-kvdo-6.2.8.7-89.el8.x86_64
  libgomp-8.5.0-6.el8.x86_64                    libwbclient-4.14.5-2.el8.x86_64                logrotate-3.14.0-4.el8.x86_64              logrotate-3.14.0-6.el8.x86_64              lvm2-8:2.03.14-1.el8.x86_64
  mcelog-3:179-1.el8.x86_64                     mdadm-4.2-rc2.el8.x86_64                       nftables-1:0.9.3-24.el8.x86_64             oddjob-0.34.7-1.el8.x86_64                 openssh-8.0p1-12.el8.x86_64
  openssh-8.0p1-17.el8.x86_64                   openssh-server-8.0p1-12.el8.x86_64             openssh-server-8.0p1-17.el8.x86_64         policycoreutils-2.9-17.el8.x86_64          polkit-0.115-12.el8.x86_64
  polkit-0.115-15.el8.x86_64                    realmd-0.16.3-23.el8.x86_64                    rsyslog-8.2102.0-6.el8.x86_64              samba-common-4.14.5-2.el8.noarch           samba-common-4.17.5-0.el8.noarch
  selinux-policy-targeted-3.14.3-85.el8.noarch  selinux-policy-targeted-3.14.3-117.el8.noarch  setroubleshoot-server-3.3.24-4.el8.x86_64  setroubleshoot-server-3.3.26-5.el8.x86_64  sssd-client-2.5.2-2.el8_5.1.x86_64
  sssd-common-2.5.2-2.el8_5.1.x86_64            sssd-common-2.8.2-1.el8.x86_64                 sssd-ipa-2.5.2-2.el8_5.1.x86_64            sssd-ipa-2.8.2-1.el8.x86_64                sssd-kcm-2.5.2-2.el8_5.1.x86_64
  sssd-krb5-common-2.5.2-2.el8_5.1.x86_64       sssd-krb5-common-2.8.2-1.el8.x86_64            sssd-proxy-2.5.2-2.el8_5.1.x86_64          sssd-proxy-2.8.2-1.el8.x86_64              systemd-239-51.el8.x86_64
  systemd-239-73.el8.x86_64                     tar-2:1.30-5.el8.x86_64                        tcpdump-14:4.9.3-2.el8.x86_64              tcpdump-14:4.9.3-3.el8.x86_64              tuned-2.16.0-1.el8.noarch
  unbound-libs-1.7.3-17.el8.x86_64              unbound-libs-1.16.2-5.el8.x86_64               wget-1.19.5-10.el8.x86_64

Error: Transaction failed
...
...
[symphony3race@vmACCT2 home]$ sudo dnf -y update
Killed
[symphony3race@vmACCT2 home]$ dmesg | egrep -i killed
...
[ 6144.651319] Out of memory: Killed process 2902 (dnf) total-vm:551872kB, anon-rss:192692kB, file-rss:4kB, shmem-rss:0kB, UID:0 pgtables:1060kB oom_score_adj:0
...
...
[symphony3race@vmACCT2 home]$ sudo fallocate -l 1G /swapfile
[symphony3race@vmACCT2 home]$ sudo mkswap /swapfile
mkswap: /swapfile: insecure permissions 0644, 0600 suggested.
Setting up swapspace version 1, size = 1024 MiB (1073737728 bytes)
no label, UUID=8bd917fd-68e7-4015-8d30-ef76ffc372e6
[symphony3race@vmACCT2 home]$ sudo chmod 0600 /swapfile
[symphony3race@vmACCT2 home]$ sudo swapon /swapfile
[symphony3race@vmACCT2 home]$ sudo dnf -y update
...
Upgraded:
  authselect-libs-1.2.6-1.el8.x86_64            ca-certificates-2022.2.54-80.2.el8.noarch chrony-4.2-1.el8.x86_64          cockpit-ws-288.2-1.el8.x86_64      dbus-daemon-1:1.12.8-24.el8.x86_64  iptables-1.8.4-24.el8.x86_64
  kmod-kvdo-6.2.8.7-89.el8.x86_64               logrotate-3.14.0-6.el8.x86_64             openssh-8.0p1-17.el8.x86_64      openssh-server-8.0p1-17.el8.x86_64 polkit-0.115-15.el8.x86_64          samba-common-4.17.5-0.el8.noarch
  selinux-policy-targeted-3.14.3-117.el8.noarch setroubleshoot-server-3.3.26-5.el8.x86_64 sssd-common-2.8.2-1.el8.x86_64   sssd-ipa-2.8.2-1.el8.x86_64        sssd-krb5-common-2.8.2-1.el8.x86_64 sssd-proxy-2.8.2-1.el8.x86_64
  systemd-239-73.el8.x86_64                     tcpdump-14:4.9.3-3.el8.x86_64             unbound-libs-1.16.2-5.el8.x86_64
Removed:
  authselect-1.2.2-3.el8.x86_64                                            iptables-ebtables-1.8.4-22.el8.x86_64                                            sssd-kcm-2.5.2-2.el8_5.1.x86_64

Complete!
...
sudo reboot
```
# Step 2: Install Software Building dependencies
```
[symphony3race@vmACCT2 ~]$ sudo dnf groupinstall 'Development Tools' -y
Failed:
  glibc-headers-2.28-225.el8.x86_64               pesign-0.112-26.el8.x86_64               sgml-common-0.6.3-50.el8.noarch               systemtap-runtime-4.8-2.el8.x86_64               xml-common-0.6.3-50.el8.noarch

Error: Transaction failed
[symphony3race@vmACCT2 ~]$
...
Running transaction
  Preparing        :                                                                                                                                                                                                              1/1
  Running scriptlet: pesign-0.112-26.el8.x86_64                                                                                                                                                                                   1/1
error: Couldn't fork %prein(pesign-0.112-26.el8.x86_64): Cannot allocate memory

Error in PREIN scriptlet in rpm package pesign
  Verifying        : pesign-0.112-26.el8.x86_64                                                                                                                                                                                   1/1

Failed:
  pesign-0.112-26.el8.x86_64

Error: Transaction failed
...
[symphony3race@vmACCT2 home]$ sudo mkswap /swapfile
Setting up swapspace version 1, size = 1024 MiB (1073737728 bytes)
no label, UUID=8bd917fd-68e7-4015-8d30-ef76ffc372e6
[symphony3race@vmACCT2 home]$ sudo swapon /swapfile
[symphony3race@vmACCT2 ~]$ sudo dnf groupinstall 'Development Tools' -y

Complete!
...
[symphony3race@vmACCT2 /]$ free -m
              total        used        free      shared  buff/cache   available
Mem:            400         171          79           3         149         214
Swap:          1023           0        1023
...
sudo dnf -y install epel-release
sudo dnf config-manager --set-enabled powertools
...
sudo dnf -y install libxslt-devel libpng-devel libX11-devel zlib-devel libtiff-devel freetype-devel libxcb-devel  libxml2-devel libgcrypt-devel dbus-devel libjpeg-turbo-devel  fontconfig-devel gnutls-devel gstreamer1-devel libXcursor-devel libXi-devel libXrandr-devel libXfixes-devel libXinerama-devel libXcomposite-devel mesa-libOSMesa-devel libpcap-devel libusb-devel libv4l-devel libgphoto2-devel gstreamer1-devel libgudev SDL2-devel gsm-devel libvkd3d-devel libudev-devel make cmake gcc flex

Complete!
```
# Step 3: Install Wine
```
[symphony3race@vmACCT2 /]$ sudo dnf -y install wget
Complete!
[symphony3race@vmACCT2 /]$ cd ~
[symphony3race@vmACCT2 ~]$ curl -O https://dl.winehq.org/wine/source/8.x/wine-8.1.tar.xz
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100 27.7M  100 27.7M    0     0   124M      0 --:--:-- --:--:-- --:--:--  123M
...
[symphony3race@vmACCT2 ~]$ cd wine-*/
[symphony3race@vmACCT2 wine-8.1]$ ./configure --enable-win64
checking build system type... x86_64-pc-linux-gnu
checking host system type... x86_64-pc-linux-gnu
checking whether make sets $(MAKE)... yes
checking for gcc... gcc
checking whether the C compiler works... yes
checking for C compiler default output file name... a.out
checking for suffix of executables...
checking whether we are cross compiling... configure: error: in `/home/symphony3race/wine-8.1':
configure: error: cannot run C compiled programs.
If you meant to cross compile, use `--host'.
See `config.log' for more details
[symphony3race@vmACCT2 wine-8.1]$
```
# Step 4: ok. Install Wine
```
sudo dnf clean all && sudo dnf update
...
...
[symphony3race@vmACCT2 ~]$ cd /
[symphony3race@vmACCT2 /]$ sudo dnf install epel-release
[symphony3race@vmACCT2 /]$ sudo yum install wine
Last metadata expiration check: 0:00:58 ago on Thu 06 Apr 2023 07:24:31 PM UTC.
Dependencies resolved.
...
Installing:
 wine 
...
Install  184 Packages
...

Complete!
```
# Step 5: Get and run server
```
[symphony3race@vmACCT2 ~]$ git clone https://github.com/dcheva/-ACCS-.git ACCS
[symphony3race@vmACCT2 ~]$ cd ACCS/server
[symphony3race@vmACCT2 ~]$ wine accServer.exe
0070:err:explorer:initialize_display_settings Failed to query current display settings for L"\\\\.\\DISPLAY1".
0024:fixme:msvcp:_Locinfo__Locinfo_ctor_cat_cstr (000000000017E980 1 C) semi-stub
0024:fixme:msvcp:_Locinfo__Locinfo_ctor_cat_cstr (000000000017E5F0 1 C) semi-stub
0024:fixme:msvcp:_Locinfo__Locinfo_ctor_cat_cstr (000000000017E5E0 1 C) semi-stub
Server starting with version 255
Starting server Efun A Wort [EUR#2] Two races per hour weekend
Joining during race is allowed
Translated realtime interval hzToMiliseconds(18)=54

SessionManager::randomizeGreenFlagTriggers: s:0.890000 e:0.950000 r:0.911228
Track monza was set and updated
Event changed
==ERR: Ignoring special assist rules for public Multiplayer
SessionManager::randomizeGreenFlagTriggers: s:0.890000 e:0.950000 r:0.929783
Significant change detected, updating lobby (1|1)
Resetting weekend to friday night
Reset time to friday night: 0 -> 0
Reset time to first session: 0 -> 43200
SessionManager::randomizeGreenFlagTriggers: s:0.890000 e:0.950000 r:0.903349
Listening to TCP 9601 | UDP 9600
Trying to connect to lobby (0 times, interval 10000 s)
Session changed: Practice -> Practice 0
Detected sessionPhase <waiting for drivers> -> <waiting for drivers> (Practice)
TCP connect returns: -1
TCP connect returns: 0
==ERR: RegisterToLobby TCP connection failed, couldn't connect to the lobby server
Trying to connect to lobby (1 times, interval 13000 s)
00dc:fixme:msvcp:_Locinfo__Locinfo_ctor_cat_cstr (00000000012EF7B0 1 C) semi-stub
00dc:fixme:msvcp:_Locinfo__Locinfo_ctor_cat_cstr (00000000012EF7B0 1 C) semi-stub
00dc:fixme:msvcp:_Locinfo__Locinfo_ctor_cat_cstr (00000000012EF7B0 1 C) semi-stub
RegisterToLobby succeeded
==ERR: This server is only supported on Windows operating systems. Running WINE may work dependent on your settings, but there are differences that affect the user's experience negatively.
Sent lobby registration request for monza
```
___
