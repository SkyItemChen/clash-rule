# 简介
本项目生成适用于 Clash Premium 内核的规则集（RULE-SET），同时适用于所有使用 Clash Premium 内核的 Clash 图形用户界面（GUI）客户端。

## 说明
本项目根据[@Loyalsoldier/clash-rules](https://github.com/Loyalsoldier/clash-rules) 进行补充规则集，供个人使用

本项目的规则集（RULE-SET）只适用于 Clash **Premium** 版本。Clash Premium 相对于普通版，增加了 **TUN 增强模式**，能接管设备所有 TCP 和 UDP 流量。

更多说明请访问[@Loyalsoldier/clash-rules](https://github.com/Loyalsoldier/clash-rules)

## 补充原因
因为需要制作一个满足代理白名单模式的规则，发现上述项目规则少了自己用到的链接，又因为不想后续编辑更多规则而麻烦，因此有了这个项目，直接下载导入方便多了

### 在线地址（URL）

> 如果无法访问域名 `raw.githubusercontent.com`，可以使用第二个地址（`cdn.jsdelivr.net`），但是内容更新会有 12 小时的延迟。以下地址填写在 Clash 配置文件里的 `rule-providers` 里的 `url` 配置项中。

- **代理域名列表 proxy.txt**：
  - [https://raw.githubusercontent.com/SkyItemChen/clash-rule/refs/heads/releases/proxy.txt](https://raw.githubusercontent.com/SkyItemChen/clash-rule/refs/heads/releases/proxy.txt)
  - [https://cdn.jsdelivr.net/gh/SkyItemChen/clash-rule@releases/proxy.txt](https://cdn.jsdelivr.net/gh/SkyItemChen/clash-rule@releases/proxy.txt)

### 使用方式

要想使用本项目的规则集，参考[@Loyalsoldier/clash-rules](https://github.com/Loyalsoldier/clash-rules)

如果Clash无法从网络获取该规则集，可以选择本地文件加载规则集
```yaml
rule-providers:
  proxy:
      type: file
      behavior: domain
      path: ./ruleset/proxy.txt
```

## 致谢

- [@Loyalsoldier/clash-rules](https://github.com/Loyalsoldier/clash-rules)
