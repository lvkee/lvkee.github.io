---
title: article title
date: 2022-04-06 10:04:02
tags:
---

# 1. bean 创建错误

可以检查一下是否正确导包。

# 2. 切面类不起作用

```xml
<bean id="paramValidAspect" class="com.sy.component.LoginComponent"/>
<aop:aspectj-autoproxy proxy-target-class="true"/>
```
在定义AOP的切面自动代理属性时同时应创建切面类的bean对象。

# 3. mybatis map dao导致报错
可以如图，在res文件夹中创建与java文件夹中dao包相同的package路径，在编译时会将此dao包和res中创建的dao文件夹整合在同一个文件夹中。
[![qf54SI.png](https://s1.ax1x.com/2022/03/31/qf54SI.png)](https://imgtu.com/i/qf54SI)
