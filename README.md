# centOS
running centOS with Apache Open Office
1.  Download ISO http://mirror.vodien.com/centos/7.9.2009/isos/x86_64/CentOS-7-x86_64-Minimal-2009.iso
2.  Create Oracle VM https://www.oracle.com/virtualization/technologies/vm/downloads/virtualbox-downloads.html
3.  Other software Mobaexterm https://mobaxterm.mobatek.net/download.html, Visual Studio Code https://code.visualstudio.com/Download
4.  Create User from installation
5.  Configure network with command nmcli d
6.  nmtui
7.  edit network and activate
8.  Open Terminal and enter following command
>service network restart
>[root@localhost 20210118]# ip addr show

>1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
>    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
>    inet 127.0.0.1/8 scope host lo
>       valid_lft forever preferred_lft forever
>    inet6 ::1/128 scope host
>       valid_lft forever preferred_lft forever
>2: enp0s3: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc pfifo_fast state UP group default qlen 1000
>    link/ether 08:00:27:a7:ad:90 brd ff:ff:ff:ff:ff:ff
>    inet 192.168.1.31/24 brd 192.168.1.255 scope global noprefixroute dynamic enp0s3
>       valid_lft 83099sec preferred_lft 83099sec
>    inet6 fe80::55da:6abf:c111:2ec1/64 scope link noprefixroute
>       valid_lft forever preferred_lft forever

8.  ping google.com
9.  sudo yum –y install openssh-server openssh-clients
10.  sudo systemctl status sshd
systemctl stop sshd
sudo systemctl enable sshd
sudo systemctl disable sshd
11. install Java
> sudo yum install java-1.8.0-openjdk-devel

> /usr/lib/jvm/java-1.8.0-openjdk-1.8.0.275.b01-0.el7_9.x86_64/jre/bin/
12. xterm
> yum install xorg-x11-xauth
> yum install xorg-x11-apps

13. wget http://sourceforge.net/projects/openofficeorg.mirror/files/4.1.8/binaries/en-US/Apache_OpenOffice_4.1.8_Linux_x86-64_install-rpm_en-US.tar.gz
14. tar xzf Apache_OpenOffice_4.1.8_Linux_x86-64_install-rpm_en-US.tar.gz
15. cd en-US/RPMS/
16. rpm -Uvh *.rpm
17. cd desktop-integration/
18. rpm -Uvh openoffice4.1.8-redhat-menus-4.1.8-9803.noarch.rpm
