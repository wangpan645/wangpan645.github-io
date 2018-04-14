---
title: 打造自己的ssr
date: 2018-04-13 14:44:26
tags: ssr
category: 
- 教程
- 科学上网
---
# Centos： #
## 一键脚本： ##
    yum -y install wget
    wget --no-check-certificate https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocksR.sh
    chmod +x shadowsocksR.sh
    ./shadowsocksR.sh 2>&1 | tee shadowsocksR.log
推荐 Centos 6.8

<!-- more -->
## bbr加速： ##
    yum -y install wget
    wget --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh
    chmod +x bbr.sh
    ./bbr.sh


 
# Debian： # 
## 一键脚本 ##

    wget --no-check-certificate https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocksR.sh
    chmod +x shadowsocksR.sh
    ./shadowsocksR.sh 2>&1 | tee shadowsocksR.log

推荐 Debian 7
注：如果在安装过程中，出现：

Media change: please insert the disc labeled‘Debian GNU/Linux 7.0.0 Wheezy — Official amd64 CD 等信息，其实是 apt源 的问题。

更换apt源：


    wget -N --no-check-certificate -P /etc/apt https://softs.fun/Bash/sources/us.sources.list
    rm -rf /etc/apt/sources.list
    cp /etc/apt/us.sources.list /etc/apt/sources.list


## 锐速加速： ##

    wget -N --no-check-certificate https://raw.githubusercontent.com/91yun/serverspeeder/master/serverspeeder.sh
    && bash serverspeeder.sh
备用地址：

    wget -N --no-check-certificate https://raw.githubusercontent.com/91yun/serverspeeder/master/serverspeeder-all.sh
    && bash serverspeeder-all.sh

卸装锐速脚本：

    chattr -i /serverspeeder/etc/apx* && /serverspeeder/bin/serverSpeeder.sh uninstall -f

## 各项命令如下： ##

重启锐速

    /serverspeeder/bin/serverSpeeder.sh restart

启动锐速

    /serverspeeder/bin/serverSpeeder.sh start

停止锐速

    /serverspeeder/bin/serverSpeeder.sh stop

查看锐速运行情况

    /serverspeeder/bin/serverSpeeder.sh status


# 逗比一键脚本：#
    wget -N --no-check-certificate https://softs.fun/Bash/ssr.sh && chmod +x ssr.sh && bash ssr.sh
## 备用下载： ##

    `wget -N --no-check-certificate https://raw.githubusercontent.com/ToyoDAdoubi/doubi/master/ssr.sh && chmod +x ssr.sh && bash ssr.sh`
