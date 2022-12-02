- [< Back to Knowledge](https://github.com/monpopza/knowledge)

# Linux Command Type

# Power Management
- Shutdown and Restart
  ```
  shutdown -h
  shutdown -r
  ```
- add timer
  ```
  add -t second >> shutdown -h -t 0 | shutdown -t now
  ```

# Package and service Management
- Install Update Upgrade and uninstall
  ```
  apt >> apt install | apt update | apt upgrade | apt remove/autoremove
  brew >> brew install | brew update | brew upgrade | brew uninstall/remove
  yum  >> yum install | yum update | yum upgrade | yum remove/erase | yum localinstall package.rpm
  dpkg >> dpkg -i package.deb | dkg -r package.deb
  rpm >> rpm -i package.rpm | rpm -e package.rpm
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
  ```
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
  userdd
  ```
- Remove User
  ```
  userdel
  ```
- Modify User 
  ```
  usermod
  ```
- Change Password
  ```
  passwd
  ```
- Add Group
  ```
  groupadd
  ```
- Remove Group
  ```
  groupdel
  ```
- Modify Group
  ```
  groupmod
  ```
- Login with Internal/Inside
  ```
  login username
  ```
- Login with Remote 
  ```
  ssh username@ipaddree/domain
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
  ```

# File Management
- folder and file command
  ```
  ls
  cd
  mkdir / rmdir
  rm
  pwd
  ln / alias-knallias
  cp
  mv
  rename
  find/locate
  grep/less
  ```
- owner file Command
  ```
  chmod
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
  diff
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
  ipconfig = ifconfig
  ```
- Firewall
  ```
  ufw
  iptable
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
  nslookup
  ping
  perf
  traceroute
  ```
# Utility
- Date time and calendar 
  ``` 
  cal
  date
  time
  ```
- What's system is?
  ```
  whoami / who
  uname -a 
  export
  ```
- Multiple in once
  ```
  tux
  ```
