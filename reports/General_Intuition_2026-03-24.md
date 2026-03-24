# General Intuition（2026-03-24）

> 📅 分析日期：2026-03-24
> 🔍 数据来源：Tavily 搜索（主力）、TechCrunch、官网等多源综合

---

## ⚡ 一句话速览

> General Intuition 是由 Medal 孵化的 AI 前沿研究实验室，专注于时空推理（spatial-temporal reasoning）世界模型，2025年10月获 $1.337 亿美元种子轮融资（Khosla Ventures 领投），是当年最大 AI 种子轮之一，号称要教机器"通过玩耍学习"实现通用人工智能。

---

## 1. 产品概览

- **产品名称**：General Intuition
- **所属厂商/公司**：General Intuition PBC（公益公司），由 Medal 孵化分拆，创始人 Pim de Witte（Medal CEO）兼任
- **产品类型**：AI 前沿研究实验室（世界模型 / AI Agent）
- **首次上线时间**：2025年（正式公开）
- **最新版本/代次**：早期研究阶段，尚未有商业化产品
- **官网地址**：https://www.generalintuition.com

## 2. 核心研究方向

- **时空推理 Agent** ⭐：能理解并预测 3D 环境中物体和实体的移动模式
- **世界模型**（World Models）⭐：在压缩的现实模拟中"做梦"，低成本测试各种可能性
- **视频理解**：聚焦向现实世界迁移的能力
- **游戏 Agent 应用**：超越传统确定性 Bot 的自适应 AI 对手

## 3. 技术能力评估

- **核心技术路线**：通过视频游戏数据训练 AI 的时空推理能力
- **数据优势**：基于 Medal 的数据集——每年 20 亿条视频，来自 1000 万月活用户、数万款游戏 ⭐
- **训练方法**：
  - Agent 仅通过视觉输入学习（看到人类玩家所见的画面）
  - 通过追踪控制器输入来学习空间移动
  - 游戏视频数据天然筛选了极端案例（极高/极低情绪），适合训练
- **技术特色**：
  - 可理解和预测从未训练过的环境
  - 模型能泛化到物理系统（机械臂、无人机、自动驾驶汽车）
  - 作为公益公司（PBC），承诺不开发替代设计师/艺术家/创作者的技术
- **研究背景**：团队成员有 DIAMOND（2024 NeurIPS Spotlight）、Δ-IRIS（ICML 2024）、IRIS（ICLR Oral 2023）等顶级论文

### 开发者生态

- **GitHub**：暂无公开代码库（前沿研究阶段）
- **研究论文**：GAIA-2、DIAMOND、Δ-IRIS、IRIS 等多篇顶会论文

## 4. 版本迭代

| 版本 | 发布时间 | 主要进展 |
|------|---------|---------| 
| 公司成立 | 2025年10月 | 正式公开，获 $133.7M 种子轮 |
| GAIA-2 发布 | 2025年 | 视频生成模型前沿研究 |
| DIAMOND 发布 | 2024年NeurIPS | Diffusion 世界建模 |

**最新技术进展**：
- 模型能理解从未训练过的环境并正确预测其中的动作
- 正在攻克：在完全陌生的物理环境中自主导航

## 5. 当前状态

- **可用状态**：🔒 早期研究阶段，尚未商业化
- **覆盖平台**：研究/技术原型阶段
- **开放范围**：暂未开放 API 或产品
- **访问限制**：仅接受简历投递（官网招聘页面）

## 6. 规模数据

- **团队规模**：约 12 人核心团队（官网列示）
- **融资规模**：$1.337 亿美元种子轮（2025年10月）
- **市场地位**：时空推理+世界模型赛道最大种子轮之一

## 7. 商业模式

- **当前阶段**：非商业化研究阶段
- **潜在商业路径**：
  - 游戏 Bot/NPC 销售（可缩放难度、填充游戏人数）
  - 搜救无人机 AI
  - 机器人/自动驾驶训练
- **差异化承诺**：不销售世界模型（避免版权问题），聚焦 Agent 应用

## 8. 投融资情况

- **公司最新估值**：未披露（种子轮 $133.7M）
- **累计融资额**：$1.337 亿（种子轮）
- **融资历史**：

