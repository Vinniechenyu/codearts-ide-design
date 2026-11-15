# CodeArts IDE Design

CodeArts IDE / 码道代码智能体的体验设计材料集，汇集业界洞察、竞品分析、产品方案、交互原型与组件规范，覆盖 IDE、ADE、Space、Work 和 CLI 等产品形态。

**[在线浏览全部材料](https://vinniechenyu.github.io/codearts-ide-design/)**

首页提供按类型 / 按产品形态的双维度目录，支持搜索、深浅模式、卡片置顶与多版本选择。当前收录 **18 份材料**：8 份交互原型、6 份业界洞察与竞品分析、2 份专项分析、1 份方法论、1 份组件规范。

> 本仓库用于设计阅读与交互演示。原型中的任务执行、用量、权限等交互不代表已接入真实后端服务。

## 快速入口

- [CodeAgent 研发用量驾驶舱](https://vinniechenyu.github.io/codearts-ide-design/codeagent-console/)：部门用量、个人用量、权限管理。
- [CodeAgent Desktop 任务起点](https://vinniechenyu.github.io/codearts-ide-design/codeagent-desktop/#new-task)：能力卡组、专家直达、Agent / Workflow 与任务提交。
- [码道 CodeArts Space 一站式工作台](https://vinniechenyu.github.io/codearts-ide-design/madao-space/)：通用 / 编程双模式、工作线、产物评审与验收。
- [码道 Work 项目版](https://vinniechenyu.github.io/codearts-ide-design/codearts-space/project.html?v=0817a)：项目、计划、任务验收、知识与资产。
- [生成响应体验优化专项](https://vinniechenyu.github.io/codearts-ide-design/madao-response-deck/?v=brief-0713-2)：实测证据、根因分析与响应体验方案。
- [Agent 对话式交互指南](https://vinniechenyu.github.io/codearts-ide-design/ai-dialogflow-components/)：过程结构、可复用组件与状态机。

## 材料目录

以下按首页类型分组；多版本材料链接指向首页当前默认版本。目录以根 `index.html` 中的 `ITEMS` 为准。

### 交互原型

| 材料 | 产品形态 | 在线预览 |
|---|---|---|
| CodeAgent · 研发用量驾驶舱管理台 | Space | [打开](https://vinniechenyu.github.io/codearts-ide-design/codeagent-console/) |
| CodeAgent Desktop · 任务起点首页交互原型 | Space | [打开](https://vinniechenyu.github.io/codearts-ide-design/codeagent-desktop/#new-task) |
| 码道CodeArts Space · 一站式工作台交互原型 | Space | [打开](https://vinniechenyu.github.io/codearts-ide-design/madao-space/) |
| 码道 Work 小程序设计 Demo | Work | [打开](https://vinniechenyu.github.io/codearts-ide-design/madao-work-miniprogram/) |
| 码道 Work · 交互原型 | Work | [打开](https://vinniechenyu.github.io/codearts-ide-design/codearts-space/project.html?v=0817a) |
| CodeArts ADE 工作台交互原型 | ADE | [打开](https://vinniechenyu.github.io/codearts-ide-design/codearts-ade-prototype/) |
| Agent Space · IDE 内的智能体协同 | Space | [打开](https://vinniechenyu.github.io/codearts-ide-design/agent-space-prototype/) |
| AI 时代的开发者工具 · CLI 设计方案 | CLI | [打开](https://vinniechenyu.github.io/codearts-ide-design/cli-design-proposal/) |

### 业界洞察 + 竞品分析

| 材料 | 产品形态 | 在线预览 |
|---|---|---|
| AI 办公智能体 · 业界洞察与竞品分析 | Work | [打开](https://vinniechenyu.github.io/codearts-ide-design/ai-office-agent-insight/) |
| 码道 Work · HTML 创作专家与产品体验设计专家 · 双专家方案 | Work | [打开](https://vinniechenyu.github.io/codearts-ide-design/madao-work-design-competitive/) |
| 拆透 ADE,重构 AI 时代的开发工作流 | ADE | [打开](https://vinniechenyu.github.io/codearts-ide-design/codearts-ade-vision/) |
| 当 IDE 遇见 Agent,体验如何被重新定义 | Space | [打开](https://vinniechenyu.github.io/codearts-ide-design/agentspace-insight/) |
| Agent Team 模式的 UX 解剖 | Space | [打开](https://vinniechenyu.github.io/codearts-ide-design/agent-team-analysis/) |
| AI CLI 设计分析与探索报告 | CLI | [打开](https://vinniechenyu.github.io/codearts-ide-design/cli-analysis-report/) |

### 专项分析

| 材料 | 产品形态 | 在线预览 |
|---|---|---|
| 码道 Work · 产品定位与功能 PRD | Work | [打开](https://vinniechenyu.github.io/codearts-ide-design/madao-work-prd/) |
| 码道 · 生成响应体验优化专项 | IDE | [打开](https://vinniechenyu.github.io/codearts-ide-design/madao-response-deck/?v=brief-0713-2) |

### 方法论 · 体验范式

| 材料 | 产品形态 | 在线预览 |
|---|---|---|
| 设计范式：任务驱动型 Agent 工作台 | Space | [打开](https://vinniechenyu.github.io/codearts-ide-design/agent-workbench-paradigm/) |

### 组件 · 规范

| 材料 | 产品形态 | 在线预览 |
|---|---|---|
| Agent 对话式交互指南 | 通用 | [打开](https://vinniechenyu.github.io/codearts-ide-design/ai-dialogflow-components/) |

## 本地预览

线上仓库提供可直接托管的静态 HTML、JavaScript、CSS 与资源。预览这些文件无需安装 Node.js 依赖，也无需先运行构建命令。

```bash
git clone https://github.com/Vinniechenyu/codearts-ide-design.git
cd codearts-ide-design
python3 -m http.server 8000
```

浏览器访问 [http://localhost:8000](http://localhost:8000)，从首页进入各材料。建议使用 HTTP 服务预览，确保相对资源路径与线上访问方式一致。

## 目录结构

```text
.
├── index.html                      # 材料画廊、分类、搜索与版本入口
├── assets/                         # 首页预览图与共享资源
├── codeagent-console/              # 研发用量驾驶舱
├── codeagent-desktop/              # Desktop 任务起点原型
├── madao-space/                    # Space 一站式工作台
├── codearts-space/                 # Work 多版本交互原型
├── madao-work-prd/                 # Work 产品定位与 PRD
├── madao-work-miniprogram/         # Work 小程序原型
├── madao-work-design-competitive/  # 双专家方案与竞品实证
├── madao-response-deck/            # 生成响应体验优化
├── codearts-ade-vision/            # ADE 洞察与设计主张
├── codearts-ade-prototype/         # ADE 工作台原型
├── agentspace-insight/            # IDE / Agent 产品横评
├── agent-team-analysis/           # Agent Team 体验分析
├── agent-workbench-paradigm/      # 任务驱动型工作台方法论
├── agent-space-prototype/         # IDE 内智能体协同原型
├── ai-office-agent-insight/       # 办公智能体横评
├── ai-dialogflow-components/      # 对话式交互指南
├── cli-analysis-report/           # AI CLI 分析
├── cli-design-proposal/           # CLI 设计方案
└── .github/workflows/static.yml   # GitHub Pages 发布工作流
```

## 首页配置

首页的数据与交互位于根 `index.html`：

| 配置 | 用途 |
|---|---|
| `ITEMS` | 材料标题、描述、类型、产品形态、状态、预览图、标签与链接 |
| `CATEGORIES` | 类型目录：专项分析、洞察、方法论、交互原型、组件规范 |
| `PRODUCTS` | 产品形态目录；Space 的 id 为 `AgentSpace`，Work 为 `CodeArts Work` |
| `STATUS` | 状态标记：`live` 可体验、`proto` 可交互、`concept` 概念探索、`doc` 可阅读 |
| `PINS` | 全站置顶卡片及顺序，使用材料的 `href` 匹配 |

搜索会匹配标题、描述、标签、类型名称与产品形态 id。主题跟随系统，手动切换后保存在浏览器的 `localStorage`。

### 添加或更新材料

1. 新建材料目录，放入入口 `index.html` 与所需资源；先通过本地服务检查页面。
2. 截取 16:9 预览图，建议 1440 × 810，放入 `assets/preview-xxx.png`。汇报 deck 的截图应隐藏演示浮层、导航与提示。
3. 在 `ITEMS` 中添加或更新 `title`、`cat`、`product`、`status`、`desc`、`preview`、`tags`、`href`。分类 id 需与 `CATEGORIES` / `PRODUCTS` 对应。
4. 有多个版本时添加 `versions` 数组，每项填写 `label`、`note`、`href`，用 `current: true` 标记默认版本；未指定时首页打开数组第一项。
5. 检查首页筛选、搜索、默认入口、各版本链接与预览图，并在 1440px 窗口下回看密集布局。
6. 同步 README 材料目录与数量，提交并推送到 `main`。

同一材料的并行 HTML 版本建议放在同一目录，共用相对资源路径。更新已有原型时，可同步更新入口链接中的版本参数（如 `?v=0817a`）。

### 调整置顶

直接修改 `PINS` 并提交，即可更新所有访客看到的置顶顺序。

也可通过 `?edit=<EDIT_KEY 的值>` 打开置顶编辑控件，在本地预览置顶、取消与排序，再点击「导出置顶配置」，将导出的 `PINS` 替换到源码并提交。编辑草稿仅保存在当前浏览器的 `localStorage`；该模式是前端配置辅助工具，不是服务端权限控制。

## 部署

[静态发布工作流](.github/workflows/static.yml) 在推送到 `main` 或手动触发 `workflow_dispatch` 时运行，将仓库内容整体上传并部署到 GitHub Pages，无应用构建步骤。

- 站点地址：[vinniechenyu.github.io/codearts-ide-design](https://vinniechenyu.github.io/codearts-ide-design/)
- 发布进度与结果：[GitHub Actions](https://github.com/Vinniechenyu/codearts-ide-design/actions/workflows/static.yml)

发布是否完成以 Actions 运行结果为准。
