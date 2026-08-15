# CodeArts IDE Design

CodeArts IDE / 码道代码智能体的体验设计材料集，统一托管。单色极简风格，双维度目录（按类型 / 按产品形态），支持搜索、深浅模式与卡片置顶。

**在线访问：** https://vinniechenyu.github.io/codearts-ide-design/

> 所有材料均以 Vibe Design 方式产出：自包含单文件 HTML，无框架、无构建。

---

## 材料（15 份）

### 业界洞察 + 竞品分析

| 材料 | 产品 | 链接 |
|---|---|---|
| AI 办公智能体 · 业界洞察与竞品分析 | Work | [`ai-office-agent-insight/`](https://vinniechenyu.github.io/codearts-ide-design/ai-office-agent-insight/) |
| 码道 Work · HTML 创作专家与产品体验设计专家 · 双专家方案（54 页） | Work | [`madao-work-design-competitive/`](https://vinniechenyu.github.io/codearts-ide-design/madao-work-design-competitive/) |
| 拆透 ADE，重构 AI 时代的开发工作流 | ADE | [`codearts-ade-vision/`](https://vinniechenyu.github.io/codearts-ide-design/codearts-ade-vision/) |
| 当 IDE 遇见 Agent，体验如何被重新定义（5 款横评） | Space | [`agentspace-insight/`](https://vinniechenyu.github.io/codearts-ide-design/agentspace-insight/) |
| Agent Team 模式的 UX 解剖（3 款横评） | Space | [`agent-team-analysis/`](https://vinniechenyu.github.io/codearts-ide-design/agent-team-analysis/) |
| AI CLI 设计分析与探索报告 | CLI | [`cli-analysis-report/`](https://vinniechenyu.github.io/codearts-ide-design/cli-analysis-report/) |

### 专项分析

| 材料 | 产品 | 链接 |
|---|---|---|
| 码道 Work · 产品定位与功能 PRD | Work | [`madao-work-prd/`](https://vinniechenyu.github.io/codearts-ide-design/madao-work-prd/) |
| 码道 · 生成响应体验优化专项 | IDE | [`madao-response-deck/`](https://vinniechenyu.github.io/codearts-ide-design/madao-response-deck/) |

### 方法论 · 体验范式

| 材料 | 产品 | 链接 |
|---|---|---|
| 设计范式：任务驱动型 Agent 工作台 | Space | [`agent-workbench-paradigm/`](https://vinniechenyu.github.io/codearts-ide-design/agent-workbench-paradigm/) |

### 交互原型

| 材料 | 产品 | 链接 |
|---|---|---|
| 码道 Work 小程序设计 Demo | Work | [`madao-work-miniprogram/`](https://vinniechenyu.github.io/codearts-ide-design/madao-work-miniprogram/) |
| 码道 Work · 交互原型 | Work | [`codearts-space/`](https://vinniechenyu.github.io/codearts-ide-design/codearts-space/pet.html) |
| CodeArts ADE 工作台交互原型 | ADE | [`codearts-ade-prototype/`](https://vinniechenyu.github.io/codearts-ide-design/codearts-ade-prototype/) |
| Agent Space · IDE 内的智能体协同 | Space | [`agent-space-prototype/`](https://vinniechenyu.github.io/codearts-ide-design/agent-space-prototype/) |
| AI 时代的开发者工具 · CLI 设计方案 | CLI | [`cli-design-proposal/`](https://vinniechenyu.github.io/codearts-ide-design/cli-design-proposal/) |

### 组件 · 规范

| 材料 | 产品 | 链接 |
|---|---|---|
| Agent 对话式交互指南（组件库） | 通用 | [`ai-dialogflow-components/`](https://vinniechenyu.github.io/codearts-ide-design/ai-dialogflow-components/) |

---

## 目录维度

**按类型：** 专项分析 · 业界洞察+竞品分析 · 方法论·体验范式 · 交互原型 · 组件·规范
**按产品形态：** IDE · ADE · Space · Work · CLI · 通用·跨产品

**状态标记：** `live` 可体验 · `proto` 可交互 · `concept` 概念探索 · `doc` 可阅读

---

## 特性

- **双维度目录** — 左侧可按类型或产品形态切换筛选
- **深浅模式** — 跟随系统 `prefers-color-scheme`，手动切换后由 `localStorage` 记忆，刷新不闪烁
- **搜索** — 按标题 / 描述 / 标签实时过滤
- **卡片置顶** — 由 `index.html` 里的 `PINS` 数组控制，置顶卡排最前并带「📌 置顶」徽标
- **多版本材料** — 一份材料可挂多个版本，卡片 hover 出「版本管理」，`current:true` 的为默认打开项
- **数据驱动** — 首页由 `ITEMS` / `CATEGORIES` / `PRODUCTS` 数组渲染，加材料只改数据
- **纯静态** — 无框架、无构建，GitHub Actions 直接发布静态文件

---

## 添加新材料

1. 新建文件夹（如 `xxx/`），放入自包含入口 `index.html` 与资源
2. 截一张 **16:9 预览图**（1440×810）放 `assets/preview-xxx.png`

   ```bash
   "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" \
     --headless=new --disable-gpu --hide-scrollbars \
     --window-size=1440,810 --force-device-scale-factor=1 \
     --screenshot=assets/preview-xxx.png --virtual-time-budget=3500 \
     "file://$PWD/xxx/index.html"
   ```

   > 演示型 deck 需先注入 CSS 隐藏演示浮层（视图切换器 / 导航 / 提示）再截图，避免黑边与工具栏残留。

3. 在根 `index.html` 的 `ITEMS` 数组复制一个对象，填写：
   `cat`（类型 id）/ `product`（产品形态 id）/ `title` / `status` / `desc` / `preview` / `tags` / `href`
4. 需要新分类 → 在 `CATEGORIES` 或 `PRODUCTS` 数组加一行（`id` / `label` / `ac` 强调色）
5. push，GitHub Actions 自动发布

> **1440px 是画廊里的实际观看宽度**：材料拷进来后按这个宽度回看一遍（内容区约 1100px），一行多卡的密集布局容易挤爆或换行。

### 多版本材料

同一材料的并行版本**放在同一目录下**（如 `codearts-space/persona.html`），共用一份 `assets/`；不要建子文件夹，否则相对资源路径会断。在 `ITEMS` 里加 `versions` 数组，每项 `label` / `href`，默认打开项标 `current:true`。

> 更新已有 demo 时顺手 bump `href` 上的 cache-buster（如 `?v=0804a`），否则老访客拿到的是缓存。

---

## 部署

GitHub Actions 发布静态文件（`.github/workflows/static.yml`），push 到 `main` 后自动触发，秒级完成。

> 2026-08 之前用的是 Pages legacy(Jekyll) 构建。站点累积到 54MB / 155 文件后，Jekyll 遍历跑不完，构建连续在 10 分钟超时处失败（错误信息只有一句 `Page build failed.`，无诊断价值）。改用 Actions 后不再走 Jekyll，构建日志也可在 Actions 标签直接查看。

---

## 卡片置顶

`index.html` 里的 `const PINS = [href, ...]` 是线上唯一可信来源，所有访客可见。

带口令访问（口令即 `index.html` 里的 `EDIT_KEY` 常量）会出现隐藏编辑模式：置顶 / 取消 / 上移下移控件与底部工具条。编辑改动只存在 `localStorage` 里做本地预览；点「导出置顶配置」复制出新的 `PINS` 一行，替换 `index.html` 里那行并 push，才对所有人生效。
