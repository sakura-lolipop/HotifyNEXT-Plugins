# HotifyNEXT-Plugins

Hotify 的 **webhook 插件目录**——让任意服务的通知（memos 评论、Grafana 告警、Sonarr 下载完成…）推到手机。

插件是**纯数据 YAML**（无代码，写不出恶意行为），放进 Hotify 的 `hooks/` 目录即装。规则全文与写法见 [hooks.md](hooks.md)。

## 安装一个插件

最简：把 [hooks.md](hooks.md) 的 raw 链接 + 你想接的服务名发给任意 AI 助手，说"照这份规则写一个 Hotify 插件并告诉我怎么装"。

或者直接拿现成的（每个文件头自带逐步部署说明）：

| 插件 | 服务 | 事件 |
|---|---|---|
| [memos](plugins/memos.yaml) | Memos 笔记 | 评论通知 |
| [github-push](plugins/github.yaml) | GitHub | push 揨交 |
| [grafana](plugins/grafana.yaml) | Grafana | 告警触发/恢复 |
| [sonarr](plugins/sonarr.yaml) | Sonarr | 剧集入库 |
| [n8n](plugins/n8n.yaml) | n8n | 工作流任意步骤 |
| [uptime-kuma](plugins/uptime-kuma.yaml) | Uptime Kuma | 监控掉线/恢复 |
| [healthchecks](plugins/healthchecks.yaml) | Healthchecks | check 超时/恢复 |
| [immich](plugins/immich.yaml) | Immich | 照片入库 |
| [jellyfin](plugins/jellyfin.yaml) | Jellyfin | 媒体入库 |
| [echo](plugins/echo.yaml) | （教学样例） | 语法示范 |

服务器（Hotify）本体在 [HotifyNEXT-Server-Release](https://gitee.com/sakura-lolipop/HotifyNEXT-Server-Release)。

## 贡献插件

提 PR 到本仓 `plugins/`（一个插件一个 yaml 文件）——见 [CONTRIBUTING.md](CONTRIBUTING.md)，人工审核合并。

## 许可

MIT（贡献即按 MIT 授权，见 CONTRIBUTING）。
