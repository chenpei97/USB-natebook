# USB
## 参考书籍


# 参考资料

官网：https://usb.org/  

USB项目开发详解：https://www.cnblogs.com/shenLong1356/p/11287833.html  
USB学习笔记：https://www.cnblogs.com/shenLong1356/p/11252977.html  
USB2.0概述及协议基础：https://www.jianshu.com/p/331d51b2c9dd  


CUBE建立USB工程：https://www.cnblogs.com/xingboy/p/9913963.html  
CUBE设置HID：https://blog.csdn.net/london_1/article/details/82855664  
基于stm32的自定义HID设备开发与上位机通讯实现：https://blog.csdn.net/github_37687123/article/details/80998607?utm_source=blogxgwz1  


# USB总线信号

## 基本状态  

|(D+,D-)|J状态|K状态|SE0状态|IDLE状态|
|---|---|---|---|---|
|低速|0,1|1,0|0,0|K|
|全速|1,0|0,1|0,0|J|
|高速|1,0|0,1|0,0|SE0|

## 基本信号  

|信号|状态|
|---|---|
|reset|SE0,10ms|
|resume|K,20ms+低速EOP|
|suspend|J,3ms|
|SOP|IDLE->K|
|EOP|SE0,2位时间+J,1位时间|
|SYNC|01:3个JK切换+2位时间|






