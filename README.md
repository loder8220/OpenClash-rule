# OpenClash-rule
Openclash规则模板，被墙的常用公司域名设置域名集并设置策略组，其他被墙公司域名使用geosite:gfw匹配国外策略组，其他（国内、没有设置域名集、没被墙的）公司域名直连。    
根据机场节点位置设置分组。   

## subconverter后端Docker安装
**安装命令**：docker run -d --restart=always -p 25500:25500 tindy2013/subconverter:latest    

**检查命令（SSH连接openwrt执行命令）**：curl http://localhost:25500/version     

如果出现 subconverter vx.x.x backend 则说明容器已经成功运行。     
如果容器无法启动  重启docker ！     

**路由器本机docker地址**：http://localhost:25500/sub      

**自定义模板地址**：https://raw.githubusercontent.com/loder8220/OpenClash-rule/refs/heads/main/Clash-Full.ini     
