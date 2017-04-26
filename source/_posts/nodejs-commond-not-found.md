---
title: nodejs commond not found
date: 2017-04-24 23:16:52
tags:
---

### Create a new post

``` bash
本文介绍了node.js包管理工具npm安装模块后，无法通过命令行执行命令，
提示‘xxx’ 不是内部或外部命令的解决方法，给需要的小伙伴参考下。
```


一般出现这样的问题原因是npm安装出现了问题，全局模块目录没有被添加到系统环境变量。
Windows用户检查下npm的目录是否加入了系统变量PATH中，如果不存在需要手动添加，添加之后需要重新启动CMD控制台。

{% asset_img 20141120174238941.jpg This is an example image %}
{% asset_img "20141120174238941.jpg" "spaced title" %}
![](20141120174238941.jpg)
nodejs模块全局目录环境变量
npm目录可以使用npm命令去查找：npm config get prefix
好了，问题解决了吧，是不是超级简单实用呢，希望本文能对大家有所帮助。