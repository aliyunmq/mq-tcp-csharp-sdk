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

### v2.0.1 · 2021-03-31 · Latest

**主要变更**

- 修改 Quick Start 文档，添加使用 x64 目标库的提示说明。
- 修复 API 兼容性，修正 `Message#setBody(byte[] body, int size)` 方法。

**资产**

| 平台 | 文件 | 大小 | SHA256 |
|---|---|---:|---|
| Windows amd64 | [aliyun-mq-csharp-sdk-2.0.1-windows.zip](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v2.0.1/aliyun-mq-csharp-sdk-2.0.1-windows.zip) | 18.5 MB | `db5b1d33…45833` |
| Linux amd64 | [aliyun-mq-csharp-sdk-2.0.1-linux.tar.gz](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v2.0.1/aliyun-mq-csharp-sdk-2.0.1-linux.tar.gz) | 17.6 MB | `35f06add…c6961` |
| Darwin amd64 | [aliyun-mq-csharp-sdk-2.0.1-darwin.tar.gz](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v2.0.1/aliyun-mq-csharp-sdk-2.0.1-darwin.tar.gz) | 18.6 MB | `705ecb07…68832` |

更多详情：[Release v2.0.1](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/tag/v2.0.1) · [SHA256SUMS.txt](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v2.0.1/SHA256SUMS.txt)

---

### v2.0.0 · 2021-03-24

**主要变更**

- 通过 GraalVM，将功能点和 Java 与 C/C++ SDK 对齐。
- 解决共享库稳定性问题。

**资产**

| 平台 | 文件 | 大小 | SHA256 |
|---|---|---:|---|
| Windows amd64 | [aliyun-mq-csharp-sdk-2.0.0-windows.zip](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v2.0.0/aliyun-mq-csharp-sdk-2.0.0-windows.zip) | 42.7 MB | `8a312198…0968a` |
| Darwin amd64 | [aliyun-mq-csharp-sdk-2.0.0-darwin.tar.gz](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v2.0.0/aliyun-mq-csharp-sdk-2.0.0-darwin.tar.gz) | 16.7 MB | `80115217…38115` |

更多详情：[Release v2.0.0](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/tag/v2.0.0) · [SHA256SUMS.txt](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v2.0.0/SHA256SUMS.txt)

---

### v1.1.4 · 2019-11-06

**主要变更**

- 支持查询顺序消息的消费轨迹。
- 优化消息拉取流程，避免特殊情况下拉取异常造成的消息堆积。
- 优化顺序消息重试间隔。
- 修复顺序消息重试时，重试次数不准确的问题。
- 修复某些条件下客户端生成 Message ID 重复的问题。

**资产**

| 平台 | 文件 | 大小 | SHA256 |
|---|---|---:|---|
| Windows (zip) | [aliyun-mq-csharp-sdk-1.1.4-windows.zip](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v1.1.4/aliyun-mq-csharp-sdk-1.1.4-windows.zip) | 52.3 MB | `c9c9c5c2…cc3dd` |
| Windows (rar) | [aliyun-mq-csharp-sdk-1.1.4-windows.rar](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v1.1.4/aliyun-mq-csharp-sdk-1.1.4-windows.rar) | 46.9 MB | `74a65f8e…0eb51` |

> zip 与 rar 包含相同的 SDK 内容，按需选用其一即可。

更多详情：[Release v1.1.4](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/tag/v1.1.4) · [SHA256SUMS.txt](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v1.1.4/SHA256SUMS.txt)

---

### v1.1.3 · 2019-02-01

**主要变更**

- 支持实例化用户使用以下两种方式接入（非实例化用户使用方式保持不变）：
  - 配置包含 InstanceId 的 NAMESRV_ADDR 方式接入使用。
  - 配置 InstanceId 和不包含 InstanceId 的 NAMESRV_ADDR 方式接入使用。
- ProducerId 和 ConsumerId 改为填写 Group ID 的值。

**资产**

| 平台 | 文件 | 大小 | SHA256 |
|---|---|---:|---|
| Windows | [aliyun-mq-csharp-sdk-1.1.3-windows.rar](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v1.1.3/aliyun-mq-csharp-sdk-1.1.3-windows.rar) | 46.9 MB | `ed60c66f…35f60c` |

更多详情：[Release v1.1.3](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/tag/v1.1.3) · [SHA256SUMS.txt](https://github.com/aliyunmq/mq-tcp-csharp-sdk/releases/download/v1.1.3/SHA256SUMS.txt)

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

SDK 接入与使用方式请参考[准备 TCP 协议的 .NET SDK 开发环境](https://help.aliyun.com/zh/apsaramq-for-rocketmq/cloud-message-queue-rocketmq-4-x-series/developer-reference/prepare-the-environment-2)。
