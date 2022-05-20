# g0h3aler-frp-owner
修改frp特征及自删除配置文件，修改版本0.42.0

重复造轮子，网上已经有很多大佬修改过frp了，包含了特征值修改、配置文件参数化、域前置等等等

本项目主要改动
1、取特征化(不完全，最新版frp的tls特征值无法修改，可能自己太菜)
2、配置文件自删除，加载运行后自删除配置文件，防止在linux或者命令审计下泄露IP地址

具体使用：
在frpc.ini中的common中添加DeleteConfig = true即可
其他功能正常使用

参考
https://github.com/uknowsec/frpModify
https://uknowsec.cn/posts/notes/FRP%E6%94%B9%E9%80%A0%E8%AE%A1%E5%88%92.html