| 轮次 | 时间 | 金额 | 主要投资方 |
|------|------|------|----------|
| 种子轮 | 2025年10月 | $1.337 亿 | Khosla Ventures（领投）、General Catalyst、Raine |

- **Khosla 评价**：认为是自 2018 年投资 OpenAI 以来最大的赌注
- **上市状态**：未上市

## 9. 竞品分析

- **所在赛道**：AI 世界模型 × 时空推理 Agent
- **主要竞品对比**：

| 维度 | General Intuition | Google DeepMind Genie | World Labs Marble | Wayve GAIA-2 |
|------|------------------|----------------------|------------------|--------------|
| 厂商 | General Intuition | Google DeepMind | World Labs（李飞飞） | Wayve |
| 核心卖点 | 时空推理+游戏数据 | 3D 世界生成 | 3D 理解 | 视频+世界模型 |
| 训练数据 | Medal 游戏视频 | 多源 | 多源 | 自研 |
| 商业化 | Agent 优先 | 对外销售 | 对外销售 | 自研 |
| 开源 | 暂无 | 暂无 | 暂无 | 论文开源 |
| 优势 | 数据壁垒、PBC定位 | 谷歌资源 | 李飞飞团队 | 专注视频 |
| 劣势 | 早期、规模小 | 方向差异 | 同样早期 | 非直接竞争 |

- **竞争格局简述**：世界模型赛道目前处于早期探索期，DeepMind Genie 和 World Labs Marble 均选择对外销售世界模型，而 General Intuition 刻意回避这一路径以规避版权风险，聚焦 Agent 应用。Khosla 认为这是"继 2018 年投资 OpenAI 以来最大的赌注"。
- **差异化定位**：通过游戏视频学习时空推理，以"玩"为核心打造通用人工智能，不与游戏开发者竞争。

## 10. 总结与展望

- **核心优势**：
  1. Medal 独有的 20 亿条/年游戏视频数据壁垒，连 OpenAI 都曾试图收购
  2. 团队有 DIAMOND、IRIS 等世界模型顶会论文背书，研究实力强
  3. Khosla Ventures + General Catalyst 顶级 VC 加持，资金充足
- **潜在风险**：
  1. 纯研究阶段，商业化路径和时间线不明确
  2. 世界模型竞争激烈，DeepMind、World Labs 资源更雄厚
  3. 时空推理是 AGI 的核心难题之一，技术突破难度极高
- **发展趋势**：
  1. 首个商业化产品可能是游戏自适应 Bot（可动态调整难度）
  2. 搜救无人机可能是第二个落地场景（创始人有人道主义背景）
  3. 若技术成熟，可能成为机器人/自动驾驶训练数据的重要来源

---

## 📎 参考信息（精选）

> 以下为本次分析中最有价值的信息源，按价值排序

1. [TechCrunch: General Intuition lands $134M seed](https://techcrunch.com/2025/10/16/general-intuition-lands-134m-seed-to-teach-agents-spatial-reasoning-using-video-game-clips/) — TechCrunch | 核心报道，$134M 融资详情
2. [General Intuition 官网](https://www.generalintuition.com/) — 官网 | 公司定位和研究方向
3. [Silicon Angle: Spatial-temporal reasoning startup closes $133.7M](https://siliconangle.com/2025/10/16/spatial-temporal-reasoning-startup-general-intuition-closes-133-7m-investment/) — Silicon Angle | 投资方信息
4. [The AI Insider: General Intuition Launches with $133.7M Seed Round](https://theaiinsider.tech/2025/11/03/general-intuition-launches-with-133-7m-seed-round-to-build-ai-agents-with-spatial-temporal-reasoning/) — The AI Insider | 融资详情
5. [Sources: A new bet on what comes after LLMs](https://sources.news/p/a-new-bet-on-what-comes-after-llms) — Sources | Khosla 访谈，对标 OpenAI 的投资逻辑
6. [LinkedIn: Pim de Witte 宣布 General Intuition](https://www.linkedin.com/posts/pimdw_introducing-general-intuition-and-our-1337m-activity-7384596582052155392-b4Fl) — LinkedIn | 创始人官方宣布
