UpdateClient
============
Auto updateclient , can update acroos versions.


流程：

1、启动，访问服务器，请求xml

2、未联网，退出；需要更新，下载更新图片。用于界面显示

3、提示是否下载安装，关闭相关进程

4、http下载zip压缩包 

5、zip解压


支持启动参数：

//exe中传递的参数, 类似如下字符串, GetCommandLine前面包括当前exe路径

//http://10.0.40.18:8081/api/v1/version.xml?version=0.0.1&product=im

//c++中post的数据必须是UTF-8的编码