# Game Creator（2026-04-07）

> 📅 分析日期：2026-04-07
> 🔍 数据来源：GitHub仓库分析、Tavily搜索、官网等多源综合

---

## ⚡ 一句话速览

> OpusGameLabs出品的AI Agent游戏工作室开源项目，通过命令让AI agent完成从脚手架→设计→音频→部署→变现的完整游戏开发流水线，支持40+ AI编程代理，MIT开源。

---

## 1. 产品概览

- **产品名称**：Game Creator
- **所属厂商/公司**：OpusGameLabs
- **产品类型**：AI游戏编辑器 / AI Agent平台
- **首次上线时间**：2025年（GitHub显示2026年2月有活跃更新）
- **最新版本/代次**：持续活跃更新中（163次commits）
- **官网地址**：https://opusgamelabs.github.io/game-creator/
- **GitHub**：https://github.com/OpusGameLabs/game-creator

## 2. 核心功能

按功能模块分类，差异化亮点用 ⭐ 标注：

- **make-game完整流水线**：一句话让AI从零构建可玩的2D/3D浏览器游戏（scaffold→像素画→设计→音频→部署→变现），共5步自动化 ⭐
- **多引擎支持**：Phaser 3（2D侧滑跑酷/平台跳跃/街机）和Three.js（3D环境）双引擎 ⭐
- **内置QA自动化**：每个代码修改步骤后自动运行Playwright测试（构建检查、运行时检查、游戏玩法验证、架构验证、视觉回归），失败自动修复重跑（最多3次） ⭐
- **程序化音频**：Strudel.cc生成Chiptune BGM和复古SFX，无需音频文件 ⭐
- **一键部署**：GitHub Pages、Vercel、Netlify、itch.io等静态托管
- **Play.fun变现**：内置OpenGameProtocol SDK，支持点数/排行榜/钱包连接 ⭐
- **8个Slash命令**：/make-game、/improve-game、/design-game、/add-feature、/add-assets、/add-audio、/monetize-game、/qa-game
- **4个自主Agent**：game-creator（端到端流水线）、game-reviewer（代码审查）、game-qa-runner（自动化测试）、game-deploy（部署自动化）
- **8个参考技能**：phaser、threejs-game、game-assets、game-designer、game-audio、game-qa、game-architecture、game-deploy、playdotfun

## 3. 技术能力评估

- **底层技术架构**：
  - 2D引擎：Phaser 3（^3.90.0）
  - 3D引擎：Three.js（^0.183.0）
  - 音频：Strudel.cc（@strudel/web ^1.3.0，AGPL-3.0许可）
  - 构建：Vite（^7.3.1）
  - 测试：Playwright（^1.58.0）+ axe-core（^4.11.0）
- **模型基座**：不绑定特定LLM，支持40+ AI编程代理（Claude Code、Cursor、Windsurf、Cline等）
- **关键技术参数**：
  - AI Agent支持：40+编程代理
  - 自动化QA：每步5层检查
  - 部署方式：静态托管（GitHub Pages/Vercel/Netlify/itch.io）
- **技术特色**：
  - EventBus发布订阅架构：模块解耦
  - GameState集中状态管理：reset()干净重启
  - 零魔法数字：所有配置在Constants.js
  - render_game_to_text()：AI可读取游戏状态而无需解析像素
- **Benchmark表现**：暂无公开Benchmark
- **开源情况**：MIT许可（使用@strudel/web需AGPL-3.0兼容）
- **API能力**：通过slash命令调用，不提供程序化API

### 开发者生态（GitHub）

- **官方 GitHub 组织**：OpusGameLabs
- **核心仓库**：

| 仓库 | Stars | Forks | 最近更新 | 许可协议 | 说明 |
|------|-------|-------|---------|---------|------|
| game-creator | 94 | 15 | 2026-03-23 | MIT | AI游戏工作室，支持40+代理，163次commits |

- **官方 SDK 覆盖**：通过npx skills add安装，Claude/VS Code Cursor/Windsurf等插件生态
- **社区活跃度**：活跃更新中，163次commits，15个forks
- **第三方生态**：支持集成到40+ AI编程代理的生态系统中

