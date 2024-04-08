---
title: 导出所有插件
---

``` bach
@echo off
for /F %%i in ('code --list-extensions') do @echo code --install-extension %%i >> install.bat
echo succeed
pause
```

