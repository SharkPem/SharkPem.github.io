---
title: Mac的Dock栏消失的解决方案
tags: Other

typora-root-url: ../../sharkpem.github.io
---

**MacOS版本：MacOS Big Sur 11.2**

当我们在设置中打开**自动隐藏和显示程序坞**时，出现了不显示程序坞，或者不想显示程序坞，以及使用了Pock这款Touch Bar软件又不想使用的话，可以参考下面的指令：

通常系统默认为1s。

打开终端，根据你所需的时间自行选择，10秒是10秒后才出现的意思。

```tex
# 先修改停留时间（后面数字为停留时间）如：
defaults write com.apple.dock autohide-delay -int 0      ##（时间设为最短）
defaults write com.apple.dock autohide-delay -int 0.5    ##（时间设为 0.5s）
defaults write com.apple.dock autohide-delay -int 10     ##（时间设为 10s）
#使设置生效
killall Dock
```