## 4. 版本迭代

| 版本 | 发布时间 | 主要变化 |
|------|---------|---------| 
| 初始版本 | ~2025年 | 基础AI游戏生成框架 |
| 持续更新 | 2026年 | 自动化QA、Play.fun变现、多Agent协作 |

**最新版本关键迭代亮点**：
- 完善的自动化QA子代理体系
- Play.fun内置变现支持
- 多代理分工协作（creator/reviewer/qa-runner/deploy）

## 5. 当前状态

- **可用状态**：✅ 开源可用（MIT许可）
- **覆盖平台**：Web浏览器（生成的游戏可部署至任意静态托管）
- **开放范围**：全球开源，npx skills add即可安装
- **访问限制**：需支持npx的Node.js环境

## 6. 规模数据

- **用户规模**：暂无公开用户数
- **收入规模**：暂无公开数据
- **增长趋势**：GitHub stars持续增长，社区活跃
- **市场地位**：AI游戏开发工具赛道的创新者，专注于AI Agent工作流编排

> ⚠️ 规模数据暂无公开披露

## 7. 商业模式

- **定价策略**：免费开源 + 可选Play.fun变现
- **价格档位**：

| 档位 | 价格 | 包含内容 |
|------|------|---------| 
| 开源基础版 | 免费 | make-game流水线、基础QA、多引擎支持 |
| Play.fun变现 | 免费接入 | SDK集成、点数/排行榜/钱包功能 |

- **主要收入来源**：不直接变现，通过Play.fun生态间接盈利
- **目标客户群**：AI编程代理用户、独立游戏开发者、内容创作者

## 8. 投融资情况

- **公司最新估值**：暂无公开数据
- **累计融资额**：暂无公开数据
- **融资历史**：未披露
- **上市状态**：未上市

## 9. 竞品分析

- **所在赛道**：AI游戏开发工具 / AI Agent开发平台
- **主要竞品对比**：

| 维度 | Game Creator | Rosebud AI | Upit | Lobehub |
|------|-------------|------------|------|---------|
| 厂商 | OpusGameLabs | Rosebud AI | Upit | Lobehub |
| 核心卖点 | Agent流水线+自动化QA | AI游戏创建 | AI游戏构建 | AI技能市场 |
| 自动化程度 | 高（多Agent协作） | 中 | 中 | 低 |
| 变现支持 | Play.fun内置 | 有 | 有 | 无 |
| 开源 | MIT开源 | 闭源/部分开源 | 闭源 | 闭源 |

- **竞争格局简述**：
  - AI游戏生成赛道已有多个产品，但Game Creator的差异化在于完整的Agent工作流+内置QA
  - 专注AI Agent生态（而非直接面向用户）是一个独特的切入角度
- **差异化定位**：面向AI Agent的游戏工厂，而非面向用户的游戏生成器

## 10. 总结与展望

- **核心优势**：
  1. **工作流完整**：从想法到部署变现的端到端自动化，大幅降低游戏开发门槛
  2. **QA内置**：每个步骤都有Playwright自动化测试，确保生成质量
  3. **多代理协作**：4个专业化Agent分工，架构清晰可扩展
- **潜在风险**：
  1. 闭源生态依赖（OpenClaw等框架）
  2. 面向开发者而非终端用户，市场教育需要时间
  3. 3D游戏生成质量依赖底层AI能力天花板
- **发展趋势**：
  1. 持续完善自动化QA和修复机制
  2. 扩大支持的AI代理范围
  3. 深化Play.fun等变现平台集成

---

## 📎 参考信息（精选）

1. [Game Creator GitHub仓库](https://github.com/OpusGameLabs/game-creator) — GitHub | 完整的架构文档和技术细节
2. [Game Creator官网](https://opusgamelabs.github.io/game-creator/) — OpusGameLabs | 产品首页和功能介绍
3. [Game Creator — Lobehub](https://lobehub.com/skills/opusgamelabs-game-creator-make-game) — Lobehub | 技能集成说明
