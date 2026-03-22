# OpenArt Worlds（2026-03-22）

> 📅 分析日期：2026-03-22
> 🔍 数据来源：Tavily 搜索（主力）、官方新闻稿、Press Release、GitHub 仓库分析等多源综合

---

## ⚡ 一句话速览

> OpenArt Worlds 是由 AI 创作平台 OpenArt 于 2026 年 3 月 18 日推出的**首个持久性空间创意环境**，基于 World Labs 空间智能 AI 技术，用户可通过文本提示或图片生成可自由导航的 3D 世界，并直接拍摄生产级内容，解决了 AI 创作中场景一致性和构图控制两大核心痛点。

---

## 1. 产品概览

- **产品名称**：OpenArt Worlds
- **所属厂商/公司**：OpenArt（由前 Google 员工 Coco Mao 和 John Qiao 创立）
- **产品类型**：世界模型 / 持久性 3D AI 创作环境
- **首次上线时间**：2026 年 3 月 18 日
- **最新版本/代次**：首发版本（v1.0）
- **官网地址**：https://openart.ai/suite/world

## 2. 核心功能

按功能模块分类列出，差异化亮点用 ⭐ 标注：

- **持久 3D 世界生成** ⭐：输入文本提示或图片，即刻生成可自由行走探索的完整 3D 环境，世界永久存在、不随切换消失
- **场景一致性保障** ⭐：每个世界均为持久环境，不同镜头/角度下场景元素严格保持一致，彻底解决系列化内容创作的核心痛点
- **空间构图控制** ⭐：用户可走入世界、选择任意角度和构图进行拍摄（"Take the shot"），构图完全由创作者主导而非模型随机决定
- **多模态输入**：支持文本转 3D 世界、图片转 3D 世界两种输入模式
- **生产级图像输出**：拍摄瞬间可添加角色、物体等提示词元素，输出可直接用于生产的高质量 2D 图像
- **3D 格式导出（规划中）**：未来版本将支持 Gaussian Splat 和 3D Mesh 格式导出，无缝集成 Unreal Engine、Blender 等专业工具
- **World Labs 独家驱动** ⭐：由 World Labs 空间 AI 模型提供支持，OpenArt 为其独家消费者端合作平台

## 3. 技术能力评估

- **底层技术架构**：扩散模型（Diffusion Models）+ 神经辐射场（NeRF）实时渲染 + 多模态语义理解模块，三者深度耦合构建动态响应用户空间行为的三维生成内核
- **模型基座**：调用 World Labs 空间智能大模型（非 OpenArt 自研基座），为 World Labs 首个面向消费者端的独家合作产品
- **关键技术参数**：
  - 参数量：暂无公开数据
  - 上下文窗口：空间上下文（用户导航路径实时影响生成）
  - 多模态支持：文本→3D、图片→3D
  - 实时渲染：毫秒级空间响应（视线移动、手势、语音均可触发世界演化）
- **Benchmark 表现**：暂无公开 Benchmark 数据（世界模型为新兴赛道，尚无标准化评测体系）
- **技术特色**：
  - "生成即存在"（Generation-as-Existence）架构：彻底跳脱"输入提示—等待推理—输出静态图"三段式流程
  - 用户视线、停留时长、手势轨迹、语音节奏均可驱动世界在隐空间实时演化
  - 光影折射角自适应用户设备空间姿态
- **开源情况**：闭源（World Labs 模型未开源），OpenArt 平台本身有开源组件（ComfyUI 工具集）
- **API 能力**：暂无独立 API 开放，OpenArt 平台提供 API 接口

### 开发者生态（GitHub）

