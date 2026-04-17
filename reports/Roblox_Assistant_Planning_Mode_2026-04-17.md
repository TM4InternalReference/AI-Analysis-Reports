# Roblox Assistant Planning Mode（2026-04-17）

> 📅 分析日期：2026-04-17
> 🔍 数据来源：Tavily 搜索（主力）、TechCrunch、Roblox 官方博客、开发者论坛等多源综合

---

## ⚡ 一句话速览

Roblox 于 2026 年 4 月为旗下 Roblox Studio 推出的 AI 助手重大升级，核心是 Planning Mode——将开发者的复杂游戏想法拆解为可编辑的执行计划，配合 Mesh 生成、Procedural Model 生成和自动化测试功能，形成 Plan-Build-Test 的 Agentic 开发闭环，帮助创作者从概念更快到可玩版本。

---

## 1. 产品概览

- **产品名称**：Roblox Assistant Planning Mode
- **所属厂商/公司**：Roblox Corporation（总部位于美国加州 San Mateo，NYSE 上市公司，股票代码 RBLX）
- **产品类型**：AI 游戏编辑器 / Agentic 开发工具
- **首次上线时间**：2026 年 4 月 16 日（正式发布）
- **最新版本/代次**：v1.0（首发版本，带 Planning Mode + Mesh Generation + Procedural Model Generation + Playtest Agent Beta）
- **官网地址**：https://create.roblox.com/docs/assistant/guide

---

## 2. 核心功能

- **Planning Mode（规划模式）**：将复杂提示词拆解为可编辑的任务列表 ⭐核心亮点
- **Mesh Generation（网格体生成）**：AI 生成带纹理的可直接使用的 3D 网格体 ⭐
- **Procedural Model Generation（程序化模型生成）**：通过文本/图片提示生成可编辑的 3D 模型，属性（书架层数、椅子数量等）可动态调整
- **Playtest Agent Beta（自动测试代理）**：AI 自动运行游戏、读取日志、捕获截图、模拟键盘鼠标输入、验证行为并自动反馈修复 ⭐
- **Agentic 闭环工作流**：Plan → Build → Test → Self-correct，形成自纠正系统
- **多 Agent 并行支持**（未来路线图）：多个 AI agent 协同工作
- **MCP 集成**：支持 Claude、Cursor、Codex 等第三方工具通过 MCP 协议接入 Roblox Studio

---

## 3. 技术能力评估

- **底层技术架构**：基于大语言模型的 Agentic 工作流系统，底层使用 Meta Llama 3 开源模型（在 Roblox Assistant 早期版本中确认）
- **模型基座**：早期版本使用 Meta Llama 3（开源模型）；Planning Mode 具体模型未公开披露
- **关键技术参数**：
  - 参数量：暂无公开数据
  - 上下文窗口：暂无公开数据
  - 多模态支持：支持文本提示、代码生成、3D 模型生成（Mesh + Procedural）、日志分析
  - 其他：内置 MCP Server，支持第三方工具集成
- **Benchmark 表现**：暂无公开的第三方 benchmark 数据
- **技术特色**：
  - **自纠正循环**（Self-correcting Loop）：Planning Mode 执行时调用 playtesting 工具，读取输出日志、捕获截图、模拟输入，发现 bug 并自动反馈给 Assistant 修复
  - **跨会话上下文保持**：规划上下文可跨 session 存储复用
  - **3D 空间理解**：Procedural Model 功能体现 AI 对 3D 空间和物理关系的理解
- **开源情况**：部分开源（Llama 3 作为底层模型基座），核心 Planning Mode 能力为闭源
- **API 能力**：通过 Studio 内置 MCP Server 向第三方工具开放部分 API（unprivileged APIs）

### 开发者生态（GitHub）

- **官方 GitHub 组织**：https://github.com/Roblox（存在但 Planning Mode 相关仓库未独立披露）
- **核心仓库**：暂无专门针对 Planning Mode 的公开 GitHub 仓库
- **官方 SDK 覆盖**：Roblox Studio（Lua）、MCP 协议集成
- **社区活跃度**：44% 的 top 1000 创作者已在使用 Roblox Assistant 或 MCP 工具（2026年3-4月数据）
- **第三方生态**：SuperbulletAI 等第三方 AI 工具已接入 Roblox；支持 Claude、Cursor、Codex 通过 MCP 接入

---

## 4. 版本迭代

| 版本 | 发布时间 | 主要变化 |
|------|---------|---------| 
| v1.0（Planning Mode） | 2026-04-16 | 首发：Planning Mode + Mesh Generation + Procedural Model（即将）+ Playtest Agent Beta |

**最新版本关键迭代亮点**：
- 从单步 prompt→输出升级为多步协作式开发伙伴
- 引入完整的 Plan-Build-Test Agentic 闭环
- 新增 3D 资产生成能力（Mesh + Procedural Model）
- AI 自动 QA 测试能力

---

## 5. 当前状态

- **可用状态**：✅ 已上线（Planning Mode + Mesh Generation 已上线；Procedural Model Generation 即将上线）
- **覆盖平台**：Roblox Studio（Desktop）
- **开放范围**：所有 Roblox Studio 创作者
- **访问限制**：需使用 Roblox Studio；部分功能（如 Playtest Agent）为 Beta 版本

---

## 6. 规模数据

- **用户规模**：
  - Roblox 整体 DAU：1.44 亿（2025年Q4，+69% YoY）
  - top 1000 创作者中使用 Assistant 或 MCP 工具的比例：44%（2026年3-4月数据）
- **收入规模**：
  - Roblox 2025年全年收入：约 49 亿美元（创纪录）
  - 2026年收入指引：至少 60 亿美元（预计 74.12 亿美元）
