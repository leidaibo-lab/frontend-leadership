---
name: "visualization-mermaid-style"
description: "生成或整理中文 Mermaid 流程图时，复用统一的主题、布局、语义配色和可读性规则；不负责定义具体业务流程。"
metadata:
  pattern: "visualization/mermaid-style"
  author: "frontend-leadership"
  version: "1.0.0"
---

# 中文 Mermaid 流程图样式

## 适用范围

当用户要求绘制、优化或导出中文 Mermaid 流程图时，优先复用本 Skill 的样式配置。适用于事故响应、研发流程、发布流程、审批流程等流程图。

本 Skill 只定义绘图样式和表达规则，不定义具体业务节点、角色职责或流程结论。业务内容由当前任务单独确定。

## 标准配置

将下面的初始化配置放在 Mermaid 代码块最前面，并根据图表类型调整 `flowchart` 参数：

```mermaid
%%{init: {
  "theme": "base",
  "themeVariables": {
    "background": "#FFFFFF",
    "fontFamily": "PingFang SC, Microsoft YaHei, sans-serif",
    "fontSize": "14px",
    "primaryColor": "#EAF2FF",
    "primaryTextColor": "#17324D",
    "primaryBorderColor": "#4D7CFE",
    "lineColor": "#7A8AA0",
    "edgeLabelBackground": "#FFFFFF",
    "clusterBkg": "#F7F9FC",
    "clusterBorder": "#D9E2EC"
  },
  "flowchart": {
    "htmlLabels": true,
    "curve": "basis",
    "nodeSpacing": 32,
    "rankSpacing": 46,
    "padding": 16,
    "useMaxWidth": true
  }
}}%%
```

## 标准语义配色

流程图需要区分节点语义时，使用以下 `classDef`。颜色用于表达节点类型，不绑定具体业务领域：

```mermaid
classDef trigger fill:#EAF2FF,stroke:#4D7CFE,color:#17324D,stroke-width:1.5px;
classDef decision fill:#FFF4DF,stroke:#E6A23C,color:#6B4300,stroke-width:1.5px;
classDef stop fill:#FFF0F0,stroke:#E45757,color:#6B1F1F,stroke-width:1.5px;
classDef action fill:#EFF8F1,stroke:#4CAF6A,color:#1F4D2B,stroke-width:1.5px;
classDef verify fill:#F1ECFF,stroke:#8064D8,color:#352266,stroke-width:1.5px;
classDef record fill:#F5F7FA,stroke:#98A2B3,color:#344054,stroke-width:1.5px;
```

| 样式 | 用途 |
| --- | --- |
| `trigger` | 入口、发现、启动、接管 |
| `decision` | 判断、分支、条件确认 |
| `stop` | 止损、阻断、风险隔离 |
| `action` | 排查、处理、执行、协作 |
| `verify` | 验证、恢复、观察、评估 |
| `record` | 记录、复盘、关闭、沉淀 |

使用时将节点 ID 放入对应的 `class` 声明，例如：

```mermaid
class A,C trigger;
class B decision;
class D,E action;
class F record;
```

## 使用规则

- 优先使用 `flowchart TD`；流程步骤较多且横向阅读更自然时，可改用 `LR`。
- 节点文案保持短句，长说明使用 `<br/>` 换行，避免一个节点承载多个动作。
- 判断节点使用 `{}`，并为分支连线补充明确的条件文本。
- 颜色只表达节点语义，不为不同业务线随意增加新颜色。
- 同一张图的主流程、异常分支和复盘收尾应保持统一字体、间距和边框风格。
- 业务流程复杂时优先拆分阶段或使用 `subgraph`，不要通过缩小字体容纳过多节点。
- 输出图片前检查中文字体、节点文字是否溢出、连线是否穿过文字，以及移动端或窄页面下的可读性。
- Mermaid 渲染器对主题变量的支持可能存在版本差异；若局部变量不生效，保留 `classDef` 作为主要视觉控制手段。

## 输出要求

生成图表时应同时给出：

1. 可直接复制渲染的 Mermaid 代码；
2. 必要的节点样式分配；
3. 当图表过于复杂时，对拆分或布局调整的简短说明。
