# JetBrains_Cracked
激活包括pycharm等工具

mac下激活方式 https://www.cnblogs.com/gdutxiaoxu/p/17098362.html<br>
复制方式3中jetbra到某个路径，不能包含中文与空格<br>
之后，打开终端，进入到 /jetbra/scripts 文件夹， 执行 install.sh 脚本, 命令如下：<br>
sudo bash install.sh<br>
正常返回done.表示执行成功。<br>
其他异常：<br>
Could not set environment: 150: Operation not permitted while System Integrity Protection is engaged<br>
chmod 777 install.sh<br>
sudo bash install.sh 如果还是不行 使用./install.sh<br>
执行如下口令，修改环境变量的属主为当前用户。<br>
sudo chown 用户名 .profile<br>
sudo chown 用户名 .jetbrains.vmoptions.sh<br>
./install.sh<br>
./install.sh: line 31: /Users/用户名/Library/LaunchAgents/jetbrains.vmoptions.plist: Permission denied<br>

sudo chmod 777 /Users/用户名/Library/LaunchAgents/jetbrains.vmoptions.plist<br> 
./install.sh<br>
./install.sh: line 43: /Users/用户名/.jetbrains.vmoptions.sh: Permission denied<br>

sudo chmod 777 /Users/用户名/.jetbrains.vmoptions.sh<br>
./install.sh<br>
done. the "kill Dock" command can fix the crash issue.<br>

illegal byte aequence<br>
执行如下命令，再执行脚本<br>
export LC_COLLATE='C'<br>
export LC_CTYPE='C'<br>

