# NodeJsDemo
* 部署
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
