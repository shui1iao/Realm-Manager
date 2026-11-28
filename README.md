# Realm-Manager

[![Release](https://img.shields.io/github/v/release/shui1iao/Realm-Manager?style=flat-square&color=2563eb)](https://github.com/shui1iao/Realm-Manager/releases/latest)
[![Shell](https://img.shields.io/badge/Shell-Bash-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white)](realm.sh)
[![Platform](https://img.shields.io/badge/Platform-Linux%20amd64%20%7C%20arm64-1e293b?style=flat-square&logo=linux&logoColor=white)](https://github.com/shui1iao/Realm-Manager/releases)

**中文** | [English](README.en.md)

**轻量级 Realm 高性能端口转发一键管理脚本**——快速部署与维护 TCP / UDP 中转规则。

## 核心特性

- **核心一键维护**：自动下载安装与升级 Realm 核心（支持 `amd64` / `arm64`），升级后自动重启服务生效。
- **规则可视化管理**：交互式添加、查看与删除端口转发规则，支持 IPv4 / IPv6 与域名目标，内置严格地址校验防 TOML 配置注入。
- **稳定守护**：自动配置 systemd 后台服务，支持可选 cron 每日定时重启。

## 快速开始

### 方式一：短链一键运行（推荐）

```bash
bash <(curl -Ls https://realm.siaoz.si)
```

### 方式二：运行最新正式发布版

```bash
curl -fsSLO https://github.com/shui1iao/Realm-Manager/releases/latest/download/realm.sh
bash realm.sh
```

## 注意事项

- 面向 Linux root + systemd 环境，请在可信 VPS 上执行。
- 修改防火墙或端口转发规则前，建议保留一个活跃 SSH 连接以防失联。
