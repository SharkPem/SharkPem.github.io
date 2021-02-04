---
title: Mac的Dock栏消失的解决方案
tags: Other

typora-root-url: ../../sharkpem.github.io
---

**MacOS版本：MacOS Big Sur 11.2**

当我们在设置中打开**自动隐藏和显示程序坞**时，出现了不显示程序坞，或者不想显示程序坞，以及使用了Pock这款Touch Bar软件又不想使用的话，可以参考下面的指令：

打开终端，根据你的需求选择

```tex
# 根据你的需求二选一：
defaults write com.apple.dock autohide-delay -int 0.5    ##（恢复自动隐藏和出现的功能，后面的数字0~1之间均可）
defaults write com.apple.dock autohide-delay -int 10     ##（禁止使用Dock栏隐藏和出现的功能，后面的数字大于1均可）
#使设置生效，这一步很重要
killall Dock
```

