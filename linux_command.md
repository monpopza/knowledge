[⬅️](https://github.com/monpopza/knowledge) | [🏠](https://github.com/monpopza)<br/>
-------
# Linux Command
- [Exit! ↗](https://github.com/monpopza/knowledge/blob/main/linux_command.md#exit-program%EF%B8%8F)
- [Power ↗](https://github.com/monpopza/knowledge/blob/main/linux_command.md#power-management%EF%B8%8F)
- [Package and Service ↗](https://github.com/monpopza/knowledge/blob/main/linux_command.md#package-and-service-management%EF%B8%8F)
- [User&Group ↗](https://github.com/monpopza/knowledge/blob/main/linux_command.md#user-and-group-management%EF%B8%8F)
- [Manual ↗](https://github.com/monpopza/knowledge/blob/main/linux_command.md#helpmanual%EF%B8%8F)
- [File ↗](https://github.com/monpopza/knowledge/blob/main/linux_command.md#file-Management%EF%B8%8F)
- [Network ↗](https://github.com/monpopza/knowledge/blob/main/linux_command.md#network-management%EF%B8%8F)
- [Utility ↗](https://github.com/monpopza/knowledge/blob/main/linux_command.md#utility%EF%B8%8F)
- [HardwareInfo ↗](https://github.com/monpopza/knowledge/blob/main/linux_command.md#check-version-os-and-hardware%EF%B8%8F)
-------
# Exit Program[⬆️](https://github.com/monpopza/knowledge/blob/main/linux_command.md#linux-command)
  - use keyboard to exit program (process)
    ```
    exit > ctrl+c
    force exit > Ctrl+Z
    ```
 -------
# Power Management[⬆️](https://github.com/monpopza/knowledge/blob/main/linux_command.md#linux-command)
  - Shutdown and Restart
    ```
    shutdown >> shutdown -h
    restart  >> shutdown -r
    ```
  - add timer (sec)
    ```
    shutdown -h -t 0
    shutdown -t now
    ```
-------
# Package and service Management[⬆️](https://github.com/monpopza/knowledge/blob/main/linux_command.md#linux-command)
  - Administrator run
    ```
    sudo package
    sudo apt/dnf/yum
    ```
  - Install Update Upgrade and uninstall (SUDO)
    - Debian Base 🟠
      ```
      apt >> apt install | apt update | apt upgrade | apt remove/autoremove
      dpkg >> dpkg -i package.deb | dkg -r package.deb
      ```
    - Centos/RedHat Base [?](https://www.interserver.net/tips/kb/install-dnf-in-rhel-centos-7/)
      ```
      yum/dnf  >> yum install | yum update | yum upgrade | yum remove/erase | yum localinstall package.rpm
      rpm >> rpm -i package.rpm | rpm -e package.rpm
      ``` 
      > redhat need to login in [?](https://access.redhat.com/solutions/253273)
  
    - MacOS [?](https://brew.sh)
      ```
      brew >> brew install | brew update | brew upgrade | brew uninstall/remove
      ```
    - Arch Linux Base
      ```
      pacman >> pacman -S package | pacman -R/-Rs package
      ```
  - Package/Service Stop
    ```
    kill/killall
    pkill
    ```
  - Task Manager
    ```
    top
    htop
    btop
    ```
    > some package need to install
  - Service command
    ```
    service >> sudo service start package / sudo service stop backage
    systemctl >> sudo systemctl | grep running
    ```
  - Service Task Timer[?](https://crontab-generator.org)
    ```
    cronjob
    crontab
    ```
    ![cronjob](https://www.guru99.com/images/1/011720_0741_CrontabinLi1.png)

  - Partition Management
    ```
    df
    fdisk
    mount
    dd
    ```
-------
# User and group Management[⬆️](https://github.com/monpopza/knowledge/blob/main/linux_command.md#linux-command)
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
    useradd newuser
    adduser newuser
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
-------
# Help/Manual[⬆️](https://github.com/monpopza/knowledge/blob/main/linux_command.md#linux-command)
  - FAQ. Help. Manual. Location.
    ```
    whatis >> whatis package
    man >> man package
    help >> package help/--help/-h/-help
    whereis >> whereis package
    ```
-------
# File Management[⬆️](https://github.com/monpopza/knowledge/blob/main/linux_command.md#linux-command)
  - go to folder in folder in folder
    ```
    cd directory/directory/directory
    ```
  - list all **item** in folder 
    ```
    ls directory/directory/directory
    ls
    ls -la  =  ll (need to install)
    ls - Flash (easy to read)
    ```
  - remove your folder
    ```
    rmdir directory
    rm -rf directory
    ```
  - make your folder
    ```
    mkdir newfolder
    ```
  - where am I in directory
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
  - Text Editor
    - nano[?](https://www.geeksforgeeks.org/nano-text-editor-in-linux/)
    - vi[?](https://saixiii.com/vi-linux-command/)
      ```
      nano
      nano namefile
      vi
      vi namefile
      vim
      vim namefile
      ```
    - Make new file (blank file)
      ```
      touch / mkfile
      ```
    - remove file 
      ```
      rm filename.file
      ```
    - show file detail as text in cmd/cli
      ```
      cat
      tail
      ```
    - compare file pair as text
      ```
      diff >> compare ascii two file
      diff 1 2
      ```
  - Compress and uncompress File Command 
  /*(somepackage need to install)*/
  - tar [more](https://www.howtogeek.com/248780/how-to-compress-and-extract-files-using-the-tar-command-on-linux/)<br/>
    [Compress]
    ```
    [one1] tar -czvf file.tar.gz /path/to/dir-file
    [mult] tar -czvf allfile.tar.gz /pathto/dir1 pathto/dir2 /file3
    ```
    [Decompress]
    ```
    tar -zxvf myfile.tar.gz
    tar -xzvf myfile.tar.gz -C /path/to/need
    ```
  
  - zip/unzip [more](https://www.geeksforgeeks.org/zip-command-in-linux-with-examples/) <br/>
    [Compress]
    ```
    zip file.zip file_list
    zip file.zip folder
    zip file.zip list file to zip
    ```
    [Decompress]
    ```
    unzip file.zip
    ```
  
  - xz[?](https://linuxhint.com/xz_compression_tutorial/) <br/>
    [Compress]
    ```
    xz file
    xz 1 2 3 4 5 6
    xz -k file_keep_original
    xz -c 1 2 3 4 5 6 > keepfile.xz
    ```
    [Decompress]
    ```
    xz -d file.xz
    unxz file.xz
    ```
    [info]
    ```
    xz -l file.xz
    ```
  - gzip/gunzip <br/>
  
    [Compress]
    ```
    gzip file   [*️⃣file will be removed]
    gzip -c file > file.gz
    ```
    [Decompress]
    ```
    gzip -d file.gz
    gunzip file.gz [*️⃣file will be removed]
    ```
    [List in gz]
    ```
    gzip -cd file.gz | wc -c
    ```

  - Download File (https)
    ```
    wget 'urldownload'
    curl 'urldownload'
    ```

-------
# Network Management[⬆️](https://github.com/monpopza/knowledge/blob/main/linux_command.md#linux-command)
  - Show IP Address and Interface
    ```
    debian base 🟠 > ipconfig = ifconfig
    ip add / ip addr
    ```
    > 🔴redhat use ipconfig > install net-tools

  - Firewall
    ```
    debian base 🟠 > ufw / iptable
    redhat base 🔴 > firewall-cmd
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
    nslookup (redhat🔴 install bind-utils)
    ping
    perf
    traceroute
    tracepath (redhat🔴)
    ```
  
 -------
# Utility[⬆️](https://github.com/monpopza/knowledge/blob/main/linux_command.md#linux-command)
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
  - Browser 
  > need to install 
    ```
    w3m 'url'
    ```
-------
# check version os and hardware[⬆️](https://github.com/monpopza/knowledge/blob/main/linux_command.md#linux-command)
  - show version os and name os
    ```
    for i in $(ls /etc/*release); do echo ===$i===; cat $i; done
    ```
  - show hardware (overview)
    ```
    lshw
    lshw -short
    ```
  - show pcie
    ```
    lspci
    lspci -vvv
    lspci -tree
    ```
  - show cpu
    ```
    lscpu
    ```
  - show block (disk tree/storage)
     ```
    lsblk
    lsblk --all
    ```
  - show usb 
    ```
    lsusb
    ```

-------
[⬅️](https://github.com/monpopza/knowledge) | [🏠](https://github.com/monpopza)
