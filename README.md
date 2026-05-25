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

## 版本列表

| 版本 | 发布日期 | Windows | Linux | Darwin | Release |
|---|---|---|---|---|---|
| **v2.0.1** | 2021-03-31 | [zip](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v2.0.1/aliyun-mq-csharp-sdk-2.0.1-windows.zip) | [tar.gz](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v2.0.1/aliyun-mq-csharp-sdk-2.0.1-linux.tar.gz) | [tar.gz](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v2.0.1/aliyun-mq-csharp-sdk-2.0.1-darwin.tar.gz) | [v2.0.1](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/tag/v2.0.1) |
| v2.0.0 | 2021-03-24 | [zip](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v2.0.0/aliyun-mq-csharp-sdk-2.0.0-windows.zip) | — | [tar.gz](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v2.0.0/aliyun-mq-csharp-sdk-2.0.0-darwin.tar.gz) | [v2.0.0](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/tag/v2.0.0) |
| v1.1.4 | 2019-11-06 | [zip](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v1.1.4/aliyun-mq-csharp-sdk-1.1.4-windows.zip) / [rar](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v1.1.4/aliyun-mq-csharp-sdk-1.1.4-windows.rar) | — | — | [v1.1.4](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/tag/v1.1.4) |
| v1.1.3 | 2019-02-01 | [rar](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v1.1.3/aliyun-mq-csharp-sdk-1.1.3-windows.rar) | — | — | [v1.1.3](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/tag/v1.1.3) |

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

SDK 接入与使用方式请参考[阿里云 RocketMQ .NET SDK 接入指南](https://help.aliyun.com/zh/apsaramq-for-rocketmq/cloud-message-queue-rocketmq-4-x-series/developer-reference/sdk-for-net)。
