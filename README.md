socket协议
客户端请求
GET /HTTP/1.1
Upgrade:websocket(告诉服务器升级到websocket)
Connection:Upgrade
Sec-WebSocket-Key: xxx (BASE64加密的密钥)
Sec-WebSocket-Version:13 (告诉服务器ws的版本)
Origin:xxx
服务端响应
HTTP/1.1 101  Switching Protocols(协议切换)
Content-Length:0
Upgrade:websocket
Sec-Websocket-Accept:xxxx
Connection:Upgrade