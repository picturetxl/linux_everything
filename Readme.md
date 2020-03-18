## 切换源



### 先备份原先的源文件

```shell
sudo cp /etc/apt/sources.list /etc/apt/sources_bk.list
```



### 打开source.list,复制进阿里云镜像

```shelll
deb http://mirrors.aliyun.com/ubuntu/ trusty main restricted universe multiverse
deb http://mirrors.aliyun.com/ubuntu/ trusty-security main restricted universe multiverse
deb http://mirrors.aliyun.com/ubuntu/ trusty-updates main restricted universe multiverse
deb http://mirrors.aliyun.com/ubuntu/ trusty-proposed main restricted universe multiverse
deb http://mirrors.aliyun.com/ubuntu/ trusty-backports main restricted universe multiverse
deb-src http://mirrors.aliyun.com/ubuntu/ trusty main restricted universe multiverse
deb-src http://mirrors.aliyun.com/ubuntu/ trusty-security main restricted universe multiverse
deb-src http://mirrors.aliyun.com/ubuntu/ trusty-updates main restricted universe multiverse
deb-src http://mirrors.aliyun.com/ubuntu/ trusty-proposed main restricted universe multiverse
deb-src http://mirrors.aliyun.com/ubuntu/ trusty-backports main restricted universe multiverse
```

### 更新源和软件

```shell
sudo apt-get update 
sudo apt-get upgrade
```





## zsh 的折腾



### 安装

```shell
sudo apt-get install -y zsh
sudo apt-get install wget
```



### 主题-oh  my zsh

[oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh/)

```shell
sh -c "$(wget https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"
```

### 配置文件

```shell
~/.zshrc
```





### 设置zsh为系统登陆终端

```shell
chsh -s `which zsh`
```











## vscode 的折腾





### vscode 与git

