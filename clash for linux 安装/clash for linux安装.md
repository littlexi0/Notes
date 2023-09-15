# clash for linux 安装

## 安装

1、打开终端，输入`wget https://github.com/Dreamacro/clash/releases/download/v1.17.0/clash-linux-amd64-v1.17.0.gz`下载clash安装包

2、解压命令`gunzip clash-linux-amd64-v1.17.0.gz`

3、使用以下命令将解压后的文件移动到 `/usr/local/bin` 目录，并重命名为 `clash`  

`sudo mv clash-linux-amd64-v1.17.0 /usr/local/bin/clash`

4、使用以下命令给 Clash 添加执行权限：

`sudo chmod +x /usr/local/bin/clash`

安装完成（如果中途报错了，可能是网络不好

## 配置

1、使用以下命令创建 Clash 的配置文件目录

`mkdir -p ~/.config/clash`

2、使用以下命令下载订阅内容并保存为配置文件：

`curl https:/xxxx.yaml > ~/.config/clash/config.yaml`

注意将上面的`https:/xxxx.yaml`替换为你的实际订阅地址

Clash 的配置文件已经创建完成。

## 启动

使用以下命令启动 Clash：

`clash -d ~/.config/clash`

如果启动后还是访问不了外网，那么可以`ctrl+c`终止，然后重新启动尝试

