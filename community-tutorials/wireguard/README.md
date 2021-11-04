---
title: Wireguard VPN on most Linux Server
description: How to install a Wireguard VPN Server very easy on most Linux Servers
updated_at: 2021-11-04
slug: install-wireguard-vpn-server-linux
author_name: Jonas Löchner
author_url: https://sancraft.dev/
author_image: https://dl.sancraft.dev/images/Sanoj/1-B.png
author_bio: -
tags: vpn, wg, wireguard, linux, debian, ubuntu, centos, fedora
netcup_product_url: https://netcup.de/bestellen/produkt.php?produkt=2623
language: en
available_languages: en
---

# Introduction
This tutorial will show you, how you can very easily install a Wireguard VPN server on the most Linux OSs on the server "RS 2000" trough a very easy installer and how you can connect to the vpn <br>
Wireguard is a fast, secure and easy to use VPN Software.
This is an advenced version of https://github.com/SanCraftDev/Debian-Setup/blob/main/README.md#wireguard-vpn

# Requirements
You need a Debian Server with an Internet Connection, which is accessible from the internet ​over a static IP or over a DynDNS address on a port of your choice. You also need root permissions on your server.

# Step 1 - Installing Wireguard
First you need to connect to your server over ssh.
Then we are going to switch to the root user and are going to update the system, and then we are going to install the Wireguard VPN Server
```sh
sudo su
apt update && apt upgrade -y && apt autoremove -y
wget git.io/wireguard -O wireguard-install.sh && sudo bash wireguard-install.sh
```

# Step 1.1 - Follwing the Installer
Now we need to follow the installer. <br>
```sh
First select your IP address, which should be shown, then press Enter
Now set there a Random Number under 1000 and press Enter
Now give your first VPN Client a Name and press Enter
As DNS Server I recommend to use AdGuard, if you want select 6 or another DNS server, now press Enter
Start the Installation, trough pressing Enter, now wait
```
Save the Installer for later to create more client configurations
```sh
wget git.io/wireguard -O wireguard-install.sh
chmod 700 /root/wireguard-install.sh
```sh

## Step 1.2 - Creating/Removing client configurations or remove wireguard - (Optional)
Now, if you want to use more than one device, you should create more client configurations.
Just run:
```sh
/root/wireguard-install.sh
```
Now you can follow the steps to creating or removing a client configurations or remove entire wireguard

# Step 2 - Setting up the devices
Download your client configuration, which is saved under /root/CLIENT-NAME.conf
Download the correct client for your device from https://www.wireguard.com/install/
Import your client configuration and connect to the VPN!

# Conclusion
Now you have set up a Wireguard VPN Server and connect your devices with the VPN. <br>
This is an advenced version of https://github.com/SanCraftDev/Debian-Setup/blob/main/README.md#wireguard-vpn

# License
MIT

# Contributor's Certificate of Origin
Contributor's Certificate of Origin By making a contribution to this project, I certify that:

 1) The contribution was created in whole or in part by me and I have the right to submit it under the license indicated in the file; or

 2) The contribution is based upon previous work that, to the best of my knowledge, is covered under an appropriate license and I have the right under that license to submit that work with modifications, whether created in whole or in part by me, under the same license (unless I am permitted to submit under a different license), as indicated in the file; or

 3) The contribution was provided directly to me by some other person who certified (a), (b) or (c) and I have not modified it.

 4) I understand and agree that this project and the contribution are public and that a record of the contribution (including all personal information I submit with it, including my sign-off) is maintained indefinitely and may be redistributed consistent with this project or the license(s) involved.

Signed-off-by: Jonas Löchner | [admin@san0j.de](mailto:admin@san0j.de)
