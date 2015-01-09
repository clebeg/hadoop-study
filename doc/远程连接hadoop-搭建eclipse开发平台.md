##远程连接Hadoop	搭建eclipse开发平台
hadoop集群搭建成功之后，我们需要利用这个集群为我们服务，
除了真正的hadoop管理人员需要经常登录服务器去维护之外，
普通开发人员没有必要、也不安全经常去登录服务器
开发人员选择的平台一定要是linux，然后通过hadoop的权限控制，
非常方便管理不同开发团队不同的项目。

**由于搭建的是windows虚拟机hadoop伪分布平台，所以这里利用win7上的eclipse讲解**
**利用windows作为开发平台，权限没办法很好的控制，只能设置一个目录权限全无作为测试**
**但是搭建环境的过程与linux是完全类似的**

###一、环境介绍
```
centos7	注意centos7利用systemctl来管理服务
jdk7
hadoop2.6.0
eclipse j2ee 版本
```

###二、hadoop eclipse 运行环境搭建
参考：http://www.open-open.com/lib/view/open1418191526714.html

关键点：下载对应版本的hadoop-eclipse-plugin-*.jar
可以选择自己下载源码编译：不过它的源码是用ant编译的。
其实没有必要非得下载源码编译，下载别人编译好的jar包也可以。不过的小心哦！

提供一个下载地址：http://pan.baidu.com/s/1jGj64p4

###三、测试
测试代码git上都有，下载即可。
注意：
*hadoop的文件目录地址需要用 hdfs://ip:port/../..指定
*目录是有读写权限的