




安装两个google浏览器

    Chrome
    Canary Chrome


tab
​    
    掘金

​    
​    

# 标签页

> 新建
>
> - mac	command + t
> - win         ctrl + t
>
> 关闭
>
> - mac	command + w 
> - win         ctrl + w
>
> 切换
>
> - ctrl  (shift)  tab  
>
> 选中地址栏
>
> - ctrl + l

​        





# 插件


## 导出

获取插件信息

    在 Chrome 浏览器上输入 chrome://extensions/ 打开拓展程序页面
    选中最上方的“开发者模式”，
    找到要导出的插件,复制这个插件的 ID 和 版本。       

查找安装文件

    Chrome 浏览器上输入 chrome://version/ 找到自己拓展程序在电脑的位置
    根据刚刚获取的id和版本定位安装文件的地址
    (如:C:\User\**\AppData\Local\Google\Chrome\User Data\Default\Extensions\niloccemoadcdkdjlinkgdfekeahmflj\3.0.3.0)

导出

    点击扩展管理页面最上方的 “打包扩展程序（package extension）”，
    在弹出的窗口中，填写刚刚获取的地址，私钥不用填
    点击打包
    在刚刚的id文件夹下会生成相应的crx文件(pem文件不用管)    


参考

    https://juejin.im/post/5ac044c75188251fc32967fd?utm_source=gold_browser_extension

