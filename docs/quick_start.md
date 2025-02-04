# 快速开始

## 前期工作

- [网络准备](network.md)
- 准备一台不小于 8 G内存的 64位 Centos 7 / Redhat 7 以上 Linux 主机；

#### 在线安装

 ```sh
 curl -sSL https://github.com/rackshift/rackshift/releases/latest/download/quick_start.sh | sh
 ```

#### 离线安装

* 下载最新 release 离线安装包
* tar -zxvf rackshiftVxx-offline.tar.gz
* cd rackshiftVxx-offline/installer
* ./install.sh

!!! warning "注意"
安装过程中需要您手动输入服务器上用作 PXE 的网卡 IP 地址作为 RackShift 服务器的 IP 地址
![runnob](https://f2c-south.oss-cn-shenzhen.aliyuncs.com/RackHD-dont-del/RackShift/config_network.jpg)

##### 安装过程截图

![runnbo](https://f2c-south.oss-cn-shenzhen.aliyuncs.com/RackHD-dont-del/RackShift/setup.jpg)

安装成功后您可以通过浏览器访问 RackShift WEB 控制台

``` sh
地址: http://ip:80
账号：admin
密码：123   

```

!!! info "控制命令"

- rsctl status 查看 RackShift 服务运行状态 - rsctl start 启动 RackShift 服务 - rsctl stop 停止 RackShift 服务 - rsctl restart 重启
  RackShift 服务 - rsctl reload 重新加载 RackShift 服务 - rsctl reconfig 重设 RackShift 服务 IP（PXE 网卡） 地址 - rsctl upgrade 升级
  RackShift 至最新版本 - rsctl uninstall 卸载 RackShift 服务 - rsctl version 查看 RackShift 版本信息