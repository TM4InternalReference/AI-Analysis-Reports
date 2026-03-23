# MoltStation（2026-03-23）

> 📅 分析日期：2026-03-23
> 🔍 数据来源：Tavily 搜索（主力）、官网深度阅读、官方文档分析等多源综合

---

## ⚡ 一句话速览

MoltStation 是一个实验性 AI Agent 游戏经济平台，让 AI 智能体自主运行游戏、竞争排名、赚取链上奖励并实现自给自足，率先提出"AI 智能体电竞"（Agentic Esports）概念。

---

## 1. 产品概览

- **产品名称**：MoltStation
- **所属厂商/公司**：MoltStation 团队（具体公司信息暂未公开）
- **产品类型**：AI Agent 游戏经济平台 / Agentic Esports 平台
- **首次上线时间**：2026 年 1 月（早期测试）
- **最新版本/代次**：v1.4.5（2026-03-12 更新）
- **官网地址**：https://www.moltstation.games

---

## 2. 核心功能

按功能模块分类列出，差异化亮点用 ⭐ 标注：

- **🤖 AI Agent 注册与身份管理**：连接 EVM 钱包铸造 Identity NFT，设置 Agent 个人资料元数据 ⭐
- **🎮 实时游戏会话（ShellRunners）**：AI Agent 自主参与街机障碍跑酷游戏，WebSocket 20Hz 实时帧同步 ⭐
- **🏆 排行榜系统**：实时性能排行榜，跟踪 Agent 的最高分和生涯表现 ⭐
- **💰 链上奖励系统**：基于得分的 $MOLTS 代币奖励派发，智能合约自动结算 ⭐
- **🖼️ NFT 成就系统**：ShellRunner NFT（高分自动铸造/升级）、PoPT NFT（首个成功提款铸造）⭐
- **🏪 NFT 市场**：买卖 Identity NFT、ShellRunner NFT、PoPT NFT
- **📡 直播观战**：实时观看 AI Agent 竞赛直播 ⭐
- **🗳️ 社区游戏投票**：Agent 参与未来游戏上线的社区投票治理

---

## 3. 技术能力评估

- **底层技术架构**：Web3 + AI Agent 混合架构，基于 Base（Ethereum L2）链构建游戏经济
- **模型基座**：AI Agent 框架无关（官方推荐 OpenClaw，可使用任意合规 Agent）
- **关键技术参数**：
  - 游戏帧率：20Hz WebSocket 实时同步
  - 链上交互：EVM 兼容（Base 链）
  - 钱包标准：EIP-712 签名认证
  - 代币标准：ERC-20（$MOLTS）、ERC-721（NFT）
- **技术特色**：
  - SIWE（Sign-In With Ethereum）钱包认证 ⭐
  - 智能合约自动奖励结算（Rewards.snapshotScoreSigned / payoutClaim）⭐
  - Agent 自主游戏循环（注册→游戏→快照→奖励→重复）⭐
  - 自改进策略参数系统（障碍风险权重、饥饿度收集权重等）⭐
- **开源情况**：部分开源（GitHub: MoltStation 组织，代码公开）
- **API 能力**：完整 REST API + WebSocket 游戏接口，官方提供多语言 Agent SDK 参考实现

### 开发者生态（GitHub）

- **官方 GitHub 组织**：https://github.com/MoltStation
- **核心仓库**：官方未公开具体仓库详情（组织页面未返回公开仓库数据）
- **官方 SDK 覆盖**：Node.js 18+（viem + ws 依赖）
- **社区活跃度**：项目处于早期发展阶段，社区数据暂无公开统计
- **第三方生态**：可与 OpenClaw 等主流 Agent 框架集成

---

## 4. 版本迭代

| 版本 | 发布时间 | 主要变化 |
|------|---------|---------| 
| v1.4.5 | 2026-03-12 | 最新版本，Agent 指令端点更新 |
| v1.0 | 2026-01 | 首发版本，ShellRunners 游戏上线 |

**最新版本关键迭代亮点**：
- 指令端点更新完善
- 路线图逐步推进

---

## 5. 当前状态

- **可用状态**：✅ 已上线（实验性运营阶段）
- **覆盖平台**：Web + API + WebSocket
- **开放范围**：全球可用（需 EVM 钱包）
- **访问限制**：需预装 AI Agent（推荐 OpenClaw）；游戏内消费需持有 ETH 用于 Gas

---

## 6. 规模数据

- **用户规模**：暂无公开数据（平台标注所有 Live Stats 均为"-"）
- **收入规模**：暂无公开数据
- **增长趋势**：暂无公开追踪数据
- **市场地位**：AI Agent 游戏赛道先驱者，暂无直接竞争对手

---

## 7. 商业模式

- **定价策略**：平台基础使用免费；NFT 铸造和市场交易产生 Gas 费用；游戏内奖励循环
- **价格档位**：

| 档位 | 价格 | 包含内容 |
|------|------|---------| 
| Agent 注册 | 免费 | Identity NFT 铸造资格 |
| ShellRunners 游戏 | 免费参与 | 赚取 $MOLTS 奖励机会 |
| NFT 市场交易 | 市场价格 | Identity/ShellRunner/PoPT NFT 自由交易 |

- **主要收入来源**：NFT 市场交易手续费、Gas 费分成（推测）
- **目标客户群**：AI Agent 开发者、Web3 玩家、加密原生用户

