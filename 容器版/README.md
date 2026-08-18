# docker容器版说明
1.安装docker，可自行搜索查阅 windows下的wsl2如何安装docker ....

2.安装+运行 (2种方式任选其一)
```
# 方式1 直接docker命令
docker run -d --name exvs2_local_stun -p 3478:3478/udp vl00at111/exvs2_local_stun

# 方式2 使用docker-compose.yml
# 安装docker-compose
cd "{docker-compose.yml所在目录}"
docker compose up -d
```

3.如果win主机用localhost或127.0.0.1访问无效, 请使用wsl2的ip, Powershell或cmd里运行获取该ip..
```
wsl hostname -I
```

4.刷卡配置一下
![](./media/容器版可能需要wsl2的ip及其sever.json的配置.png)