### **标题1：OSI模型**

#### 1.1定义

开放式系统互联通信参考模型 ，简称OSI模型，一种概念模型，由国际标准化组织提出，一个试图使各种计算机在世界范围内互连为网络的标准框架。

 OSI将[计算机网络体系结构](https://baike.baidu.com/item/计算机网络体系结构)(architecture）划分为以下七层 ：

 ![img](https://bkimg.cdn.bcebos.com/pic/77c6a7efce1b9d16a9ef96c9f2deb48f8c546469?x-bce-process=image/watermark,g_7,image_d2F0ZXIvYmFpa2U4MA==,xp_5,yp_5) 

 [物理层](https://baike.baidu.com/item/物理层): 将数据转换为可通过物理介质传送的[电子信号](https://baike.baidu.com/item/电子信号) 

 [数据链路层](https://baike.baidu.com/item/数据链路层): 决定访问网络介质的方式。 

 在此层将数据分帧，并处理流控制。本层指定[拓扑结构](https://baike.baidu.com/item/拓扑结构)并提供硬件寻址，相当于邮局中的装拆箱工人。 

 [网络层](https://baike.baidu.com/item/网络层/4329439): 使用权数据路由经过大型网络 相当于邮局中的排序工人。 

 [传输层](https://baike.baidu.com/item/传输层): 提供终端到终端的可靠连接 相当于公司中跑邮局的送信职员。 

 [会话层](https://baike.baidu.com/item/会话层): 允许用户使用简单易记的名称建立连接 相当于公司中收寄信、写信封与拆信封的秘书。

 [表示层](https://baike.baidu.com/item/表示层): 协商数据交换格式 相当公司中简报老板、替老板写信的助理。  

 [应用层](https://baike.baidu.com/item/应用层/4329788): 用户的应用程序和网络之间的接口。 

#### 1.2层次划分

根据建议X.200，OSI将计算机网络体系结构划分为以下七层，标有1～7，第1层在底部。 现“OSI/RM”是[英文](https://baike.baidu.com/item/英文)“Open Systems Interconnection Reference Model”的缩写。

- ### 第7层 应用层

主条目：[应用层](https://baike.baidu.com/item/应用层)

应用层（Application Layer）提供为应用软件而设的接口，以设置与另一应用软件之间的通信。例如: HTTP，HTTPS，FTP，TELNET，SSH，SMTP，POP3等。

- ### 第6层 表达层

主条目：表达层

表达层（Presentation Layer）把数据转换为能与接收者的系统格式兼容并适合传输的格式。

- ### 第5层 会话层

主条目：[会话层](https://baike.baidu.com/item/会话层)

会话层（Session Layer）负责在数据传输中设置和维护计算机网络中两台计算机之间的通信连接。

- ### 第4层 传输层

主条目：[传输层](https://baike.baidu.com/item/传输层)

传输层（Transport Layer）把传输表头（TH）加至数据以形成数据包。传输表头包含了所使用的协议等发送信息。例如:传输控制协议（TCP）等。

- ### 第3层 网络层

主条目：[网络层](https://baike.baidu.com/item/网络层)

网络层（Network Layer）决定数据的路径选择和转寄，将网络表头（NH）加至数据包，以形成分组。网络表头包含了网络数据。例如:互联网协议（IP）等。

- ### 第2层 数据链路层

主条目：[数据链路层](https://baike.baidu.com/item/数据链路层)

数据链路层（Data Link Layer）负责网络寻址、错误侦测和改错。当表头和表尾被加至数据包时，会形成帧。数据链表头（DLH）是包含了物理地址和错误侦测及改错的方法。数据链表尾（DLT）是一串指示数据包末端的字符串。例如以太网、无线局域网（Wi-Fi）和通用分组无线服务（GPRS）等。

分为两个子层：逻辑链路控制（logic link control，LLC）子层和介质访问控制（media access control，MAC）子层。

- ### 第1层 物理层

主条目：[物理层](https://baike.baidu.com/item/物理层)

物理层（Physical Layer）在局部局域网上传送[数据帧](https://baike.baidu.com/item/数据帧)（data frame），它负责管理计算机通信设备和网络媒体之间的互通。包括了针脚、电压、线缆规范、集线器、中继器、网卡、主机适配器等。

- **影响**

OSI是一个定义良好的协议规范集，并有许多可选部分完成类似的任务。它定义了开放系统的层次结构、层次之间的相互关系以及各层所包括的可能的任务，作为一个框架来协调和组织各层所提供的服务。

OSI参考模型并没有提供一个可以实现的方法，而是描述了一些概念，用来协调进程间通信标准的制定。即OSI参考模型并不是一个标准，而是一个在制定标准时所使用的概念性框架。

 ![img](https://s5.51cto.com/oss/201906/17/aaf923228df01d11a7b805d4db5d1d33.jpeg) 

 

### 标题2： TCP/IP协议 

#### 2.1定义

 Internet 是基于传送控制协议/网际协议(TCP/IP)协议族的，TCP/IP协议族分为5层：应用层、传输层、网际层、数据链路层和物理层。与OSI协议族不同的是，TCP/IP协议族没有表示层和会话层。图1.显示了TCP/IP与OSI对比的的不同层及其协议。 











