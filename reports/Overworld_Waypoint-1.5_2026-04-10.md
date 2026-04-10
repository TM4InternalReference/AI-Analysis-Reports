# Overworld Waypoint-1.5（2026-04-10）

> 📅 分析日期：2026-04-10
> 🔍 数据来源：HuggingFace Blog、GamesBeat、FinancialContent 等多源综合

---

## ⚡ 一句话速览

> Overworld Waypoint-1.5 是全球首个消费级 GPU 实时运行的 AI 世界模型，720p/60fps 高保真输出，训练数据量提升 100 倍，本地优先架构保护隐私，云端串流降低门槛。

---

## 1. 产品概览

- **产品名称**：Waypoint-1.5（Overworld 公司）
- **所属厂商/公司**：Overworld（前身 Wayfarer Labs），美国罗德岛州普罗维登斯
- **产品类型**：实时 AI 世界模型 / 生成式 3D 交互引擎
- **首次上线时间**：Waypoint-1 于 2026 年 1 月发布；Waypoint-1.5 于 **2026 年 4 月 9 日**发布
- **最新版本/代次**：Waypoint-1.5（双档位：720p + 360p）
- **官网地址**：https://over.world/ | https://www.overworld.stream/

## 2. 核心功能

- **720p/60fps 高保真实时生成**⭐：在 RTX 3090~5090 等消费级 GPU 上实时运行
- **双档位硬件适配**：720p 档（高端 PC）+ 360p 档（游戏本、MacBook、Apple Silicon）
- **本地 Biome Runtime**⭐：简化安装流程，下载后几分钟即可本地运行，保护隐私
- **云端 Overworld.stream**：浏览器直接访问，无需本地配置
- **World Engine**：灵活易用的核心推理库，官方+第三方客户端支持

## 3. 技术能力评估

- **底层技术架构**：Diffusion Transformer（Rectified Flow Transformer）
- **模型基座**：自研 Diffusion 世界模型，训练数据来自 10,000 小时游戏视频 + 控制信号配对
- **关键技术参数**：
  - Waypoint-1.5-1B（720p）：RTX 3090~5090 支持 720p/60fps
  - Waypoint-1.5-1B-360P：游戏本、Mac（即将支持）
  - 训练数据量：Waypoint-1.5 是 Waypoint-1 的 **~100 倍**
  - 视频建模技术：帧间冗余计算优化，降低延迟
- **技术特色**：
  - ⭐ 本地优先（Local-First）：数据不离开本地设备，隐私保护+低碳
  - ⭐ 帧因果（Frame-Causal）Rectified Flow：保证长时间运动一致性
  - ⭐ 实时交互延迟低：鼠标+键盘输入零延迟响应
- **开源情况**：部分开源（Biome Runtime、World Engine 均已发布 GitHub）
- **API 能力**：World Engine 提供 Python API；支持第三方客户端集成

### 开发者生态（GitHub）

