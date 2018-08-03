# Question
Q1:ubuntu 解决“无法获得锁 /var/lib/dpkg/lock -open （11：资源暂时不可用）”的方法  
A1:强制解锁sudo rm /var/cache/apt/archives/lock  
          sudo rm /var/lib/dpkg/lock  
          
Q2：八代CPUi7装双系统  
A2：开机-F10-安全-安全引导配置-旧支持开启，安全引导禁用-F10保存-重启四数字验证回车。F9-引导设备选项-选择（KingstonDataTraveler 3.0PMAP）  
    开机连续点击F9-选SATA1
          
Q3:ubuntu更换源  
    sudo cp /etc/apt/source.list /etc/apt/source.list.bak  
    sudo gedit /etc/apt/source.list删除所有内容,负责163源  
    sudo apt-get update

Q4:vim : Depends: vim-common (= 2:7.4.052-1ubuntu3.1) but 2:7.4.273-2ubuntu4 is to be installed  
A4:        sudo apt-get purge vim-common  
          sudo apt-get update  
          sudo apt-get upgrade  
          sudo apt-get install vim
