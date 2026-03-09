# docker-app-phantun

> 规范名称：`docker-app-phantun`
> 底层核心项目：`phantun`
> 对应 LuCI 插件：`luci-app-phantun`

`docker-app-phantun` 是一个面向 `phantun` 的 Docker 化管理端项目，用于统一管理服务端 / 客户端实例、持久化配置，并与 OpenWrt 侧 `luci-app-phantun` 在命名与职责上保持一致。

## 特性

- 基于 Go 的轻量化实现
- 支持 Client / Server 双模式管理
- 提供 Web UI、日志广播与运行状态查看
- 支持 TUN / iptables 相关运行环境
- 与 `openwrt-reyan_new/luci-app-phantun` 逻辑对齐

## 快速开始

```bash
git clone https://github.com/iHub-2020-Org/docker-app-phantun.git
cd docker-app-phantun
docker compose up -d --build
```

访问：`http://localhost:8080` 或服务器 IP 对应端口。

## 命名说明

本项目历史上曾使用 `phantun-docker` 作为仓库名称。现统一规范为：

- Docker 项目：`docker-app-phantun`
- LuCI 插件：`luci-app-phantun`
- 核心后端：`phantun`