**代币经济学（$MOLTS）**：
- 平台玩家奖励：40%
- 团队财政部：10%
- Clanker LP 流通：50%
- 总奖励池：400 亿（400B）

---

## 8. 投融资情况

- **公司最新估值**：暂无公开数据
- **累计融资额**：暂无公开数据
- **融资历史**：暂无公开融资记录
- **上市状态**：未上市

---

## 9. 竞品分析

- **所在赛道**：AI Agent 游戏经济平台 / Agentic Esports
- **主要竞品对比**：

| 维度 | MoltStation | Synergetics.ai + ESCS | AI Agent Game 2025 大赛 |
|------|---------|---------|---------|
| 厂商 | MoltStation 团队 | Synergetics.ai / ESCS | Flowith AI 联合举办 |
| 核心卖点 | 实时 AI 游戏经济，自动化奖励循环 | AI Agent + 链上支付的电竞联盟 | 智能体创作大赛 |
| 技术路线 | Web3 + Base 链 + AI Agent | AI + Web3 电竞整合 | 比赛制，平台化运营 |
| 定价 | 免费参与 + Gas 消耗 | 赛事参与制 | 奖金激励 |
| 优势 | 先发优势，完整游戏循环，实时观战 | 战略联盟背书 | 社区流量，KOL 加持 |
| 劣势 | 无公开融资，平台数据不透明 | 非游戏平台 | 非持续运营平台 |

- **竞争格局简述**：MoltStation 是目前市场上**唯一**专注于 AI Agent 持续性游戏经济运行的平台，竞品多为赛事或活动形式。
- **差异化定位**：不仅做赛事，而是打造 AI Agent"打工赚钱-自给自足"的完整经济闭环

---

## 10. 总结与展望

- **核心优势**：
  1. **赛道先驱**：首个提出并落地"Agentic Esports"概念的平台
  2. **完整经济闭环**：注册→游戏→链上快照→奖励提取→循环，自动化程度高
  3. **开源友好**：Skill 文件完全公开，可与任意合规 Agent 集成

- **潜在风险**：
  1. **平台数据不透明**：无公开用户量、收入等核心指标，真实性难以验证
  2. **监管风险**：加密货币 + AI Agent 的结合可能面临各国监管政策变化
  3. **可持续性存疑**：平台活跃度数据（Agents Registered 等）均显示为 0，早期阶段依赖外部 Agent 生态导入

- **发展趋势**：
  1. 短期：持续迭代 ShellRunners + 社区投票上线新游戏
  2. 中期：引入更多游戏类型，扩大 $MOLTS 生态应用场景
  3. 长期：成为最大 AI Agent 游戏平台，主导 Agentic Esports 赛道标准

---

## 📎 参考信息（精选）

1. [MoltStation 官网](https://www.moltstation.games/) — 官方网站 | 平台完整信息，基础数据
2. [MoltStation 官方文档](https://docs.moltstation.games/) — 技术文档 | API 架构、智能合约设计
3. [MoltStation Skill 文件](https://www.moltstation.games/skills/moltstation/SKILL.md) — 完整 Agent 接入协议 | 核心实现细节
4. [Twitter @sukh_saroy 推文](https://x.com/sukh_saroy/status/2034682592491168119) — 产品介绍 | 创始愿景描述
5. [Twitter @moltstation](https://x.com/moltstation) — 官方社交 | 实时动态和公告
6. [Forbes: Moltbook AI Social Network](https://www.forbes.com/sites/guneyyildiz/2026/01/31/inside-moltbook-the-social-network-where-14-million-ai-agents-talk-and-humans-just-watch/) — Forbes 报道 | 行业背景参考
7. [Synergetics.ai + ESCS 战略合作](https://www.prnewswire.com/news-releases/synergeticsai-and-escs-announce-strategic-alliance-to-bring-ai-agents-and-on-chain-payments-to-the-global-e-sports-arena-302636568.html) — PR Newswire | 竞品动态

---

## MoltStation 速览

**一句话**：首个 AI Agent 游戏经济平台，让 AI 智能体自主玩游戏赚取链上奖励，打造"Agentic Esports"生态。

📌 **基本信息**
厂商：MoltStation 团队 | 类型：AI Agent 游戏经济平台 | 状态：✅ 已上线
上线时间：2026-01 | 最新版本：v1.4.5
官网：https://www.moltstation.games

🔧 **核心能力**
AI Agent 自主参与实时街机游戏、链上 $MOLTS 奖励派发、NFT 成就系统（ShellRunner/PoPT）、实时排行榜与观战、钱包签名认证（SIWE）

⚙️ **技术亮点**
基于 Base（Ethereum L2）链构建完整游戏经济，EIP-712 钱包认证，智能合约自动奖励结算，WebSocket 20Hz 实时帧同步，Agent 自改进游戏策略系统
Benchmark：暂无公开 Benchmark 数据

📊 **规模 & 商业**
用户规模：暂无公开数据（平台 Live Stats 均为 0）
收入：暂无公开数据
定价：免费参与，游戏消耗 Gas；NFT 市场自由定价
融资：暂无公开融资信息

⚔️ **竞品格局**
主要竞品：Synergetics.ai（AI + Web3 电竞联盟）、AI Agent Game 2025（智能体创作大赛）
核心优势：赛道先驱，唯一持续运营的 AI 游戏经济平台
主要风险：平台数据不透明，可持续性待验证

---
📅 2026-03-23 | 完整报告：{GitHub_URL}
