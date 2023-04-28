### 获取应用部署必须的程序与脚本
联系相关人


### 创建应用目录  
在D盘中创建audit目录，并将程序压缩包复制到此目录下解压  
解压后可以看到如下几个目录  
apps
web 
nginx 
sql_script 


### 初始化数据库  
进入D:\audit\sql_script，双击run.bat执行脚本


### 配置环境变量
在环境变量中配置如下两个参数  
AUDIT_USER：安装数据库时设置的用户名  
AUDIT_PWD：安装数据库时设置的用户密码


### 启动应用并加载到Windows服务(服务器重启后无需再次执行)
进入D:\nginx，双击执行install.bat  
进入D:\audit\apps\audit_server，双击执行server_install.bat  
进入D:\audit\apps\audit_mgmt，双击执行mgmt_install.bat  
进入D:\audit\apps\audit_message_socket，双击执行socket_install.bat  