- **官方 GitHub 组织**：[github.com/Overworldai](https://github.com/Overworldai) + [github.com/Wayfarer-Labs](https://github.com/Wayfarer-Labs)
- **核心仓库**：

| 仓库 | Stars | 最近更新 | 许可协议 | 说明 |
|------|-------|---------|---------|------|
| [Biome](https://github.com/Overworldai/Biome) | — | 活跃 | MIT | 本地 Runtime 运行时 |
| [World Engine](https://github.com/Wayfarer-Labs/world_engine) | — | 活跃 | MIT | 核心推理库 |
| [Waypoint-1.5-1B](https://huggingface.co/Overworld/Waypoint-1.5-1B) | — | 2026-04 | 模型权重 | HuggingFace 下载 |

## 4. 版本迭代

| 版本 | 发布时间 | 主要变化 |
|------|---------|---------| 
| **Waypoint-1** | 2026年1月 | 首个实时交互 Diffusion 世界模型，证明本地运行可行性 |
| **Waypoint-1.5** | **2026年4月9日**⭐ | 720p+360p 双档位；训练数据量提升100倍；Mac/Windows 支持 |

**Waypoint-1.5 关键迭代亮点**：
- 硬件覆盖从高端 RTX 扩展到游戏本和 Mac
- 视觉保真度和环境一致性显著提升
- 本地安装流程简化（new installer flow）

## 5. 当前状态

- **可用状态**：✅ 已发布（研究预览版）
- **覆盖平台**：本地（Windows/Mac/Linux）+ 云端浏览器
- **开放范围**：全球可访问
- **访问限制**：需 RTX 3090+（720p）或中等配置（360p）

## 6. 规模数据

- **用户规模**：暂无公开 DAU/MAU 数据
- **融资情况**：已完成 **450 万美元 Pre-Seed 融资**（2026年1月披露）
- **增长趋势**：开源社区关注度上升，GitHub 活跃

> ⚠️ 规模数据均标注"暂无公开数据"

## 7. 商业模式

- **定价策略**：基础版免费（本地 Runtime + 云端体验）；商业使用需授权
- **价格档位**：

| 档位 | 价格 | 包含内容 |
|------|------|---------|
| 体验版 | 免费 | Biome 本地运行 + Overworld.stream 云端 |
| World Engine | 免费（MIT） | 第三方集成开发 |
| 商业授权 | 未公开 | 企业级使用 |

- **主要收入来源**：企业授权、技术合作
- **目标客户群**：独立游戏开发者、AI 研究者、创意爱好者

## 8. 投融资情况

- **最新融资**：**450 万美元 Pre-Seed**（2026年1月）
- **投资方**：未披露具体机构（Kindred Ventures 等机构参与跟投）
- **上市状态**：未上市

## 9. 竞品分析

- **所在赛道**：AI 世界模型 / 实时生成式交互引擎
- **主要竞品对比**：

| 维度 | **Waypoint-1.5** | **World Labs (李飞飞)** | **Genie 3 (DeepMind)** | **GWM-1 (Worlds)** |
|------|-----------------|----------------------|----------------------|------------------|
| 厂商 | Overworld | World Labs | Google DeepMind | Worlds |
| 核心卖点 | 本地实时、消费级GPU | 空间智能、3D 生成 | 视频生成控制 | 无限可探索环境 |
| 技术路线 | Diffusion + 本地优先 | 空间生成模型 | 视频生成 | 实时世界引擎 |
| 定价 | 免费基础版 | 未上线 | 研究免费 | 订阅制 |
| 硬件要求 | RTX 3090+（本地） | 大型 GPU 集群 | 云端 | 云端+本地 |
| 进展阶段 | 研究预览 | 早期 | 研究预览 | 已上线 |

- **竞争格局简述**：
  - 世界模型赛道 2026 年加速爆发，DeepMind Genie 3、World Labs、李飞飞等重量级玩家入局
  - Overworld 差异化定位：**本地优先 + 消费级硬件**，而非大厂集群路线
  - "如果只能跑在集群上，就只是 Demo；跑在日常 GPU 上，才能真正改变游戏"

- **差异化定位**：
  > 专注"本地优先"：不是要替代云端渲染，而是让 AI 世界模型真正在每个人手里跑起来——隐私、低延迟、无需联网

## 10. 总结与展望

- **核心优势**：
  1. **消费级硬件实时运行**：720p/60fps 在 RTX 3090~5090 上已验证，工程化能力领先
  2. **本地优先架构**：隐私保护+低碳+离线可用，用户真正拥有数据
  3. **训练效率突破**：100 倍数据量提升带来视觉质量和一致性的质变

- **潜在风险**：
  1. **算力瓶颈**：360p 档覆盖更广硬件但画质损失，高端卡价格门槛仍在
  2. **大厂竞争压力**：DeepMind、World Labs 等资金和技术储备远超 Overworld
  3. **商业化路径模糊**：目前以研究预览为主，企业级变现模式尚不清晰

- **发展趋势**：
  1. Waypoint-2 预计将支持更复杂交互（多角色、物理规则）
  2. Apple Silicon 适配完成后将大幅扩展用户群
  3. 第三方客户端生态扩展，World Engine 有望成为行业标准接口

---

## 📎 参考信息（精选）

1. [Waypoint-1.5: Higher-Fidelity Interactive Worlds for Everyday GPUs](https://huggingface.co/blog/waypoint-1-5) — HuggingFace Blog | 技术深度解析
2. [Overworld Releases Waypoint-1.5](https://gamesbeat.com/overworld-releases-ai-based-waypoint-1-5-real-time-world-simulation-system/) — GamesBeat | 产品发布报道
3. [Overworld 450万美元Pre-Seed融资](https://www.finsmes.com/2026/01/overworld-raises-4-5m-in-pre-seed-funding.html) — FinSMEs | 投融资信息
4. [Introducing Waypoint-1](https://huggingface.co/blog/waypoint-1) — HuggingFace Blog | 初始版本技术解析
5. [World Models: Five Competing Approaches](https://themesis.com/2026/01/07/world-models-five-competing-approaches/) — Themesis | 赛道全景分析
6. [Overworld Official Site](https://over.world/) — 官网 | 产品入口
