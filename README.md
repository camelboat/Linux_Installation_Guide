# Introduction
- This document includes suggestions for installing linux(ubuntu, especially kubuntu) for my personal use.
- Don't want to waste time for searching all of these again each time installing a new system!!!

## Tips
- If the original system is in UEFI, then you need to partition the disk before you start to install the new system(so that you can have two systems) or you switch the BIOS to legacy boot mode and install it on the whole disk.
- Update mirrors deb if in China in `$ /etc/apt/sources.list`
- kwin setting, just follow the last computer
- vim setting
- Modify default editor to vim 
`$ sudo update-alternatives --config editor`
## software list
- wps office
- sogou input
- darktable
- pari-gp
- matlab
- clion
- pycharm

## specific softwares concerns

### wps office:
- to install the lost fonts, go to https://github.com/iamdh4/ttf-wps-fonts
- To solve the problem of opening document in Ark, run:
```bash
$ cd /usr/share/mime/packages
$ sudo rm wps-office-et.xml
$ sudo rm wps-office-wpp.xml
$ sudo rm wps-office-wos.xml
$ sudo update-mime-database /usr/share/mime
```
