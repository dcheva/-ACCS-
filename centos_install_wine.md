# Step 1: Update System
https://computingforgeeks.com/install-wine-on-centos-desktop-system/
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
