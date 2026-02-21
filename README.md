本仓库规则只作为视频演示用途，考虑到兼容性，通用性，不能满足所有人的需求，请fork到自己仓库根据自己实际情况进行修改。

## 文件说明

### 根目录
- `direct.list`: 直连域名列表，包含不需要经过代理的域名。
- `proxy.list`: 代理域名列表，包含需要经过代理的域名。
- `fakeipfilter.json`: FakeIP 过滤配置，用于指定哪些域名不应解析为 FakeIP。

### 配置文件 (config/)

#### mihomo/ (Mihomo/Clash)
- `config.yaml`: Mihomo 基础配置文件。
- `configdns.yaml`: DNS 相关配置。
- `full.ini`, `mini.ini`: 不同精简程度的 INI 格式配置。
- `fuxie.yaml`: 覆写配置。
- `AI/`: 包含一些自动化处理脚本 (`transform.go`, `go_parser.py` 等) 和智能规则配置。

#### proxychain/
- `config.json`, `config.yaml`: ProxyChains 的配置文件。

#### singbox/
- `1.12.x/`: 适配 Sing-box 1.12.x 版本的配置。
  - `config.json`: 基础配置。
  - `sub-config.json`: 订阅转换相关的配置。
  - `iphone.json`: 针对 iPhone 设备的配置。
  - `momofake.json`, `fork-momofake.json`: 特定场景或修改版的配置。

#### zijian/
- `client/`: 客户端配置文件 (`config.json`, `config.yaml`)。
- `server/`: 服务端配置文件 (`config.json`)。  