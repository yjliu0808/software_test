### Jmeter学习

https://www.bilibili.com/video/BV1SQ4y1M7s1?from=search&seid=10217912523307144830

（学习链接来源）

Jmeter录制脚本

Jmeter是Apche公司使用Java平台开发的一款测试工具

Jmeter可以做：接口测试、性能测试、压力测试、数据库测试、Java程序测试

Jmeter优点：开源免费、支持多协议（http/udp等）、轻量级、功能强大

Jmeter:无法验证JS程序，也无法验证页面的UI，所以要和Selenium配合完成Web应用测试

#### Jmeter安装

- 需要JAVA环境

- 在官方下载（官方地址：http://jmeter.apache.org/download_jmeter.cgi）

- 解压后，进入jmeter路径的bin目录双击jmeter.bat即可（linux启动Jmeter，/Jmeter/bin  找到jmeter.sh）

- https://jmeter-plugins.org/install/Install/（jmeter插件地址）

  Download **[plugins-manager.jar](https://jmeter-plugins.org/get/)** and put it into **`lib/ext`** directory, then restart JMeter.

#### Jmeter目录文件

- bin目录下的文件作用：

  1. examples 		目录中有CVS样例  

  2.  jmeter.bat       windows启动文件

  3. jmeter.log jmeter       运行日志文件

  4. jmeter.sh                  linux的启动文件

  5. jmeter.properties              系统配置文件    （配置文件修改，重启后生效）

  6. jmeter-server.bat windows             分布测试要用到的服务器配置

  7. jmeter-server  linux分布式测试要用到的服务器配置

     注：其中系统配置文件中的SSL设置重点关注如下几个：#指定https协议层 https=http+TLL

     https.default.protocol=TLS

- docs接口文档目录：D:\Program Files\apache-jmeter-5.2.1\apache-jmeter-5.2.1\docs\api

- extras目录放插件目录，提供了Ant的支持，可以使用Ant批量执行脚本实现自动化测试

     D:\Program Files\apache-jmeter-5.2.1\apache-jmeter-5.2.1\extras

- lib目录：存放Jar包，D:\Program Files\apache-jmeter-5.2.1\apache-jmeter-5.2.1\lib

- licenses： jmeter证书

- printable_docs目录：用户手册

   D:\Program Files\apache-jmeter-5.2.1\apache-jmeter-5.2.1\printable_docs\usermanual

  其中printable_docs/usermanual/component_reference.html)------核心帮助用户使用手册

#### Jmeter入门脚本

- 添加测试计划：默认有，不需要新建

  添加线程组>添加http请求>配置http(名称、协议、服务器名称或ip、http请求方法)>

  线程组下面添加监听器的查看结果树

- 线程组

​       线程数：虚拟用户数量

​       Ramp-up:规定时间内启动线程数

​       循环次数：线程的循环次数&永远（死循环）stop停止

- 取样器

  作用：向服务器发送请求并记录响应的信息和响应的时间

- 监听器：查看结果

- jmeter运行原理：按照线程方式运行

  ​    jmeterGUI模式运行测试脚本对电脑本身的资源消耗较大，无法实现大的并发和压力测试

  ​    使用命令行模式实现高并发和压力测试

  ​    使用GUI模式主要目的是编写和调试jmeter测试脚本

- jmeter测试计划要素：

  ​	测试计划、在测试计划至少有一个线程组、在线程组至少有一个取样器、在测试计划中必须要有监听器

#### 一、jmeter录制脚本

##### 1.用badboy录制（安装badboy、）

1. 打开badboy在地址栏输入被测网址回车
2. 打开badboy时默认记录状态，输入网址直接操作即可
3. 操作完成。。点击停止记录
4. 导致脚本（file-export to jmeter）保存
5. 在jmeter中打开已有文件
6. jmeter脚本文件的后缀明名.jmx
7. 在jmeter点击打开文件，选择文件路径找到需要的文件进行打开
8. 在jmeter执行之前要添加监听器

##### 2.使用jmeter自身代理录制移动端

1. 配置jmeter
   - 打开jmeter创建新的测试计划
   - 在测试计划下添加一个线程组
   - 添加http代理服务器（在测试计划下-右键-非测试元件-http代理服务） 

1. 配置http代理服务器
   - 端口号默认
   - http domains中填写电脑本地ip或localhost
   - 目标控制器选择 测试计划>线程组
   - 点击启动按钮---点击ok

1. 配置手机代理和电脑ip一直即可 

#### 二、jmeter核心



























