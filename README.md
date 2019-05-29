# SoftEnter-VPN
Install Soft enter VPN In Centos7

# 1.在安装前我们需要安装它的依赖库如下：
    yum -y install gcc zlib-devel openssl-devel readline-devel ncurses-devel
#安装Softenter server端到centos7
#在官网找到下载地址;https://github.com/SoftEtherVPN/SoftEtherVPN_Stable/releases/download/v4.29-9680-rtm/softether-vpnserver-v4.29-9680-rtm-2019.02.28-linux-x64-64bit.tar.gz
#下载 
    wget https://github.com/SoftEtherVPN/SoftEtherVPN_Stable/releases/download/v4.29-9680-rtm/softether-vpnserver-v4.29-9680-rtm-2019.02.28-linux-x64-64bit.tar.gz
#解压

    tar xzvf softether-vpnserver-v4.29-9680-rtm-2019.02.28-linux-x64-64bit.tar.gz
#安装

    cd vpnserver
    make
    [root@vultr vpnserver]# make
    --------------------------------------------------------------------

    SoftEther VPN Server (Ver 4.29, Build 9680, Intel x64 / AMD64) for Linux Install Utility
    Copyright (c) SoftEther Project at University of Tsukuba, Japan. All Rights Reserved.

    --------------------------------------------------------------------


    Do you want to read the License Agreement for this software ?

     1. Yes
     2. No

    Please choose one of above number:
    #选1 按流程完成安装过程
    
# 设置vpmcmd:

    ./vpncmd
    [root@vultr vpnserver]# ./vpncmd
    vpncmd command - SoftEther VPN Command Line Management Utility
    SoftEther VPN Command Line Management Utility (vpncmd command)
    Version 4.29 Build 9680   (English)
    Compiled 2019/02/28 19:22:54 by yagi at pc33
    Copyright (c) SoftEther VPN Project. All Rights Reserved.

    By using vpncmd program, the following can be achieved. 

    1. Management of VPN Server or VPN Bridge 
    2. Management of VPN Client
    3. Use of VPN Tools (certificate creation and Network Traffic Speed Test Tool)

    Select 1, 2 or 3: 1
    选择1管理VPN server 或者VPN Bridge.
    主机名或Hub名回车默认即可
    
# 设置管理员密码
    
    ServerPasswordSe
    VPN Server>ServerPasswordSe
    ServerPasswordSet command - Set VPN Server Administrator Password
    Please enter the password. To cancel press the Ctrl+D key.

    Password: ********
    Confirm input: ********


    The command completed successfully.
    输入两次管理员密码(1t*****)后Ctrl+C 退出
    
安装即完成 关于vpn服务端的设置可下载SoftEnter server 管理工具连接设置，参考https://blog.csdn.net/qq_39591494/article/details/78625394


 
