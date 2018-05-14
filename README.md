# shadowsocks
使用shadowsocks的一点方法
## 终端连接ssh
terminal命令终端，ssh 登录名@服务器地址，如 ssh root@12.12.12.12，enter键之后会提示你密码，登录名，服务器地址，密码。
## 错误一 清理当前终端内关于远程服务器的缓存与秘钥
ECDSA host key "ip地址" for has changed and you have requested strict checking错误。
输入 ssh-keygen -R "你的远程服务器ip地址"    
目的是清除你当前机器里关于你的远程服务器的缓存和公钥信息，注意是大写的字母“R”。  
## 为Debian / Ubuntu 安装shadowsocks服务端:  
$ apt-get install python-pip  
$ pip install shadowsocks
## 为Centos 安装shadowsocks服务端:
$ yum install python-setuptools  
$ easy_install pip  
$ pip install shadowsocks
## pip install 环节错误  
Command "python setup.py egg_info" failed with error code 1 in /tmp/pip-install-RW_sjI/shadowsocks/
sudo python -m pip install --upgrade --force pip 
sudo pip install setuptools==33.1.1

