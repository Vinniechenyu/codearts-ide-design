# CodeArts IDE Design

CodeArts IDE / 码道代码智能体的体验设计材料集,统一托管。单色极简风格(参考 dousanmiao.com),左侧目录按类型浏览,支持搜索与深浅模式切换。

**在线访问:** https://vinniechenyu.github.io/codearts-ide-design/

## 材料

| 材料 | 分类 | 链接 |
|---|---|---|
| 码道 · 生成响应体验优化专项(40 页 deck) | 专项分析 | [`madao-response-deck/`](https://vinniechenyu.github.io/codearts-ide-design/madao-response-deck/) |
| 拆透 ADE,重构 AI 时代的开发工作流 | 业界洞察+竞品分析 | [`codearts-ade-vision/`](https://vinniechenyu.github.io/codearts-ide-design/codearts-ade-vision/) |
| 当 IDE 遇见 Agent,体验如何被重新定义(5 款横评) | 业界洞察+竞品分析 | [`agentspace-insight/`](https://vinniechenyu.github.io/codearts-ide-design/agentspace-insight/) |
| Agent Team 模式的 UX 解剖(3 款横评) | 业界洞察+竞品分析 | [`agent-team-analysis/`](https://vinniechenyu.github.io/codearts-ide-design/agent-team-analysis/) |
| Agent Space · IDE 内的智能体协同(高保真原型) | 交互原型 | [`agent-space-prototype/`](https://vinniechenyu.github.io/codearts-ide-design/agent-space-prototype/) |
| Agent 对话式交互指南(组件库) | 组件·规范 | [`ai-dialogflow-components/`](https://vinniechenyu.github.io/codearts-ide-design/ai-dialogflow-components/) |

## 分类目录

专项分析 · 业界洞察+竞品分析 · 交互原型 · 组件·规范(空分类会在目录占位,便于扩展)。

## 特性

- **深浅模式** — 跟随系统 `prefers-color-scheme`,手动切换后由 `localStorage` 记忆,刷新不闪烁
- **目录筛选 + 搜索** — 左侧分类筛选,右上搜索框按标题/描述/标签实时过滤
- **数据驱动** — 首页由 `index.html` 里的 `ITEMS` / `CATEGORIES` 数组渲染,加材料只改数据
- **纯静态单文件** — 无框架、无构建,GitHub Pages 直接托管

## 添加新材料

1. 新建文件夹(如 `xxx/`),放入自包含入口 `index.html` 与资源
2. 截一张 **16:9 预览图**(1440×810)放 `assets/preview-xxx.png`
   ```bash
   "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" \
     --headless=new --disable-gpu --hide-scrollbars \
     --window-size=1440,810 --force-device-scale-factor=1 \
     --screenshot=assets/preview-xxx.png --virtual-time-budget=3500 \
     "file://$PWD/xxx/index.html"
   ```
   > 演示型 deck(如 madao)需先注入 CSS 隐藏演示浮层(视图切换器/导航/提示)再截图,避免黑边/工具栏残留。
3. 在根 `index.html` 的 `ITEMS` 数组复制一个对象,填写:
   `cat`(分类 id)/ `title` / `status`(`live` 可体验 · `proto` 可交互 · `concept` 概念探索 · `doc` 可阅读)/ `desc` / `preview` / `tags` / `href`
4. 需要新分类 → 在 `CATEGORIES` 数组加一行(`id` / `label` / `ac` 强调色)
5. push,约 1 分钟后 GitHub Pages 自动更新