- **增长趋势**：用户规模同比增长 69%；收入持续增长；AI 工具采用率快速提升
- **市场地位**：Roblox 是全球最大 UGC 游戏平台，在 AI+游戏开发赛道处于领先地位

> ⚠️ Planning Mode 本身的独立用户/收入数据暂无公开披露

---

## 7. 商业模式

- **定价策略**：免费内置于 Roblox Studio；Roblox 主要通过 Robux 虚拟货币盈利
- **价格档位**：Roblox Assistant 功能全部免费使用
- **主要收入来源**：
  - Robux 虚拟货币销售（$0.01/Robux）
  - Roblox Plus 订阅（2026年4月30日上线，替代 Premium，10%-20% Robux 折扣）
  - 付费游戏收入分成（桌面端：50%/60%/70% 分成取决于游戏定价）
- **目标客户群**：Roblox 平台游戏开发者（从新手到 top 1000 专业创作者）

---

## 8. 投融资情况

- **公司最新估值**：未披露（上市公司，市值随股价波动）
- **累计融资额**：Roblox 已于 2021 年直接上市（DPO），无传统 VC 融资历史
- **融资历史**：Roblox 2021 年 3 月直接上市（NYSE: RBLX），此前融资历史不公开
- **上市状态**：已上市（NYSE: RBLX）

---

## 9. 竞品分析

- **所在赛道**：AI 游戏编辑器 / Agentic 游戏开发工具
- **主要竞品对比**：

| 维度 | Roblox Assistant | Unity AI | Unreal AI（CodeAssist等） | SuperbulletAI |
|------|---------|---------|---------|---------|
| 厂商 | Roblox | Unity | Epic Games | SuperbulletAI |
| 核心卖点 | Plan-Build-Test 全闭环 + 平台原生 | Unity 编辑器深度集成 | 虚幻引擎生态 + 蓝图可视化 | Roblox 专用 AI builder |
| 技术路线 | Llama 3 基座 + 自研 Agentic | Unity 主推 | Unreal Engine + AI | 第三方专用 |
| 定价 | 免费内置 | 部分免费 | 部分免费 | 1M free tokens/月 |
| 优势 | 平台原生、44% top 创作者已用、UGC 生态 | 引擎市场占用率 | 图形质量领先 | Roblox 专用优化 |
| 劣势 | 仅限 Roblox 平台 | AI 功能相对初级 | 上手门槛高 | 第三方依赖 |

- **竞争格局简述**：Roblox Assistant 是首个将完整 Agentic 闭环（Plan-Build-Test-Self-correct）深度集成到游戏引擎的 UGC 平台；传统引擎（Unity/Unreal）在 AI 编程助手方面相对初级，但具有更广泛的适用范围。
- **差异化定位**：深度嵌入 Roblox UGC 生态，降低创作者门槛，加速从想法到上线闭环

---

## 10. 总结与展望

- **核心优势**：
  1. 业界首个完整的 Agentic 游戏开发闭环（Plan-Build-Test-Self-correct），真正实现"AI 驱动的多步协作开发伙伴"
  2. 原生集成于全球最大 UGC 游戏平台（1.44 亿 DAU），44% top 创作者已使用，生态基础扎实
  3. 自纠正系统使 AI 随使用时间推移越来越准确，形成数据飞轮效应

- **潜在风险**：
  1. 目前仅支持 Roblox 平台，生态封闭性限制扩张
  2. Procedural Model Generation 功能尚未上线（"即将推出"），产品成熟度待验证
  3. AI 生成内容的版权归属、资产所有权等法律问题尚不明确

- **发展趋势**：
  1. 多 Agent 并行协同工作
  2. 云端长时复杂工作流
  3. 更智能的 NPC 行为模拟
  4. 与 Claude、Cursor、Codex 等主流 AI 工具的无缝集成
  5. AI workflow 可视化节点图

---

## 📎 参考信息（精选）

1. [Announcing Planning Mode for Roblox Assistant](https://devforum.roblox.com/t/announcing-planning-mode-for-roblox-assistant/4580715) — Roblox 官方开发者论坛 | 官方首发公告，完整功能说明
2. [Roblox's AI assistant gets new agentic tools to plan, build, and test games](https://techcrunch.com/2026/04/16/robloxs-ai-assistant-gets-new-agentic-tools-to-plan-build-and-test-games/) — TechCrunch | 权威科技媒体深度报道
3. [Roblox Studio is Going Agentic](https://about.roblox.com/newsroom/2026/04/roblox-studio-going-agentic) — Roblox 官方博客 | Nick Tornow（SVP Engineering）官方撰文
4. [Roblox AI assistant gets agentic tools to plan, build, and self-test games](https://thenextweb.com/news/roblox-ai-assistant-agentic-tools-planning-procedural-models) — The Next Web | 产品功能技术解析
5. [Roblox Q4业绩与用户增长双超预期](https://cloud.tencent.com/developer/news/3563310) — 腾讯云社区 | Roblox 业绩数据（DAU 1.44亿）
6. [4万字深度分析：2026年的全球UGC游戏](https://news.qq.com/rain/a/20260311A08DNR00) — 腾讯新闻 | Roblox 在 UGC 游戏赛道的竞争格局
7. [Roblox：百亿UGC 帝国的经济模型解析](https://www.tuoluo.cn/article/detail-10103499.html) — 陀螺科技 | Roblox 商业模式深度拆解
8. [SuperbulletAI AI Game Builder for Roblox](https://devforum.roblox.com/t/superbulletai-launched-the-most-powerful-ai-game-builder-for-roblox-and-its-free-for-everyone-to-try/3856417) — Roblox 开发者论坛 | 第三方 Roblox AI 工具生态
