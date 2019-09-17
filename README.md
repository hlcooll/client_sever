客户端服务端

#from socket import *
#AttributeError: type object 'socket' has no attribute 'socket' 错误

导入套接字，然后从套接字导入*。
由于socket中有一个socket函数，当你调用socket.socket时，python很可能会混淆并使用socket内的socket。

#修改为：
import socket
socket.socket # <class 'socket.socket'>
