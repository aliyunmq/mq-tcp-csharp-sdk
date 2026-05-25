# mq-tcp-csharp-sdk

RocketMQ 4.x TCP 协议 .NET (C#) SDK 二进制包归档仓库。

> ⚠️ **维护状态**：本 SDK 已停止更新，仅用于历史版本归档。新项目请使用基于 gRPC 协议的 RocketMQ 5.x SDK。

## 文件命名规范

```
aliyun-mq-csharp-sdk-{version}-{platform}.{ext}
```

- `version`：SDK 版本号，如 `1.1.3`、`2.0.1`
- `platform`：`windows` / `linux` / `darwin`
- `ext`：`zip` / `rar` / `tar.gz`

每个 Release 同时附带 `SHA256SUMS.txt` 用于完整性校验。

## 下载

最新版本 **v2.0.1**：

- [Windows amd64](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v2.0.1/aliyun-mq-csharp-sdk-2.0.1-windows.zip)
- [Linux amd64](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v2.0.1/aliyun-mq-csharp-sdk-2.0.1-linux.tar.gz)
- [Darwin amd64](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v2.0.1/aliyun-mq-csharp-sdk-2.0.1-darwin.tar.gz)

完整版本列表、变更日志与历史版本下载：[Releases](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases)

## 完整性校验

每个 Release 附带 `SHA256SUMS.txt`，下载后可校验：

```bash
# Linux / macOS
curl -LO https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v2.0.1/aliyun-mq-csharp-sdk-2.0.1-linux.tar.gz
curl -LO https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v2.0.1/SHA256SUMS.txt
shasum -a 256 -c SHA256SUMS.txt --ignore-missing
```

```powershell
# Windows
Get-FileHash aliyun-mq-csharp-sdk-2.0.1-windows.zip -Algorithm SHA256
```

## 使用文档

- [环境准备](https://help.aliyun.com/zh/apsaramq-for-rocketmq/cloud-message-queue-rocketmq-4-x-series/developer-reference/prepare-the-environment-2)
- [收发普通消息](https://help.aliyun.com/zh/apsaramq-for-rocketmq/cloud-message-queue-rocketmq-4-x-series/developer-reference/send-and-subscribe-to-normal-messages-2)
- [收发顺序消息](https://help.aliyun.com/zh/apsaramq-for-rocketmq/cloud-message-queue-rocketmq-4-x-series/developer-reference/send-and-subscribe-to-ordered-messages-8)
- [收发定时消息](https://help.aliyun.com/zh/apsaramq-for-rocketmq/cloud-message-queue-rocketmq-4-x-series/developer-reference/send-and-receive-scheduled-messages)
- [收发事务消息](https://help.aliyun.com/zh/apsaramq-for-rocketmq/cloud-message-queue-rocketmq-4-x-series/developer-reference/send-and-subscribe-to-transactional-messages-4)
- [订阅消息（集群与广播模式）](https://help.aliyun.com/zh/apsaramq-for-rocketmq/cloud-message-queue-rocketmq-4-x-series/developer-reference/subscribe-to-messages)
