---
layout: post
title:  "windows telnet 回显"
date:   2016-11-24 20:45:18 +0800
categories: windows
---
windows默认是没有打开telent功能的，需要手动启用：
打开`控制面板`----`程序`----`启用或关闭Windows功能`----打开telnet客户端。
在cmd中输入telnet，进入Microsoft Telnet>命令提示符下，输入`help`
显示：
<img src="/file/telnet1.png"/>
输入`set ?`
显示：
<img src="/file/telnet2.png"/>
输入 `set localecho`
输入`quit`退出
<hr>
测试：
`telnet www.baidu.com 80`
按下ctrl+],回车
输入`GET / HTTP/1.1`回车 再回车
显示的是get请求后服务器的响应信息
