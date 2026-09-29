# Frontend Leadership · 前端负责人实战手册与 AI Skills

面向前端负责人与技术管理者，提供团队管理、职级评审、人才培养和 AI 研发协作的参考材料、模板与使用指南。

你可以从一份评审标准或证据记录模板开始，也可以让 AI 读取仓库中的 Skill，结合你的实际情况辅助整理管理方案。规模化治理部分提供了从小团队走向 30+ 人、多业务线组织的实践参考。

[立即使用](#立即使用) · [AI 辅助管理](#ai-辅助管理) · [深入阅读](#深入阅读) · [完整 Skill 索引](.agents/skills/README.md)

## 立即使用

选择一个当前要解决的问题，打开对应资料：

| 你要做什么 | 入口 | 第一步 |
| --- | --- | --- |
| 理解职级责任、梳理成长方向 | [前端岗位职级标准与发展指南](.agents/skills/frontend-leadership/people-culture-manager/references/frontend-leveling-standards.md) | 对照 P2-P5 的责任范围，梳理当前职责与目标职级的差距 |
| 准备职级评审、统一评审依据 | [前端职级评审、定级与校准基线](.agents/skills/frontend-leadership/people-culture-manager/references/frontend-leveling-review-baseline.md) | 按评审输入整理事实、个人贡献和持续结果证据 |
| 准备复盘或述职，记录工作价值 | [价值证据台账模板](.agents/skills/frontend-leadership/frontend-leader/references/value-evidence-ledger-template.md) | 选择一件已完成的工作，填写一张单条价值证据卡 |

职级与评审材料基于特定组织场景整理，使用时先对齐自己团队的岗位职责、职级体系和授权范围。记录工作结果时保留基线、统计周期和证据出处。

## AI 辅助管理

仓库中的 Skill 定义了任务处理方法，并指向相关资料。先将仓库克隆或下载到本地，用能够读取项目文件的 AI 编程助手打开仓库目录；按下面的示例明确要求读取文件即可，不依赖工具自动识别 Skill。

### 试一次：把工作记录整理成价值证据卡

将以下输入复制给助手，并把方括号替换为自己的实际信息。这是任务输入示例，输出需要结合原始记录核对。

```text
请先读取 AGENTS.md 和 .agents/skills/README.md，再读取：
.agents/skills/frontend-leadership/frontend-leader/SKILL.md
.agents/skills/frontend-leadership/frontend-leader/references/value-evidence-ledger-template.md

请根据以下事实，帮我整理一张价值证据卡：
- 工作事项：[最近完成的一件具体工作]
- 背景与目标：[当时的问题，以及希望改善什么]
- 我的责任和关键判断：[本人负责什么，做过哪些取舍]
- 团队及协作方贡献：[其他人完成的部分]
- 已知结果与证据：[前后变化、统计周期、可核对的记录]
- 当前缺失的信息：[尚未统计或无法确认的内容]

请按模板输出证据卡草稿，并列出待补证据与需要我确认的判断。
缺失内容标注“待补充”，不要编造数据、因果关系或已完成的成果。
仓库中的团队背景与案例仅作方法参考，不代表我的实际经历。
```

拿到草稿后，重点核对结果是否有证据支撑、个人与团队贡献是否分清、哪些判断仍需验证。其他任务可从[完整 Skill 索引](.agents/skills/README.md)选择组织、人才或技术效能方向。

## 深入阅读

需要设计团队运行机制或推进研发协作时，再按问题阅读以下材料，并结合团队规模、管理授权和业务阶段调整：

| 你正在解决的问题 | 推荐阅读 |
| --- | --- |
| 团队超过 30 人后，如何保持稳定交付 | [30 人前端团队可经营组织运行系统](.agents/skills/frontend-leadership/frontend-leader/references/organization-operating-system.md) |
| 如何在固定大团队内扩展多个子业务线 | [前端负责人管理业务线的方法](.agents/skills/frontend-leadership/frontend-leader/references/business-line-management.md) |
| 如何规划团队规模化建设路线 | [前端团队规模化实施路线图](.agents/skills/frontend-leadership/frontend-leader/references/implementation-roadmap.md) |
| 如何把 AI 纳入需求、开发、审查和复盘流程 | [前端 AI 开发治理闭环](.agents/skills/frontend-leadership/frontend-leader/references/ai-development-loop.md) |

## 核心内容

### 前端团队治理

- 30+ 人团队的组织运行、责任边界和季度经营机制
- 固定大团队与动态子业务线的扩展方式
- 业务线负责人、副手和梯队人选的授权与培养
- 交付责任、风险上浮、复盘和质量治理

### 人才与组织机制

- P2-P5 前端岗位职级标准与发展指南
- 职级评审、定级和跨团队校准基线
- 招聘、面试、1v1、反馈、绩效和团队稳定性材料
- 面向真实管理结果的成长证据记录方式

### 工程效能与 AI 协作

- 工程底座、质量稳定性和跨业务线能力建设
- 从 AI 工具使用到团队级研发治理闭环
- 需求澄清、方案评审、代码审查、自测和知识沉淀
- AI API 网关、产研协作和组织升级实践

## 目录结构

```text
.
├── AGENTS.md                         # Agent 协作规则与 Skill 路由
├── README.md                         # 项目入口与精选导航
├── CHANGELOG.md                      # 项目更新记录
├── .agents/skills/                   # 可复用 Skill、参考材料和模板
│   ├── company-public/
│   └── frontend-leadership/
└── outputs/                          # 阶段性文档与制度草案
```

所有可复用 Skill、参考材料和模板统一维护在 `.agents/skills/`，完整使用与维护规则见 [AGENTS.md](AGENTS.md)。

## 参与和反馈

欢迎围绕以下方向提出 Issue 或 Pull Request：

- 补充可验证的团队治理案例和结果证据
- 改进模板、清单和文档结构
- 指出过时、含糊或缺少适用边界的内容
- 分享不同规模团队下的适配方式

新增或更新 Skill 时，请遵守 [AGENTS.md](AGENTS.md) 和 [.agents/skills/README.md](.agents/skills/README.md) 中的目录、元数据和引用规则。

## 更新

项目会持续围绕前端组织治理、人才机制、工程效能和 AI 协作进行整理。具体变更见 [CHANGELOG.md](CHANGELOG.md)，提交信息遵守 `type(scope): message` 规范。
