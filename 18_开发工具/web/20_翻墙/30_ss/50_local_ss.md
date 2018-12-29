

# 下载

    https://github.com/shadowsocks/shadowsocks-windows/releases

# 使用

    https://github.com/shadowsocks/shadowsocks-windows

# 特别说明


## 模式

    系统模式
    
        所有网站默认走代理
    
    PAC模式(推荐)
        
        在连接网站的时候读取PAC文件里的规则，来确定你访问的网站有没有被墙，
        如果符合，那就会使用代理服务器连接网站，
        而PAC列表一般都是从GFWList更新的
            
    


# 服务

给服务器做代理

https://luzeshu.com/blog/shadowsocks




{
  "server":"104.128.235.156", 
  "server_port":9000,
  "local_address": "127.0.0.1",
  "local_port":1080,
  "password":"ss0330_#",
  "timeout":300,
  "method":"aes-256-cfb",
  "workers": 1
}
