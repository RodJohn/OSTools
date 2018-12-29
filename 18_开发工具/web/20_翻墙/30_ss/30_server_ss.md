


# 1 购买 


## 1.1 分析

    别人搭建的服务器
    容易被封
    
## 1.3 常用 
    
    https://global.v2ss.info/
    
    https://get.ishadowx.net/


# 3 自建服务


## 3.1 分析

    自己玩
    套餐好
    
    
## 3.3 选择服务器

原则

    便宜
    可以使用国内支付手段
    网络访问无限制
    带宽和内存CPU最低就好
    

参考

    https://www.zhihu.com/question/20800554    
 
实践    
    

    阿里云
        香港服务器
        cpu 1G ,RAM 0.5G ,带宽 1Mbps
        按量收费(注意停机也会收钱)
    
    hostus
        便宜
    
    

       


## 3.6  linux搭建 

准备

    使用root用户


下载并运行脚本

    $ wget --no-check-certificate -O shadowsocks-all.sh https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocks-all.sh
    $ chmod +x shadowsocks-all.sh
    $ ./shadowsocks-all.sh 2>&1 | tee shadowsocks-all.log


配置

    按提示选择源码语言(go)，密码()、端口(80)、加密方式(aes-256-cfb)
    并等待脚本执行完毕

效果
    
    最终会显示以下效果，说明部署已完成
    
    Congratulations, your_shadowsocks_version install completed!
    Your Server IP        :11.11.11.11
    Your Server Port      :8989
    Your Password         :123456
    Your Encryption Method:aes-256-cfb
    
    Welcome to visit:https://teddysun.com/486.html
    Enjoy it    
    
防火墙

    开启防火墙
    阿里云要开启安全组



卸载

    $ ./shadowsocks-all.sh uninstall

