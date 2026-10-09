# Agent Skills Index

本目录是当前仓库唯一的 Skill 主资产源。所有 Agent 在处理任务前，应先根据本索引选择相关 Skill，再读取对应的 `SKILL.md` 和必要的参考材料。

## 目录原则

- 新增 Skill 统一放在 `.agents/skills/<顶级目录>/<技能目录>/`。
- 每个 Skill 必须包含 `SKILL.md`。
- `SKILL.md` 的 `name` 必须等于 `<顶级目录>-<技能目录>`。
- `SKILL.md` 必须补齐 `metadata.pattern`、`metadata.author`、`metadata.version`。
- `metadata.pattern` 必须等于 `<顶级目录>/<技能目录>`。
- 参考材料放在 `references/`，模板放在 `templates/`，静态模板或表单放在 `assets/`。
- 新增、更新、删除都只在 `.agents/` 下进行。
- 不把 Skill 内容写入 `.cursor/`、`.trae/`、`.qoder/`、`.vscode/` 或根目录 `skills/`。

## 前端负责人架构思考类

| Skill | 入口 | 适用场景 |
| --- | --- | --- |
| frontend-leadership-frontend-leader | `frontend-leadership/frontend-leader/SKILL.md` | 前端负责人管理规划、个人管理时间线与事实校验、价值证据台账、30+ 团队治理、固定大团队与多子业务线动态扩展、纵横矩阵可经营运行系统、业务线负责人机制、副手梯队、工程底座、AI 开发治理闭环、管理文章写作、多视角审稿与降 AI 味、前端负责人向产研 AI 协作架构推动者成长 |
| frontend-leadership-org-architect | `frontend-leadership/org-architect/SKILL.md` | 前端组织架构、业务线划分、固定大团队与子业务线负责人分层、纵横矩阵运行边界、向上汇报、价值表达、危机处理、组织顶层设计 |
| frontend-leadership-people-culture-manager | `frontend-leadership/people-culture-manager/SKILL.md` | 招聘、面试、绩效、1v1、人才梯队、团队稳定性、临时调动、敏感反馈、高情商沟通 |
| frontend-leadership-tech-efficiency-architect | `frontend-leadership/tech-efficiency-architect/SKILL.md` | 架构、基建、组件库、监控稳定性、AI 效能、质量治理、横向能力可经营机制、技术债、AI Coding 跃迁四图总览、产研组织升级、AI 实践与 Harness 工程 |

### 写作与图文整理规则

事故管理通报：[线上问题通报层级参考](frontend-leadership/org-architect/references/incident-notification-levels.md)。适用于 P0/P1 同步 CTO、CTO 判断老板知情范围，以及历史通报口径与现行 SOP 的衔接。

管理事实来源：[个人管理时间线](frontend-leadership/frontend-leader/references/personal-management-timeline.md)。已记录线上事故响应机制完成宣讲、团队认可及后续版本管理安排；演练计划与实际效果分别记录，宣讲日期待补。

| 资料 | 入口 | 适用场景 |
| --- | --- | --- |
| 管理文章写作与降 AI 味 | [management-article-writing.md](frontend-leadership/frontend-leader/references/management-article-writing.md) | 文章、分享稿、AI 实践文档与架构说明；区分 Agent 指令、事实材料与读者正文，清理对话残留，核对图文及实践状态 |

### 职级标准与评审资料

| 文档 | 入口 | 适用场景 |
| --- | --- | --- |
| 前端岗位职级标准与发展指南 | [frontend-leveling-standards.md](frontend-leadership/people-culture-manager/references/frontend-leveling-standards.md) | 全员职级要求、P4-P5 技术与管理双通道、个人实践及成长证据 |
| 前端职级评审、定级与校准基线 | [frontend-leveling-review-baseline.md](frontend-leadership/people-culture-manager/references/frontend-leveling-review-baseline.md) | 负责人评审、长期治理证据认定、责任机会、分歧复核与结果反馈 |

### AI Coding 跃迁：四图与配套说明

| 资料 | 入口 | 适用场景 |
| --- | --- | --- |
| AI Coding 跃迁总览 | [ai-coding-evolution.md](frontend-leadership/tech-efficiency-architect/references/ai-coding-evolution.md) | 统一阅读入口，依次串联四张图及其实践边界 |
| AI 驱动组织运行模式升级讨论：内部分享 | [分享稿与页面留存](frontend-leadership/tech-efficiency-architect/references/ai-organization-operating-model-sharing.md) | 已开展的分享，包含协作分工、前端样板和三个试点建议；后续实施与效果另行记录 |
| AI 递进节奏图 | [ai-coding-progression.png](frontend-leadership/tech-efficiency-architect/assets/ai-coding-progression.png) | 表达、项目接入、加法与减法，收束到工程化建设 |
| AI 驱动产研组织升级（构思-实践版） | [说明](frontend-leadership/tech-efficiency-architect/references/ai-driven-product-rd-organization-upgrade.md) · [原图](frontend-leadership/tech-efficiency-architect/assets/ai-product-rd-collaboration-overview.png) | 组织运行升级、目标、思想、治理评估 |
| AI 实践架构与 Harness 工程 | [说明](frontend-leadership/tech-efficiency-architect/references/ai-product-rd-collaboration-architecture.md) · [原图](frontend-leadership/tech-efficiency-architect/assets/ai-practice-harness-architecture.png) | 前端在产研中的输入关系、支撑能力与 V1.0/V2.0 实践流程 |
| Skills 结构与数量规划 | [说明](company-public/skill-governance/references/ai-coding-skills-planning.md) · [原图](company-public/skill-governance/assets/ai-coding-skills-structure.png) | 需求 2、设计 1、开发 7、提测 2 个预留位置，按场景加载，未命名位置保留待定 |
| 前端 AI 开发治理闭环 | [ai-development-loop.md](frontend-leadership/frontend-leader/references/ai-development-loop.md) | 开发前、中、后的操作步骤、人员责任及效果证据边界 |

## 公司公共类

| Skill | 入口 | 适用场景 |
| --- | --- | --- |
| company-public-skill-governance | `company-public/skill-governance/SKILL.md` | Skill 创建规范、目录质量校验、文档归属整理、对话共识建议录入、AI Coding 的 Skills 场景与数量规划 |
| company-public-wf-openspec-mode | `company-public/wf-openspec-mode/SKILL.md` | AI 落地到真实项目的 OpenSpec/SDD 思路参考、proposal/spec/tasks 机制理解、模型选择；当前 leader 项目不作为强制实践工作流 |

## 可视化类

| Skill | 入口 | 适用场景 |
| --- | --- | --- |
| visualization-mermaid-style | `visualization/mermaid-style/SKILL.md` | 中文 Mermaid 流程图的统一主题、布局、语义配色和可读性规则 |

## 更新要求

- 新增、移动、删除 Skill 时，同步更新本索引。
- 修改 Skill 的适用场景时，同步更新根目录 `AGENTS.md` 的常用路由。
- 引用外部仓库内容时，应复制到 `.agents/skills/` 并注明来源或保留原目录结构，不在本仓库保留外部 checkout。
