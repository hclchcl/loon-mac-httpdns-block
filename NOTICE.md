# 署名、来源与许可

本仓库分别发行 **Mac HTTPDNS 拦截器**。适配者：hclchcl；适配及独立发行日期：2026-10-28。

原作者：VirgilClyne。原项目：[VirgilClyne/GetSomeFries](https://github.com/VirgilClyne/GetSomeFries)。依据 `sgmodule/HTTPDNS.Block.sgmodule` 的固定快照，原文随 `sources/HTTPDNS.Block.sgmodule` 提供。适用许可为 GNU GPL v3。

适配内容：移除 Surge 专属参数，改为 Loon 原生规则；IP 阻断收窄到端口 80/443/8080；选取明文 HTTP 复写、增加路径边界并去重；排除非法 IPv4 和不符合 URL 表示方式的 IPv6 路径条目；未纳入 Map Local 或 HTTPS MitM 配置。逐条记录见 [httpdns-changes.json](sources/httpdns-changes.json)。

上游的提交、文件 Git blob SHA、原始更新时间及链接见 [manifest.json](sources/manifest.json)。本次发行日期不代表每条上游规则均更新到该日期。

本项目参考可莉插件展示的功能方向，没有复制、解密或再分发可莉的 `.lpx` 文件，不是原作者的官方 Mac 移植。

插件以可编辑明文发行，按 [GPL-3.0](LICENSE) 许可。重新分发修改版时请保留适用署名、许可及修改说明。本仓库不适用原 DNS 项目的 MIT 许可。

Loon 语法依据：[插件](https://nsloon.app/docs/Plugin/)、[逻辑规则](https://nsloon.app/docs/Rule/logic_rule/)、[原生 Rewrite](https://nsloon.app/docs/Rewrite/rewrite_v2/)。

未进行实机效果测试，不提供覆盖全部应用的效果保证。
