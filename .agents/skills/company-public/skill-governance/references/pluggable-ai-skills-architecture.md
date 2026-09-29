# 可插拔 Skill 架构：资产归属与场景加载

Skill 需要同时解决两个问题：资料由谁维护，以及当前任务需要加载哪些方法。物理目录按稳定的业务域或职能归属组织，执行时按任务场景选择入口，二者不必使用同一套分类。

业务知识、项目规则和工作流程分别维护。SDD、OpenSpec 等工作方式可以按项目需要调整，领域规则与已确认事实仍保持可追溯。

## 两级目录与资产归属

本仓库采用 `.agents/skills/<归属目录>/<技能目录>/SKILL.md` 作为 Skill 入口。两级约束指 Skill 的归属层级，不限制其中 references、templates、assets 的必要组织。

```text
.agents/skills/
├── frontend-leadership/
│   ├── frontend-leader/
│   │   ├── SKILL.md
│   │   └── references/
│   ├── org-architect/
│   │   ├── SKILL.md
│   │   └── references/
│   ├── people-culture-manager/
│   │   ├── SKILL.md
│   │   ├── references/
│   │   └── assets/
│   └── tech-efficiency-architect/
│       ├── SKILL.md
│       ├── references/
│       └── assets/
└── company-public/
    ├── skill-governance/
    │   ├── SKILL.md
    │   ├── references/
    │   └── assets/
    └── wf-openspec-mode/
        ├── SKILL.md
        ├── references/
        └── templates/
```

目录归属用于明确维护责任，可以配合 CODEOWNERS 指定审查人；CODEOWNERS 本身不提供文件读取或细粒度访问控制，访问权限仍由仓库和相关系统配置。

## 按场景选择入口

需求澄清、设计、实现或测试任务，可以跨稳定的资产目录选择必要 Skill。可复用业务方法和独立的处理动作都可以成为入口，是否拆分取决于职责、触发条件和实际使用记录，不要求每个 Skill 都对应一个组织节点。

[AI Coding 的 Skills 场景与数量规划](ai-coding-skills-planning.md)按需求、设计、开发、提测预留入口。它描述业务项目的场景规划，不要求当前知识仓库改成相同数量或复制一套阶段目录。

跨角色任务需要共享已经确认的需求、接口和验收资料。相同规则保留一个维护位置，多个入口引用；不同角色的假设与待确认项不能混成一个已生效结论。

## 公共入口与按需读取

公共 Skill 可以负责识别场景、说明共享约束并指向资料。仅创建 SKILL.md 不会使它自动发现任务或主动分发内容，实际行为取决于 Agent 的加载机制、入口说明和执行流程。

一次任务先读取必要入口，再加载相关参考材料。公共入口保持简短，详细的设计规范、接口规则和案例放到参考文件；避免每次调用都读入全部历史资料。

## 工作流与知识分开维护

项目级指导文件说明协作与验证约定，Skill 提供可复用处理方法，任务资料记录本次目标和状态。工作流负责组织这些材料进入执行过程，并保留人工确认、测试与复盘。

在本仓库中，OpenSpec/SDD 用于理解业务项目的实践方式，不启用完整执行流。目标业务项目实际接入前，还需确定模板、工具版本、验证器与团队约定。

架构调整后，核对入口是否清楚、资料是否重复、引用是否有效，以及维护人和实际使用方式是否明确。数量增加或减少都应服务于任务结果与维护成本。
