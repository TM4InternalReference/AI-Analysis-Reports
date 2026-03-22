# General Intuition — AI 产品深度分析报告

> 📅 分析日期：2026-03-22
> 🔍 数据来源：Tavily 搜索（主力）、TechCrunch 文章深度阅读等多源综合

---

## ⚡ 一句话速览

> General Intuition 是从游戏视频分享平台 Medal 分拆出来的 AI 前沿研究实验室，通过海量游戏视频数据训练具备时空推理能力的世界模型和 AI Agent，目标是实现真正通向 AGI 所需的物理世界理解能力。

---

## 1. 产品概览

- **产品名称**：General Intuition（公司名，也指其核心产品线）
- **所属厂商/公司**：General Intuition Inc.，由 Pim de Witte（同时担任 Medal CEO）创立，总部位于美国
- **产品类型**：AI Agent 平台 + 世界模型（World Model）
- **首次上线时间**：2025 年 10 月正式公开（种子轮同步曝光）
- **最新版本/代次**：首发版本，暂无迭代版本记录
- **官网地址**：https://www.generalintuition.com/

## 2. 核心功能

- **时空推理模型（Spatial-Temporal Reasoning）**：通过视频游戏片段学习物体和实体如何在空间中移动和随时间变化，这是传统 LLMs 缺乏的核心能力 ⭐
- **世界模型（World Model）**：在压缩的现实模拟环境中让 Agent 先"做梦"测试各种可能性，低成本推导假设以加速现实世界学习 ⭐
- **AI Agent 训练**：基于纯视觉输入的 Agent，仅看到人类玩家所见画面，通过控制器输入在空间中移动
- **游戏 Bot 与 NPC 生成**：可扩展至任意难度等级的 AI 对手，区别于传统"确定性 Bot"（每次产生相同输出的预编程角色）
- **搜索救援无人机**：在无 GPS 环境中自主导航的无人机应用

## 3. 技术能力评估

- **底层技术架构**：基于视频游戏数据训练的世界模型 + 视觉驱动 Agent，模型通过观察玩家视角（第一人称摄像头视角）学习环境理解
- **模型基座**：自研foundation model，基于 Medal 平台的 2B+ 年度游戏视频数据
- **关键技术参数**：
  - 训练数据规模：每年 20 亿个游戏视频（来自 Medal 平台 1000 万 MAU）
  - 数据优势：游戏玩家倾向于上传极端正面或负面案例，形成精确有用的边缘案例训练数据（"选择偏见"反而成为优势）
  - 隐私保护：采用隐私优先的 Action Labels 数据处理方式
- **Benchmark 表现**：暂无公开 Benchmark 数据
- **技术特色**：
  - 纯视觉输入 + Controller 输入驱动，模拟人类玩家操作方式
  - 可在没有 GPS 的陌生物理环境中导航
  - 能理解未曾训练过的环境并正确预测其中的行为
  - 技术路径可直接迁移至机械臂、无人机、自动驾驶汽车等物理系统（这些设备通常也用游戏手柄操控）
- **开源情况**：完全闭源
- **API 能力**：暂无公开 API 信息

### 开发者生态（GitHub）

- **官方 GitHub 组织**：暂无公开 GitHub 组织信息
- **核心仓库**：无公开仓库

## 4. 版本迭代

| 版本 | 发布时间 | 主要变化 |
|------|---------|---------| 
| v1.0 | 2025年10月 | 首发版本，正式公开同时宣布 $134M 种子轮 |

**最新版本关键迭代亮点**：首发版本，无前代对比

## 5. 当前状态

- **可用状态**：🔒 早期研发阶段，尚未商业化产品
- **覆盖平台**：暂未公布具体平台计划
- **开放范围**：仅限有限合作伙伴预览
- **访问限制**：严格受限

## 6. 规模数据

- **用户规模**：暂未公开具体 Agent 用户规模（Medal 平台：1000 万 MAU）
- **收入规模**：暂无公开数据（公司处于纯研发投入阶段）
- **增长趋势**：公司刚刚完成分拆并获得大额融资，团队快速扩张中
- **市场地位**：世界模型 + 空间推理赛道的新进入者，差异化明显

## 7. 商业模式

- **定价策略**：尚在规划中，未公开
- **价格档位**：暂无信息
- **主要收入来源**：
  - 游戏 Bot/NPC 授权（替代传统确定性机器人）
  - 搜索救援无人机软件
  - 未来可能扩展至机器人、自动驾驶等领域
- **目标客户群**：游戏开发商、无人机运营商、机器人企业

