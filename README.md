# JetBrains_Cracked
激活包括pycharm等工具

mac下激活方式 https://www.cnblogs.com/gdutxiaoxu/p/17098362.html
复制方式3中jetbra到某个路径，不能包含中文与空格
之后，打开终端，进入到 /jetbra/scripts 文件夹， 执行 install.sh 脚本, 命令如下：
sudo bash install.sh
正常返回done.表示执行成功。
其他异常：
Could not set environment: 150: Operation not permitted while System Integrity Protection is engaged
chmod 777 install.sh
sudo bash install.sh 如果还是不行 使用./install.sh
执行如下口令，修改环境变量的属主为当前用户。
sudo chown 用户名 .profile
sudo chown 用户名 .jetbrains.vmoptions.sh
./install.sh        
./install.sh: line 31: /Users/用户名/Library/LaunchAgents/jetbrains.vmoptions.plist: Permission denied

sudo chmod 777 /Users/用户名/Library/LaunchAgents/jetbrains.vmoptions.plist 
./install.sh                                                     
./install.sh: line 43: /Users/用户名/.jetbrains.vmoptions.sh: Permission denied

sudo chmod 777 /Users/用户名/.jetbrains.vmoptions.sh
./install.sh                                     
done. the "kill Dock" command can fix the crash issue.

illegal byte aequence
执行如下命令，再执行脚本
export LC_COLLATE='C'
export LC_CTYPE='C'

