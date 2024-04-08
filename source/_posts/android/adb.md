---
title: adb 教程
---

## devices 
<!-- 显示 设备  -->
adb devices
<!-- 断开设备连接 -->
adb kill-server

## 安装apk
<!-- adb install <apk path> -->
adb install G:/test.apk
adb uninstall apk包名
## 显示包信息
<!--  打开 shell  终端-->
adb shell 
<!-- 显示 安装包名 -->
adb shell pm list package -f 

## 查看apk信息
<!-- android sdk -> build tools -->
aapt dump badging test.apk

## 查看进程
adb shell ps
adb shell "ps | grep 包名"

## 日志
adb logcat
<!-- 所有进程 -->
adb logcat -v process
<!-- 过滤进程 -->
adb logcat -v process | grep ***
<!--清除日志缓存 -->
adb logcat  -c
<!-- 保存日志 -->
adb logcat -v time > G:\log.txt
<!-- log level -->
– *V* : Verbose (明细);
– *D* : Debug (调试);
– *I* : Info (信息);
– *W* : Warn (警告);
– *E* : Error (错误);
– *F* : Fatal (严重错误);
– *S* : Silent(Super all output) (最高的优先级, 可能不会记载东西);

adb logcat WifiHW:D *:S*


<!-- 参考链接 -->
<https://blog.csdn.net/pony12/article/details/121538834>


adb logcat -v time | findstr com.DefaultCompany.OpenIM > G:\log.txt