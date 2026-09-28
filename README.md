# Leader

面向前端负责人的组织治理与 AI 研发协作知识库。

这里沉淀从小团队走向 30+ 人规模时可以复用的管理方法、责任机制、人才标准、工程底座和 AI 开发治理实践。内容不是泛泛的管理口号，而是围绕真实团队场景整理的 Skill、参考材料、模板和阶段性产出物。

## 适合谁

- 正在从直接管理需求转向管理业务线和负责人的前端负责人
- 需要建设职级、人才梯队、评审和团队运行机制的技术负责人
- 希望把 AI 从个人工具使用推进为团队研发治理闭环的工程管理者
- 需要可直接参考的组织设计、工程效能和管理文档的团队

## 从这里开始

按你的问题选择入口：

| 你正在解决的问题 | 推荐阅读 |
| --- | --- |
| 团队超过 30 人后，如何保持稳定交付 | [30 人前端团队可经营组织运行系统](.agents/skills/frontend-leadership/frontend-leader/references/organization-operating-system.md) |
| 如何在固定大团队内扩展多个子业务线 | [前端负责人管理业务线的方法](.agents/skills/frontend-leadership/frontend-leader/references/business-line-management.md) |
| 如何规划团队规模化建设路线 | [前端团队规模化实施路线图](.agents/skills/frontend-leadership/frontend-leader/references/implementation-roadmap.md) |
| 如何把 AI 纳入需求、开发、审查和复盘流程 | [前端 AI 开发治理闭环](.agents/skills/frontend-leadership/frontend-leader/references/ai-development-loop.md) |
| 如何建立可复核的职级与评审标准 | [前端岗位职级标准与发展指南](.agents/skills/frontend-leadership/people-culture-manager/references/frontend-leveling-standards.md) |
| 如何按事实记录团队和个人价值 | [价值证据台账模板](.agents/skills/frontend-leadership/frontend-leader/references/value-evidence-ledger-template.md) |

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

## 这个仓库的特点

1. **以责任和结果为主线**：不只记录做过什么，更说明谁负责、如何判断、如何验收。
2. **以机制替代个人英雄主义**：把管理经验整理成负责人机制、SOP、评审标准和运行节奏。
3. **以可复用资产为交付物**：优先沉淀 Skill、模板、清单、路线图和案例，而不是只写观点。
4. **以真实约束为背景**：关注团队规模、业务线变化、授权边界、质量风险和长期维护成本。

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

## 使用方式

### 人阅读

先从“从这里开始”选择一个具体问题，再沿着文档中的引用继续阅读。建议不要一次性通读全部内容，而是围绕当前团队问题抽取责任边界、运行节奏和验收证据。

### Agent 使用

`.agents/skills/` 是本仓库唯一的 Skill 主资产源。使用支持 Skill 路由的 Agent 时：

1. 先读取 `.agents/skills/README.md`。
2. 根据任务选择对应目录下的 `SKILL.md`。
3. 只加载该 Skill 指向的必要参考材料、模板或资产。
4. 输出时优先复用仓库中已有的口径、清单和案例。

## 参与和反馈

欢迎围绕以下方向提出 Issue 或 Pull Request：

- 补充可验证的团队治理案例和结果证据
- 改进模板、清单和文档结构
- 指出过时、含糊或缺少适用边界的内容
- 分享不同规模团队下的适配方式

新增或更新 Skill 时，请遵守 [AGENTS.md](AGENTS.md) 和 [.agents/skills/README.md](.agents/skills/README.md) 中的目录、元数据和引用规则。

## 更新

项目会持续围绕前端组织治理、人才机制、工程效能和 AI 协作进行整理。具体变更见 [CHANGELOG.md](CHANGELOG.md)，提交信息遵守 `type(scope): message` 规范。