## 8. 投融资情况

- **公司最新估值**：暂无公开估值（种子轮通常不公布估值）
- **累计融资额**：$1.337 亿美元（种子轮）
- **融资历史**：

| 轮次 | 时间 | 金额 | 主要投资方 |
|------|------|------|----------|
| Seed | 2025年10月 | $1.337亿 | Khosla Ventures、General Catalyst、Raine |

- **上市状态**：未上市

**附注**：据 The Information 报道，OpenAI 曾于 2024 年底尝试以 $5 亿美元收购 Medal（General Intuition 母公司），但被拒绝。

## 9. 竞品分析

- **所在赛道**：AI 世界模型（World Model）+ AI Agent（空间推理方向）
- **主要竞品对比**：

| 维度 | General Intuition | DeepMind Genie 3 | World Labs Marble | Sora (OpenAI) |
|------|---------|---------|---------|---------|
| 厂商 | General Intuition | Google DeepMind | World Labs (Fei-Fei Li) | OpenAI |
| 核心卖点 | 游戏视频驱动的时空推理 Agent | 实时交互式3D世界生成 | 单图生成静态3D世界 | 视频生成 |
| 技术路线 | 视觉+动作标签驱动 | 实时生成+24fps交互 | 上游计算生成精细3D | Diffusion Transformer |
| 定价 | 未商业化 | 部分开放 | 部分开放 | 付费API |
| 优势 | 独特游戏数据护城河，20亿+/年视频 | Google算力支持 | 学术权威背景 | 先发优势和品牌 |
| 劣势 | 刚起步，生态不成熟 | 非专注Agent应用 | 非专注Agent应用 | 缺乏物理世界理解 |

- **竞争格局简述**：世界模型赛道目前主要有三类玩家——科技巨头（DeepMind、Google）、明星创业公司（World Labs）和垂直领域专家（General Intuition）。General Intuition 差异化在于专注"空间推理"这一 LLMs 天然缺乏的能力，且拥有独特的游戏视频数据护城河。
- **差异化定位**：不与世界模型厂商直接竞争销售模型，而是将世界模型作为训练 Agent 的底层基础设施，应用聚焦游戏和救援无人机

## 10. 总结与展望

- **核心优势**：
  1. **数据护城河**：Medal 平台每年 20 亿个游戏视频，覆盖数万款游戏，20亿+/年的数据积累难以复制
  2. **独特技术路径**：专注空间-时间推理，这是迈向 AGI 不可或缺但当前 LLMs 缺乏的能力
  3. **应用落地明确**：游戏 Bot 和救援无人机有清晰商业化路径，避免与巨头直接竞争模型销售

- **潜在风险**：
  1. **技术商业化难度**：世界模型训练成本高昂，商业化路径需要时间验证
  2. **人才竞争**：作为刚完成融资的创业公司，与巨头争夺顶尖 AI 人才挑战巨大
  3. **监管风险**：AI Agent 在无人机等实体领域的应用可能面临严格监管

- **发展趋势**：
  1. 短期内专注游戏 Bot 和 NPC 场景，验证技术可行性
  2. 中期扩展至搜索救援无人机和其他实体世界 Agent
  3. 长期目标是成为 AGI 进程中"空间推理"能力的核心提供商

---

## 📎 参考信息（精选）

1. [General Intuition lands $134M seed to teach agents spatial reasoning using video game clips](https://techcrunch.com/2025/10/16/general-intuition-lands-134m-seed-to-teach-agents-spatial-reasoning-using-video-game-clips/) — TechCrunch | 主要信息来源，详细报道融资和技术方向
2. [General Intuition Raises $134 Million Seed to Advance AI Agents with Spatial Reasoning](https://mlq.ai/news/general-intuition-raises-134-million-seed-to-advance-ai-agents-with-spatial-reasoning/) — MLQ.ai | 融资详情补充
3. [General Intuition | The frontier research lab dedicated to games](https://www.generalintuition.com/) — 官方网站 | 公司官方信息
4. [World Models & General Intuition: Khosla's largest bet since LLMs & OpenAI](https://www.latent.space/p/world-models-and-general-intuition) — Latent Space | 深度技术访谈，Pim de Witte 详解技术路径
5. [Genie 3: A new frontier for world models](https://deepmind.google/blog/genie-3-a-new-frontier-for-world-models/) — Google DeepMind | 竞品 Genie 3 技术详解
6. [A new world model startup is quietly raising big money](https://sources.news/p/a-new-world-model-startup-is-quietly) — Sources News | General Intuition 早期报道
