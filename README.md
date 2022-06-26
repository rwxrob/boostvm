# SKILSTAK Beginner Boost Starter VM

Welcome to the first release of the SKILSTAK Beginner Boost virtual machine.

## Install a VMWare Player of Some Kind

* [VMWare Workstation Player (Free)](https://customerconnect.vmware.com/en/downloads/details?downloadGroup=WKST-PLAYER-1622&productId=1039)
* [VMWare Workstation Pro (Trial)](https://customerconnect.vmware.com/en/downloads/details?downloadGroup=WKST-1621-WIN&productId=1038)
* [VMware Fusion for Mac (Free)](https://customerconnect.vmware.com/downloads/get-download?downloadGroup=FUS-PUBTP-2021H1)

You might also consider joining your local [VMUG](https://www.vmug.com/membership/vmug-advantage-membership/).

## Download, Import, Setup SKILSTAK Boost VM (OVA File)

1. Download the [OVA][] file
2. Optionally [validate the checksum](#optional-checksum-validation)
3. Download and install Oracle VirtualBox
4. Double click the [OVA][] file to open and import into VirtualBox
5. Login as user `boost` with password `password`
6. Note the IP address 
7. Connect from Windows Terminal or iTerm2 using `ssh boost@<ipaddress>

[OVA]: https://drive.google.com/file/d/1jKFuD7RGAFWITuWTfj4ILqoDYfi88gRA/view?usp=sharing

## Optional Checksum Validateion

For those who know what sha256sum is and how to validate it here is the checksum:

```
119340D890EDD11A0BA914804CEBBC68F9DF507C53035FFBA5DD577DF890C445
```

For those who don't know what a checksum is (yet) don't worry about it for now. Eventually, you will be able to use this to validate that a time is the authentic original and not been tampered with in transit or put on a phishing server to hack you.

## Setup

This repo contains the setup script to create a fresh SKILSTAK Beginner
Boost Ubuntu Server virtual machine. Most will never need it and can
just use the [OVA] file.  But for those who want to make their own
simply install Ubuntu Server and run the script within this repo to
setup the server and install everything.

> 💀DANGER: This script is highly destructive! Piping this (or any
> random script from the Internet) and running as root with bash is
> a horrible idea unless you know what every line of the script does. DO
> NOT RUN THIS ON A SYSTEM YOU CARE ABOUT! It is for beginner training
> only and even then is primarily used to create safe training virtual
> machines that should be downloaded and used instead of this script.

```
curl https://raw.githubusercontent.com/rwxrob/boostvm/main/run | sudo bash
```

