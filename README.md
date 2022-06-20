# SKILSTAK Beginner Boost Starter VM

To get started
Welcome to the first release of the SKILSTAK Beginner Boost virtual machine. Follow these steps to get up and running as fast as possible:

1. Download the [OVA][] file
2. Download and install Oracle VirtualBox
3. Double click the [OVA][] file to open and import into VirtualBox
4. Login as user `boost` with password `password`
5. Note the IP address 
6. Connect from Windows Terminal or iTerm2 using `ssh boost@<ipaddress>

[OVA]: https://mega.nz/file/9CM0yIiL#uPslRos1XLLV76fvs7VwPvFTQNukHBGdXbjiWyynWdk

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

