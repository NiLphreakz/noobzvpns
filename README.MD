# NoobzVpn-Server

### What is NoobzVpn ?

Independent tunneling protocol is now in stable stage git-master repository.

### How is work ?
Like other VPN this app just bypass network traffic like tcp,udp including dns. with wide-custom payload and more flexibility. unlike openvpn / ssh tunnel using Concurrent Transport, we use Multiplex Transport (like shadowsock) model with more flexibility to custom Transport model. :)

### Tunneling :
* Dual-Stack IPv4/IPv6
* All TCP, UDP, DNS

### Transport :
* Dual-Stack IPv4/IPv6
* TCP plain & SSL (HTTP/WebSocket/Direct/Etc, custom with your own :p)
* UDP (QUIC/DNS/Etc) ? #comming_soon, we not include it yet. because very poor in my test. but we keep working on it.

# Guide

### Minimum Requiment :
* Linux x86_64 with systemd init.
* 1 Core CPU, 512MB RAM, 500MB Disk Available (my extreme test)
* For other Linux with CPU x86(32bit), arm, arm64 server you can request and join beta test.
* For other init system, you can contribute this project to create/add support for other init system like s6, SysV, runit, OpenRC, etc...

### Installation :
* follow this step with **root user / root access** (sudo/doas/etc)
##### Install / Upgrade (Debian / Ubuntu / other Debian Base)
```
apt update && apt install git && git clone https://github.com/NiLphreakz/noobzvpns.git && cd noobzvpns/ && sh ./install.sh
```
##### Full Uninstall
```
cd noobzvpns/ && sh ./uninstall.sh && cd && rm -r noobzvpns
```

