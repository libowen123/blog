从URL输入到页面展现
#1.URL是什么
- URL:统一资源定位符，用于定位互联网上的资源
- http、https、ftp、file协议
#2.域名解析
##1. 为什么要发明域名
- 域名便于记忆，具有语义化的作用
##2. 域名是什么
- 在http://jirengu.com:8080/blog中jirengu.com就是域名
##3. IP地址是什么
- 每个处于互联网中的设备都有IP地址，形如192.168.0.1
- 局域网IP和公网IP是有差别的
- 127.0.0.1代表本机IP
##4.浏览器解析的流程
###1.浏览器缓存
 - 浏览器会缓存DNS记录一段时间
###2.系统缓存
- 从hosts文件查找是否有该域名和对应IP
###3.路由器缓存
- 一般路由器也会缓存域名信息
###4.ISP DNS缓存
- 比如到电信的DNS上查找缓存
###5.如果都没找到，则向根域名服务器查找域名对应IP,根域名服务器把请求转发到下一级，直到找到IP
#3.服务器处理
- 服务器是一台安装系统的机器，常见的系统如Linux、windows sever 2012
- 系统里安装的处理请求的应用叫web sever
##web 服务器
- 常见的web服务器有Apache、Nginx、IIS、Lighttpd
- web服务器接收用户的Request交给网站代码，或者接受请求反向代理到其他web服务器
#4.网站处理流程
- MVC模型(model)-视图(view)-控制器(controller)
![图片发自简书App](http://upload-images.jianshu.io/upload_images/957126-9839e06a257eb66f.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1080/q/50)
#5.浏览器处理
- 1.HTML字符串被浏览器接受后被一句句读取解析
- 2.解析到link标签后重新发送请求获取css
- 3.解析到script标签后发送请求获取js，并执行代码
- 4.解析到img标签后发送请求获取图片资源
#6.绘制网页
- 浏览器根据HTML和CSS计算得到渲染树，绘制到屏幕上，js会被执行