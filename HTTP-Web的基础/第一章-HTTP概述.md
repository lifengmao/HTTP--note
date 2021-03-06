HTTP概述
====
本章是对HTTP进行了简单介绍。包含了以下几个方面：<br>
```
Web客户端与服务器之间的通信
Web内容资源的出处
Web事务是怎样工作的
HTTP报文格式
TCP网络传输
不同的HTTP协议变体
HTTP架构组件中的一部分
```
因特网的多媒体信使
----
HTTP使用的是可靠的数据传输协议。<br>
Web客户端和服务器
----
客户端会向服务器发送HTTP请求，服务器会在HTTP响应中回送所请求的数据。服务器和客户端构成了万维网的基本组件。<br>
资源
----
Web服务器是Web资源的宿主。Web资源是Web内容的源头。所有类型的内容来源都是资源。<br>
###媒体类型
Web服务器会为所有HTTP对象数据加一个MIME类型。MIME是一种文本标记，表示一种主要的对象类型和一个特定的子类型，中间由一条斜杠来分隔。<br>
```
HTML:text/html
ASCII:text/plain
JPEG:image/jpeg
GIF: image/gif
QuickTime: video/quicktime
PowerPoint: application/vnd.ms-powerpoint
```
###URI
服务器的资源名被称为统一资源标识符（Uniform Resource Indetifier,URI）。它有两种形式：URL和URN。<br>
###URL
URL（统一资源定位符）是资源标识符最常见的形式。它通常包含协议、服务器和本地资源等信息。<br>
###URN
URN（同一资源名）是作为特定内容的唯一名称使用的，与目前资源所在地无关。 仍处于试验阶段。<br>
事务
----
一个HTTP事务由一条请求命令和一个响应结果组成。这种通信是通过HTTP报文的格式化数据块进行的。<br>
###方法
HTTP支持集中不同的请求命令，这些命令被称为HTTP方法。每条HTTP请求报文都包含一个方法。<br>
```
GET 从服务器向客户端发送命名资源
PUT 将来自客户端的数据存储到一个命名的服务器资源中
DELETE 从服务器删除命名资源
POST 将客户端数据发送到一个服务器网关应用程序
HEAD 仅发送命名资源响应中的HTTP首部
```
###状态码
每条HTTP报文响应时都会携带一个状态码。状态码是一个三位数字的代码，告知客户端请求是否成功。<br>
###Web页面可包含多个对象
一个Web页面通常不是单个资源而是一组资源的集合<br>
报文
----
HTTP报文都是纯文本，不是二进制代码，它一般包含起始行、首部字段和主体。<br>
连接
----
TCP提供了：
```
无差错的数据传输
按序传输
未分段的数据流
```
协议版本
----
略<br>
Web结构组件
----
```
代理
位于客户端和服务器之间的HTTP中间版本
缓存
HTTP的仓库
网关
连接其他应用程序的特殊Web服务器
隧道
对HTTP通信报文进行盲转发的特殊代理
Agent代理
发起自动HTTP请求的半智能Web客户端
```


