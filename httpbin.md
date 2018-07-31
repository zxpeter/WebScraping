# Introduction to Httpbin
---Xuanwo's Blog

在所有需要做HTTP请求的开发过程中，总有一个这样的痛点：我发出去的请求到底是什么样子的？
特别是在一些需要签名和认证的场合，服务器只会冷冰冰的返回一个40x错误，你无从得知错误的具体详情.

### 1. httpbin是什么
httpbin是一个HTTP Request & Response Service，你可以向他发送请求，然后他会按照指定的规则将你的请求返回。这个类似于echo服务器，但是功能又比它要更强大一些。 
httpbin支持HTTP/HTTPS，支持所有的HTTP动词，能模拟302跳转乃至302跳转的次数，
还可以返回一个HTML文件或一个XML文件或一个图片文件（还支持指定返回图片的格式）。

### 2. httpbin怎么用
httpbin的使用方法非常简单，你只需要把请求的地址修改为httpbin.org即可。 比如：

### 3. 获取请求中的user-agent
请求：
curl http://httpbin.org/user-agent
返回：
{"user-agent": "curl/7.19.7 (universal-apple-darwin10.0) libcurl/7.19.7 OpenSSL/0.9.8l zlib/1.2.3"}

