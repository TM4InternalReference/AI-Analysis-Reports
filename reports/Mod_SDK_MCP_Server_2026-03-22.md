# Mod SDK MCP Server — AI 产品深度分析报告

> 📅 分析日期：2026-03-22
> 🔍 数据来源：Tavily 搜索（主力）、网易我的世界开发者官网、GitHub 等多源综合

---

## ⚡ 一句话速览

> Mod SDK MCP Server 是网易《我的世界》中国版推出的开源 MCP 服务器，为 AI 编程助手提供 Mod SDK 完整知识库，实现文档检索、代码生成、代码审查一站式 AI 辅助开发，降低 Mod 开发门槛。

---

## 1. 产品概览

- **产品名称**：Mod SDK MCP Server
- **所属厂商/公司**：MCNeteaseDevs（网易我的世界官方开发者团队）
- **产品类型**：AI 游戏开发者工具 / MCP Server
- **首次上线时间**：2026 年 3 月 18 日（开源发布）
- **最新版本/代次**：首发版本
- **官网地址**：https://github.com/MCNeteaseDevs/modsdk_mcp_server

## 2. 核心功能

- **智能文档检索**：模糊搜索、驼峰分词、中文搜索，覆盖全部 API 接口与事件文档 ⭐
- **一键代码生成**：自动生成符合中国版规范的 Mod 项目模板、Server/Client System、自定义物品/方块/实体代码 ⭐
- **工具与武器生成**：一键生成剑、镐、斧、锹、锄、弓、盔甲、食物、可投掷物品的完整 JSON 配置 ⭐
- **配方与战利品表**：生成有序/无序合成配方、熔炉配方、战利品表、生成规则，无需手写繁琐 JSON
- **代码审查**：自动检测 Python 2.7 兼容性问题、客户端/服务端混用错误、性能反模式
- **组件百科查询**：随时查询物品/方块/实体/中国版特有组件的用法和配置细节
- **内置最佳实践**：生成的所有代码自动遵循官方性能优化规范（CompFactory 缓存、Tick 降帧等）

## 3. 技术能力评估

- **底层技术架构**：基于 MCP（Model Context Protocol）协议，通过 stdio 或 SSE 传输模式与 AI 编程助手通信
- **模型基座**：支持 Claude Desktop、Cursor、CodeMaker 等所有兼容 MCP 协议的主流 AI 编程客户端
- **关键技术参数**：
  - Python >= 3.10
  - Context7 文档规模：58万+ tokens，3800+ 文档片段
  - 支持 SSE（Server-Sent Events）协议的任意 MCP 客户端
- **技术特色**：
  - 网易中国版 Mod SDK 专属适配，与国际版 MCP Server（如 modrinth MCP Server）形成差异化
  - 支持 Context7 零配置接入，文档实时同步官方仓库
  - 内置网易官方性能优化规范，开箱即用
- **开源情况**：完全开源（GitHub 开源）
- **API 能力**：作为 MCP Server 运行在本地端口 8080，通过标准 MCP 协议与 AI 助手交互

### 开发者生态（GitHub）

- **官方 GitHub 组织**：MCNeteaseDevs
- **核心仓库**：

| 仓库 | Stars | Forks | 最近更新 | 许可协议 | 说明 |
|------|-------|-------|---------|---------|------|
| modsdk_mcp_server | 暂无公开数据 | 暂无公开数据 | 2026-03-18 | 暂无数据 | 网易中国版 Mod SDK MCP Server |

- **第三方生态**：Context7 平台同步收录（零配置使用）

## 4. 版本迭代

| 版本 | 发布时间 | 主要变化 |
|------|---------|---------| 
| v1.0 | 2026-03-18 | 首发版本，正式开源上线 |

**最新版本关键迭代亮点**：首发版本，无前代对比

## 5. 当前状态

- **可用状态**：✅ 已开源，可直接部署使用
- **覆盖平台**：支持 Claude Desktop（推荐）、Cursor/VS Code、支持 SSE 协议的所有 MCP 客户端
- **开放范围**：完全开源，免费使用
- **访问限制**：无访问限制，需本地部署

## 6. 规模数据

- **用户规模**：暂无公开数据（新产品刚发布）
- **收入规模**：暂无公开数据（开源免费工具）
- **增长趋势**：依托网易《我的世界》中国版开发者社区，潜在用户基数大
- **市场地位**：网易中国版 Mod 开发 AI 辅助工具赛道的先行者

