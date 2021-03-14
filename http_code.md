## **HTTP 状态码总结**

* **1xx**
  - 100 Continue 继续
  - 101 Switching Protocols 装换协议，http1.1新加入的

* **2xx**
  - 200 OK 返回正常
  - 201 Created 创建正常，表示已经在请求的中创建了相应的文档
  - 202 Accepted 告诉客户端， 请求在执行中了，但是还没执行完
  - 203 Non-Authoritative Information 非官方的信息，意思是这个是正在使用的文档副本，所以某些响应头信息可能不正确
  - 204 No Content 无内容
  - 205 Reset Content 重置了内容
  - 206 Partial Content 部分内容

* **3xx**
  - 300 Multiple Choices 多重选择
  - 301 Moved Permanently 请求的内容被放到别的地方了
  - 302 Found 找到了只是找到的是临时的url
  - 303 See other
  待更新

* **4xx** 这个一般式客户端的锅
  - 400 Bad Request请求错误
  - 401 Unauthorized 未授权。身份有问题
  - 402 要充值，一般没啥用，以后比特币什么的估计御用
  - 403 Forbidden 标志没有授权，禁止通行
  - 404 Not Found 这个很常见
  - 405 Method Not Allowed 请求的方法有问题，一般是GET POST 这些用错了
  - 406 Not Accepted 无法访问， Accept头信息指定的类型不一致
  - 407 Proxy Authentication Requried 代理服务器的认证要求 和 401 一样，不过是针对代理的
  - 408 Request TimeOut 请求超时
  - 409 Confilct 冲突这个主要是PUT方法，修改的文档版本信息什么的不一致
  - 410 Gone 请求的文档不见了，这个和404不相同，只要是文档被移走了

* **5xx** 这个一般是服务器自己抽风了
  - 500 Internal Sever Error 内部服务器异常
  - 501 Not Implement 还没来实现
  - 502 Bad Gateway 错误的网关
  - 503 Service Unavailable 服务器在维护或者什么的没有响应了
  - 504 Gateway Timeout 超时了
  - 505 Http version not support http的版本不支持
