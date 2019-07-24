## CentOS 7 x86_64 Setup 

#### Setup local CentOS 7 repo from ISO
- Copy ISO to local
- modify [base] repo and use the DVD ISO as repository

#### Update CentOS 7 OS
```bash
yum clean all
yum -y update
yum install git ansible bind-utils net-tools vim-enhanced

sync; reboot 
```
#### Install 3rd party repo and addons 
```bash
yum install epel-release

yum install ntfs-3g ntfsprogs 

yum install htop tcping  
```

#### Install gui tools

* visual studio code
```bash
rpm --import https://packages.microsoft.com/keys/microsoft.asc

sh -c 'echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/vscode.repo'

yum install code
```
* google chrome/chromium browser
`yum -y install chromium`
