# NodeJsDemo
* 部署Nodejs
* npm
* 语法
* 应用
-----
## 部署
### 安装Node.js
安装地址：https://nodejs.org/en/download/
* LTS=Long Team Support=官方版本
* Current=社区版本
* LTS8.0以后版本集成npm,无需额外安装

### 检查安装
检查环境变量是否包含nodejs的安装目录

        Windows + R -> cmd -> path

## npm
### set config
设置代理为null

        npm config set proxy null
        
or

        npm config delete proxy
        
设置https代理为null

        npm config set https-proxy null
        
or

        npm config delete https-proxy
        
设置证书校验

        npm config set strict-ssl false

### 使用npm引用express
全局安装

        npm install express -g
        
局部安装

        cd 项目路径
        npm init -f
        npm install express

## FirstDemo
```js
    // 使用 require 指令来载入 http 模块
    var http = require('http');
    
    // 创建服务器，并使用 listen 方法绑定 8080 端口
    // 通过 request, response 参数来接收和响应数据
    http.createServer(function (request, response) {

        // 发送 HTTP 头部 
        // HTTP 状态值: 200 : OK
        // 内容类型: text/plain
        response.writeHead(200, {'Content-Type': 'text/plain'});

        // 发送响应数据 "Hello World"
        response.end('Hello World\n');
    }).listen(8080);

    // 终端打印如下信息
    console.log('Server running at http://127.0.0.1:8080/');
```
        node server.js
        Server running at http://127.0.0.1:8888/