- **官方 GitHub 组织**：[OpenArt-AI](https://github.com/OpenArt-AI)（88 followers）
- **核心仓库**：

| 仓库 | Stars | Forks | 最近更新 | 许可协议 | 说明 |
|------|-------|-------|---------|---------|------|
| [ComfyUI-Assistant](https://github.com/OpenArt-AI/ComfyUI-Assistant) | 21 | 3 | 2024-05 | - | ComfyUI Assistant 自定义节点 |
| [workflow-model-list](https://github.com/OpenArt-AI/workflow-model-list) | 3 | 22 | 2024-10 | - | 工作流模型列表 |
| [ComfyUI-Manager](https://github.com/OpenArt-AI/ComfyUI-Manager) | 3 | 2,067 | 2024-06 | GPL-3.0 | ComfyUI 管理器（Fork） |
| [ComfyUI_examples](https://github.com/OpenArt-AI/ComfyUI_examples) | 2 | 1,290 | 2023-12 | - | ComfyUI 工作流示例 |
| [ComfyUI-OpenArt-fal-API](https://github.com/OpenArt-AI/ComfyUI-OpenArt-fal-API) | 2 | 50 | 2025-08 | Apache-2.0 | FAL API 集成节点 |

- **官方 SDK 覆盖**：JavaScript、Python（通过 ComfyUI 节点）
- **社区活跃度**：总体规模偏小，仓库 Stars 数量较低，以 Fork 贡献为主
- **第三方生态**：全球最大 ComfyUI 工作流分享平台之一，用户可上传自建工作流（平台积累了大量社区工作流资源）

## 4. 版本迭代

| 版本 | 发布时间 | 主要变化 |
|------|---------|---------| 
| v1.0（首发） | 2026-03-18 | 首次发布：文本/图片生成可导航 3D 世界，持久空间环境，构图控制，World Labs 驱动 |

**首发版本关键迭代亮点**：
- 首个消费级持久性 3D 创作空间
- 场景一致性通过设计保证（世界永久存在）
- 首次实现消费级 AI 平台的空间构图控制能力
- 未来路线图：Gaussian Splat、3D Mesh 导出 → 对接 Unreal Engine、Blender

（注：首发版本，无前代对比）

## 5. 当前状态

- **可用状态**：✅ 已上线（2026-03-18 正式发布）
- **覆盖平台**：Web（主平台）、API（平台级）
- **开放范围**：全球可用，面向下一代 AI 原生创作者、电影制作人、故事讲述者
- **访问限制**：需注册账号，部分高级功能需付费订阅

## 6. 规模数据

- **用户规模**：600 万 + 注册用户（平台整体用户量）
- **收入规模**：2025 年 ARR 约 1,200 万美元（另一数据：2025 年已达 1,600 万美元 ARR），同比增长约 1,100%
- **增长趋势**：用户数从 2022-2023 年的起步阶段增长至 600 万 +；收入从约 100 万美元量级增长至 1,200-1,600 万美元 ARR（2025年）
- **市场地位**：AI 图像/视频生成平台领域头部玩家之一；3D 世界生成赛道新兴领跑者（首个消费级持久空间创作环境）

> ⚠️ OpenArt Worlds 作为独立功能模块暂无单独规模数据，以上为 OpenArt 平台整体数据

## 7. 商业模式

- **定价策略**：Freemium（免费增值）+ 订阅制
- **价格档位**：

| 档位 | 月付价格 | 年付价格（月均） | 包含内容 |
|------|------|------|---------| 
| Free | $0 | $0 | 基础图像生成额度 |
| Essential | $14 | $7 | ~12K Credits，更多模型访问 |
| Advanced | $29 | $14.5 | ~24K Credits，更高分辨率，更多高级功能 |
| Infinite | $56 | $28 | 无限额度，高级模型全覆盖 |

- **主要收入来源**：To C 订阅（核心）+ To B 企业级服务（推测）
- **目标客户群**：AI 原生创作者、电影制作人、故事讲述者、游戏开发者、内容创作者

## 8. 投融资情况

- **公司最新估值**：暂无公开估值数据
- **累计融资额**：约 400 万美元（含 2022 年种子轮 + 2023 年种子轮，具体金额来源差异较大）
- **融资历史**：

| 轮次 | 时间 | 金额 | 主要投资方 |
|------|------|------|----------|
| 种子轮 | 2022 年 | 未披露 | Canaan Partners、Felix Capital 等 |
| 种子轮 | 2023 年 | $400 万–$500 万 | Basis Set Ventures、DCM Ventures、Calm Ventures |

- **上市状态**：未上市
- **团队规模**：约 10-16 人（高度精简，小团队高效运转）

## 9. 竞品分析

- **所在赛道**：AI 世界模型 / 3D 场景生成 / 沉浸式 AI 创作平台
- **主要竞品对比**：

| 维度 | OpenArt Worlds | World Labs | OpenAI Sora | Meta Movie Gen |
|------|---------------|------------|-------------|----------------|
| 厂商 | OpenArt | World Labs（李飞飞联合创立） | OpenAI | Meta |
| 核心卖点 | 持久 3D 空间 + 消费级 | 大规模 3D 世界生成、API | 长视频生成、世界模拟器 | 个性化短视频生成 |
| 技术路线 | Diffusion + NeRF（World Labs 模型） | 自研空间智能大模型 | 自研视频生成模型 | 自研视频生成模型 |
| 定价 | 订阅制（$7-$28/月） | API 付费 | ChatGPT 订阅绑定 | 免费/企业 |
| 优势 | 消费级首个持久 3D、World Labs 独家 | 学术背景强、大规模生成能力强 | 品牌强、算力强 | Meta 生态 |
| 劣势 | 依赖第三方模型、规模数据少 | 仅限 API、消费者端空白 | 视频非 3D 交互 | 消费级功能有限 |

- **竞争格局简述**：3D 世界生成赛道目前处于早期阶段，World Labs 为技术先行者但以 API 为主，OpenArt Worlds 抢占了消费级持久 3D 创作空白；Sora 等视频生成工具提供"世界模拟"能力但非真正可交互 3D 世界
- **差异化定位**：首个将"持久性"和"空间可导航性"同时实现并面向消费者开放的 AI 创作工具，强调"走入其中"而非"生成图像"的范式跃迁

## 10. 总结与展望

- **核心优势**：
  1. **场景一致性**：通过"持久世界"设计从根本上解决系列化内容创作的最大痛点
  2. **空间创作临场感**：用户不再是"指令发出者"，而是以具身方式参与世界构建
  3. **World Labs 独家合作**：获取世界模型领域前沿技术，消费级首发优势明显

- **潜在风险**：
  1. **技术依赖**：核心模型来自 World Labs，非完全自研，存在合作变动风险
  2. **商业化验证**：虽平台整体 ARR 表现亮眼，但 3D 世界生成作为新功能其付费转化率有待验证
  3. **算力成本**：实时 3D 渲染的推理成本显著高于静态图像生成，规模化后的毛利压力

- **发展趋势**：
  1. 导出格式扩展（Gaussian Splat → Blender/Unreal Engine），向专业影视游戏工作流渗透
  2. 多人协作世界构建（路线图推测）
  3. 与 AI 视频生成深度整合（世界 → 关键帧 → 视频），成为 AI 影视工作流的中间节点
  4. 平台整体向"AI 原生创作操作系统"演进，OpenArt Worlds 为核心差异化功能

---

## 📎 参考信息（精选）

1. [OpenArt Launches Worlds — The First Persistent Spatial Creative Environment](https://openart.ai/blog/post/openart-worlds-press-release) — OpenArt 官方新闻稿 | 核心产品信息
2. [OpenArt World：AI创作进入沉浸式新时代](https://www.showapi.com/news/article/69bcb0f34ddd79ab6706983b) — 技术博客 | 技术架构深度解析
3. [OpenArt at $12M ARR growing 1,100% YoY](https://sacra.com/research/openart-at-12m-arr/) — Sacra | ARR 规模增长数据
4. [OpenArt - 2026 Company Profile, Team, Funding](https://tracxn.com/d/companies/openart/__rGLZ4jZtTKFqOnIFJpVIpXqrPEtJHfzKwCfxXxYFnns) — Tracxn | 融资历史
5. [Generating Bigger and Better Worlds](https://www.worldlabs.ai/blog/bigger-better-worlds) — World Labs 官方博客 | 3D 世界生成技术背景
6. [OpenArt - GitHub Organization](https://github.com/OpenArt-AI) — GitHub | 开发者生态
7. [The Paintbrush Belongs to Everyone: The OpenArt Story](https://openart.ai/blog/post/the-openart-story) — OpenArt 官方 | 公司创始人背景
8. [How OpenArt hit $12M revenue with a 11 person team in 2025](https://getlatka.com/companies/openart.ai) — Latka | 团队规模收入
