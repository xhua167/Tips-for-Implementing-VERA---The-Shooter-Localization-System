# Tips-for-Implementing-VERA---The-Shooter-Localization-System




1) If you started the server once in local machine, next time remember to check whether there are any existing process bounded to localhost with using following codes:                   
$ ps -fA | grep python               
501 81651 12648   0  9:53PM ttys000    0:00.16 python -m SimpleHTTPServer                
Then kill the second number with following command:            
$ kill 81651                     

2) 本地安装mysql（路径:./url/local/mysql)              
使用如下指令在terminal中打开mysql:                
$/usr/local/mysql/bin/mysql -uroot -p              
输入密码               
在mysql commandline用一下指令将initial.sql导入指定database:                   
$use dbname               
$source 绝对路径/initial.sql                      
