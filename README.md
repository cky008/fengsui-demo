# 烽燧 FengSui · 在线演示 / Live demo

**打开演示 / Open the demo → <https://demo.fengsui.iocky.com/>**

「烽燧」(FengSui / `cpe-dash`) 是华为 5G CPE Ultra 6（H168-383）的私有化射频监控与短信网关：3CA 载波聚合、邻区扫描、锁频锁站、设备访问控制、加密短信中心、Telegram 与 MCP 智能体接入。这里是它的 Web 控制台的在线演示。

- **数据全部是虚构的**：IMEI、号码、MAC、IP、基站信息都是 RFC / 保留号段里的占位值，短信和联系人也都是编的。
- **一切都在你的浏览器里**：页面里自带一个模拟后端，代替家里 NAS 上的守护进程。锁频、重启、断网、上网时段、收发短信都能点，但只在当前页面生效，刷新即复原，不会发出任何请求（除了加载页面本身）。
- **和真实版本一致**：初始数据是构建时由真守护进程录制的；页面内的后端与守护进程共用同一套入参校验、锁频与访问控制规划、短信会话逻辑，并由契约测试逐项比对。

这个仓库只存放演示的构建产物（`gh-pages` 分支），由主项目每次发布时自动更新，请不要直接修改该分支。

---

FengSui (`cpe-dash`) is a self-hosted RF monitor and SMS gateway for the Huawei 5G CPE Ultra 6 (H168-383). This is a live demo of its web console.

- **Every value is fictional**: identifiers are RFC / reserved placeholders, and the messages and contacts are made up.
- **Everything runs in your browser**: an in-page backend stands in for the daemon. Locks, reboots, blocking devices, internet time windows and SMS all work, inside that page only, and reset on reload.
- **Faithful to the real thing**: the starting data is recorded from the real daemon at build time, and the in-page backend shares the daemon's validation, planning and SMS code, checked call by call by a contract test.

This repository only holds the demo's build output (the `gh-pages` branch), published automatically by the main project's release workflow. Please don't edit that branch by hand.
