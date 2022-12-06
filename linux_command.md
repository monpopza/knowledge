[Back](https://github.com/monpopza/knowledge) | [Home](https://github.com/monpopza)

# Linux Command Type

# Power Management
- Shutdown and Restart
  ```
  shutdown >> shutdown -h
  restart  >> shutdown -r
  ```
- add timer
  ```
  add -t second >> shutdown -h -t 0 | shutdown -t now
  ```

# Package and service Management
- Install Update Upgrade and uninstall (SUDO)
  - Debian Base 
  ```
  apt >> apt install | apt update | apt upgrade | apt remove/autoremove
  dpkg >> dpkg -i package.deb | dkg -r package.deb
  ```
  - Centos/RedHat Base
  > [more detail](https://www.interserver.net/tips/kb/install-dnf-in-rhel-centos-7/)
  ```
  yum/dnf  >> yum install | yum update | yum upgrade | yum remove/erase | yum localinstall package.rpm
  rpm >> rpm -i package.rpm | rpm -e package.rpm
  ``` 
  > need to login in [Redhat](https://access.redhat.com/solutions/253273)
  
  - MacOS/OSX Base
  ```
  brew >> brew install | brew update | brew upgrade | brew uninstall/remove
  ```
  > need to setup [brew](https://brew.sh)
  - Arch Linux Base
  ```
  pacman >> pacman -S package | pacman -R/-Rs package
  ```
- Package/Service Stop
  ```
  kill/killall
  pkill
  ```
- Taskmanager
  ```
  top
  htop
  ```
- Service command
  ```
  service >> sudo service start package / sudo service stop backage
  systemctl >> sudo systemctl | grep running
  ```
- Service Task Timer
  ```
  cronjob
  crontab
  ```
  > [crontab generator](https://crontab-generator.org)
  ![cronjob](https://www.guru99.com/images/1/011720_0741_CrontabinLi1.png)

- Partition Management
  ```
  df
  fdisk
  mount
  dd
  ```
# User and group Management
- Login to Super User
  ```
  su
  sudo -i
  ```
- User Superuser to run command
  ```
  sudo package
  ```
- User Info
  ```
  id
  ```
- User List
  ```
  users
  ```
- Add User 
  ```
  userdd newuser
  ```
- Remove User
  ```
  userdel loduser
  ```
- Modify User 
  ```
  usermod modiuser
  ```
- Change Password
  ```
  passwd
  passwd user
  ```
- Add Group
  ```
  groupadd namegroup
  ```
- Remove Group
  ```
  groupdel namegroup
  ```
- Modify Group
  ```
  groupmod namegroup
  ```
- Login with Internal/Inside
  ```
  login username
  ```
- Login with Remote 
  ```
  ssh username@ipaddree/domain
  telnet username@ipaddress
  ```
- logout
  ```
  exit
  logout
  ```
# Help/Manual
- F1 Package
  ```
  whatis >> whatis package
  man >> man package
  help >> package help/--help/-h/-help
  whereis >> whereis package
  ```

# File Management
- for folder
  ```
  ls directory/directory/directory
  ls
  ls - Flash (list as human)
  cd directory/directory/directory
  mkdir / rmdir directory/directory/directory
  rm filename.file
  rm -rf directory
  ```
- show where am I in directory
  ```
  pwd
  ```
- Link File (shortcut file)
  ```
  ln filenamea directory/filenamea
  alias-knallias
  ```
- copy file
  ```
  cp filea directory/filea
  ```
- move file
  ```
  mv filea directory filea
  ```
- change name file
  ```
  mv filea fileb
  ```
- etc for file and explorer
  ```
  find/locate
  grep >> search file
  less/more >> list full screem with use arrow down and uo to select
  ```
- owner file Command
  ```
  chmod 777
  chmod +x
  chown
  chgrp
  ```
- Text Command
  ```
  nano
  vi
  touch / mkfile
  cat
  tail
  diff >> compare ascii two file
  
  ```
- Compress and uncompress File Command
  ```
  tar
  zip / unzip
  xz
  gzip
  ```
- Download File
  ```
  wget
  curl
  ```

# Network Management
- General
  ```
  debian base > ipconfig = ifconfig
  ip add / ip addr
  ```
  > redhat use ipconfig > install net-tools
- Firewall
  ```
  debian base > ufw / iptable
  redhat base > firewall-cmd
  ```
- Stop Network
  ```
  ifdown
  ```
- Start Network
  ```
  ifup
  ```
- Network utility 
  ```
  nslookup (redhat install bind-utils)
  ping
  perf
  traceroute
  ```
# Utility
- Date time and calendar 
  ``` 
  clock >> set clock
  cal
  date
  time
  ```
- What's system is?
  ```
  whoami / who / whois
  uname -a 
  export
  ```
- Multiple in once
  ```
  tmux
  ```
- run in backgroud
  ```
  screen
  ```

[Back](https://github.com/monpopza/knowledge) | [Home](https://github.com/monpopza)
