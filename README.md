# OpenWRT-CI
云编译OpenWRT固件

官方版：
https://github.com/immortalwrt/immortalwrt.git

高通版：
https://github.com/VIKINGYFY/immortalwrt.git

# 固件简要说明：

固件每天早上4点自动编译。

固件信息里的时间为编译开始的时间，方便核对上游源码提交时间。

MEDIATEK系列、QUALCOMMAX系列、ROCKCHIP系列、X86系列。

# 目录简要说明：

workflows——自定义CI配置

Scripts——自定义脚本

Config——自定义配置


#自行增加的插件及组件

#补全linux系统管理指令
CONFIG_PACKAGE_sudo=y

#KMS服务器（内置编译失败）
CONFIG_PACKAGE_luci-app-vlmcsd=y

#DDNS动态域名解析系统
CONFIG_PACKAGE_luci-app-ddns=y

#DDNS依赖
CONFIG_PACKAGE_drill=y

#虚拟服务器
CONFIG_PACKAGE_luci-app-openvpn-server=y

#FTP服务器
CONFIG_PACKAGE_luci-app-vsftpd=y

#微信通知推送
CONFIG_PACKAGE_luci-app-wechatpush=y

#IPTV组播转换
CONFIG_PACKAGE_luci-app-msd_lite=y

#IPTV组播代理
CONFIG_PACKAGE_luci-app-omcproxy=y

#web服务器
CONFIG_PACKAGE_luci-app-uhttpd=y

#多端网盘-alist
CONFIG_PACKAGE_luci-app-alist=y

#网页版终端命令行
CONFIG_PACKAGE_luci-app-ttyd=y

#图形化监控
CONFIG_PACKAGE_btop=y

#全能推送PushBot
CONFIG_PACKAGE_luci-app-pushbot=y

#关机poweroff
CONFIG_PACKAGE_luci-app-poweroff=y

#阿里云盘aliyundrive-webdav
CONFIG_PACKAGE_luci-app-aliyundrive-webdav=y

#主题界面luci-theme-edge
CONFIG_PACKAGE_luci-theme-edge=y

#以上为自行增加的插件及组件
