
1. Yukle
1.  [![](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy?template=https://github.com/enesproovp/shadow-proxy/tree/re)，[一键部署到heroku](https://heroku.com/deploy?template=https://github.com/enespropvp/shadow-proxy/tree/re)
  
    也可以选择另一个版本的服务端[shadowsocks-websocket-python](https://github.com/onplus/shadowsocks-websocket-python/blob/deploy/README.md)；**手机用户建议部署跨平台支持更好的[v2ray](https://github.com/onplus/v2hero)**

1. 设置 加密算法和app 密码

![deploy](https://user-images.githubusercontent.com/31188782/31343896-ab0a868a-ad43-11e7-8a83-369cf5e385b0.jpg)

[](https://user-images.githubusercontent.com/31188782/31310674-e783c9e4-abce-11e7-87d2-48f328e74169.JPG)

支持的加密算法类型如下https://github.com/mrluanma/shadowsocks-heroku#supported-ciphers

## 启动本地 Client
1. 下载release https://github.com/enespropvp/shadow-proxy/releases （[备份](https://github.com/onplus/archive/tree/master/tool)）

2. 修改config.json参数，运行ss-h.exe 或 start.vbs (或 [win托盘工具taskbar.exe](https://github.com/onplus/shadowsocks-heroku/issues/39))

5. 启动成功，命令行显示：`server listening at { address: '127.0.0.1', family: 'IPv4', port: 1080 }`

## 配置代理
1. 下载：Chrome 浏览器 [SwitchyOmega](https://github.com/FelisCatus/SwitchyOmega/releases) 插件（[参考教程](https://github.com/FelisCatus/SwitchyOmega/wiki/GFWList), 导入备份文件[SSHeroku.Bak.zip](https://github.com/onplus/shadowsocks-heroku/files/1371313/SSHeroku.zip)）

2. 安装：打开浏览器的扩展程序页面 `chrome://extensions`，把 `SwitchyOmega.crx` 文件拖放到浏览器扩展程序页面安装 

3. 配置：添加SwitchyOmega代理服务器
```
    代理协议： SOCKS5
    代理服务器local_address：127.0.0.1 
    代理端口local_port： 1080 
```
    
## 可选：
1. 使用无污染DNS https://www.zhihu.com/question/32229915
2. cow/meow智能代理  https://github.com/cyfdecyf/cow#cow-climb-over-the-wall-proxy
```
    #rc配置文件
    listen = http://127.0.0.1:7777
    proxy = socks5://127.0.0.1:1080
```
3. 网站导航 http://www.ipv6daohang.com/
