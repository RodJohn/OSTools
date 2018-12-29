
fiddler作用
代理PC浏览器
代理IE/EDGE
代理google
移动端抓包
过滤

# fiddler作用

Fiddler2 是一个使用本地 127.0.0.1:8888 的 HTTP 代理，
任何能够设置 HTTP 代理为 127.0.0.1:8888 的浏览器和应用程序都可以使用 Fiddler。

它能够记录客户端和服务器之间的所有 HTTP请求，可以针对特定的HTTP请求，分析请求数据、设置断点、调试web应用、修改请求的数据，甚至可以修改服务器返回的数据



# 代理PC浏览器


代理IE/EDGE

    点击file  选择captrue traffic  
    软件会自动将ie的代理服务设置为fiddler

代理google

    使用SwitchyOmega添加代理指向fiddler,并切换为fiddler



移动端抓包 

    1.前提条件
        app需要开启了允许抓包
    手机和PC要在同一个局域网
    
    2.手机设置代理
    1.android “设置”->“WLAN”，
    2.找到你要连接的网络，在上面长按，然后选择“修改网络”，
    3.弹出网络设置对话框，然后勾选“显示高级选项”
    4.在“代理”后面的输入框选择“手动”，
    在“代理服务器主机名”后面的输入框输入电脑的ip地址，
    在“代理服务器端口”后面的输入框输入8888，然后点击“保存”按钮。


3.fiddler

设置代理
1.启动   Fiddler， Tools > Fiddler Options，
2.勾选   Allow romote computers to connect



# 说明

webSession

不仅是单条session,Fiddler还支持保存所有抓取到的session(并支持导入)，这对于抓取可疑请求然后保存，并在之后随时分析这些请求是很有帮助的。

如果想要重新发送某些请求，可以选中这些请求，然后点击工具栏中的reply.就可以重新发送选中的这些请求。


详情和数据统计面板

1. Statistic。
关于HTTP请求的性能和其他数据分析

2. Inspectors。
分为上下两个部分，上半部分是请求头部分，下半部分是响应头部分。对于每一部分，提供了多种不同格式查看每个请求和响应的内容

3. AutoResponder
Fiddler比较重要且比较强大的功能之一。可用于拦截某一请求，并重定向到本地的资源，或者使用Fiddler的内置响应。

4. Filter
Fiddler另一个比较强大的功能。Fiddler提供了多维度的过滤规则，足以满足日常开发调试的需求





5.host切换
1.当 Fiddler 已经建立会话时，任何修改 hosts 的行为都不会被 Fiddler 注意到
2.如果必须在建立会话时修改host,
	tool-->host-->enable remapping →
	手动编辑或者导入host(只是给fiddler本次使用)
	save as 



过滤

1.域名过滤
第一个选择 No Zone Filter
第二个按需
规则编写
*.baidu.com表示所有的百度二级域名会话；
*baidu.com表示一级域名+二级域名的会话


2.url过滤



6开启过滤
1.勾选useFilter,开启总开关  
2.actions-now  ,将刚刚的设置起效





参考资料
http://www.cnblogs.com/sunny-sl/p/6542375.html
http://blog.csdn.net/ohmygirl/article/details/17846199