## 7. 商业模式

- **定价策略**：完全免费（开源）
- **价格档位**：无收费项目
- **主要收入来源**：非商业化产品，主要服务于网易《我的世界》开发者生态
- **目标客户群**：《我的世界》中国版 Mod 开发者

## 8. 竞品分析

- **所在赛道**：AI 游戏开发者工具（MCP Server for Game Modding）
- **主要竞品对比**：

| 维度 | Mod SDK MCP Server | MCoding MCP Server | modrinth MCP Server | mcmodding-mcp |
|------|---------|---------|---------|---------|
| 厂商 | 网易（MCNeteaseDevs） | 社区开发者 | Modrinth | 社区开发者 |
| 核心卖点 | 中国版 Mod SDK 专属适配 | 通用 Minecraft AI 控制 | Minecraft Mod 搜索索引 | Minecraft 源码深度访问 |
| 技术路线 | 知识库+代码生成+审查 | AI 控制游戏角色 | Mod 索引检索 | 源码映射+Mixin分析 |
| 适配版本 | 中国版（网易） | 国际版 | 国际版 | 国际版 |
| 定价 | 免费开源 | 免费开源 | 免费开源 | 免费开源 |
| 优势 | 官方支持、中文文档完整 | 可直接操控游戏 | 生态成熟 | 功能全面 |
| 劣势 | 仅限中国版 | 功能有限 | 非网易官方 | 非官方 |

- **竞争格局简述**：MCP 协议在 Minecraft 生态的应用处于早期，各家都是独立工具，互补性强于竞争性。网易官方推出的 Mod SDK MCP Server 优势在于对中国版 Mod SDK 的深度适配和官方支持。
- **差异化定位**：专注《我的世界》中国版 Mod SDK 的 AI 辅助开发，是目前唯一由中国游戏厂商官方推出的 MCP Server 产品

## 9. 技术架构亮点

- **MCP 协议标准**：遵循 Linux Foundation 旗下的 Model Context Protocol 开放协议
- **Context7 双轨支持**：
  - 自建 MCP Server：支持完整代码生成和审查功能
  - Context7 平台：零配置快速查文档，文档自动同步更新
- **网易官方最佳实践内置**：所有生成代码自动遵循官方性能优化规范，降低新手开发门槛
- **Python 2.7 兼容性处理**：自动检测不兼容写法（如 f-string、type hints）

## 10. 总结与展望

- **核心优势**：
  1. **官方背书**：网易《我的世界》官方团队开发，文档权威、持续维护有保障
  2. **降低开发门槛**：一键生成代码、内置最佳实践，让 Mod 开发更高效规范
  3. **MCP 生态整合**：同时支持自建 MCP Server 和 Context7 零配置接入，灵活选择

- **潜在风险**：
  1. **平台局限性**：仅支持《我的世界》中国版，国际版用户无法使用
  2. **生态依赖**：依附于网易 Mod SDK 版本更新，MCP Server 能力受限于 SDK 本身
  3. **社区活跃度**：刚开源，GitHub 社区和第三方插件生态尚待观察

- **发展趋势**：
  1. 短期：随着网易 Mod SDK 更新同步迭代，保持文档和工具最新
  2. 中期：可能接入更多 AI 客户端（如 Copilot、Windsurf 等）
  3. 长期：结合 Context7 扩展至 Apollo 等更多网易游戏开发者工具

---

## 📎 参考信息（精选）

1. [全新妙妙工具 Mod SDK MCP Server 来啦！- 我的世界开发者官网](https://mc.163.com/dev/developer_cn/news/renew/20260318/37047_1291751.html) — 网易官方 | 主要信息来源，详细功能介绍
2. [modsdk_mcp_server - GitHub](https://github.com/MCNeteaseDevs/modsdk_mcp_server) — GitHub | 官方开源仓库
3. [Context7 Mod SDK 文档](https://context7.com/mcneteasedevs/mc-netease-sdk) — Context7 | 零配置文档接入
4. [Model Context Protocol - GitHub](https://github.com/modelcontextprotocol) — Linux Foundation | MCP 协议规范
5. [Minecraft MCP Servers 生态概览](https://mcpservers.org/en/servers/ogmatrix/mcmodding-mcp) — MCP Servers | 竞品参考
