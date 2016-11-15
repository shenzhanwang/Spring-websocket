# Spring-websocket
  传统的HTTP协议，一般通过向服务器发送请求，拉取数据实现半双工通信，缺点是服务器难以直接向浏览器下发消息，因此，websocket协议应运而生，可用于向建立连接的浏览器主动下发任意数据（PUSH）。本项目基于Spring平台，整合websocket协议，实现一个简易web聊天室的功能。主要特性如下:
  
  1.包含聊天室登录、退出的功能。登录时，浏览器自动向服务器发起websocket连接，退出时自动切断。
  
  2.登录后，用户可查看到聊天室在线的用户列表，我们在服务器上通过一个hashmap始终记录了当前在线的用户列表；

  3.登录的用户可以点击一个在线的其他用户，并给他发送消息，消息先提交给服务器，在通过服务器转发给另一端用户；
  
  4.支持群发消息的功能，使用时，服务器会将收到的消息群发给当前在线的所有用户。
  
  效果图：
   ![alt text](https://github.com/shenzhanwang/Spring-websocket/blob/master/%E6%88%AA%E5%9B%BE/1.jpg)
   
   ![alt text](https://github.com/shenzhanwang/Spring-websocket/blob/master/%E6%88%AA%E5%9B%BE/2.jpg)
   
   
