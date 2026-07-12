# CodeArts IDE Design · 材料启动台

CodeArts IDE / 码道代码智能体相关的体验设计材料统一托管。像素编辑风启动台,左侧目录按类型浏览。

**在线启动台:** https://vinniechenyu.github.io/codearts-ide-design/

## 材料

| 材料 | 分类 | 链接 |
|---|---|---|
| 码道·生成响应体验优化专项(40 页 deck) | 系统化专项分析 | [`madao-response-deck/`](https://vinniechenyu.github.io/codearts-ide-design/madao-response-deck/) |
| CodeArts ADE·拆透 ADE,重构工作流 | 概念方案探索 | [`codearts-ade-vision/`](https://vinniechenyu.github.io/codearts-ide-design/codearts-ade-vision/) |

## 分类目录

系统化专项分析 · 概念方案探索 · 产品交互原型 · 竞品分析 · 设计文档/规范(空分类会在目录占位,便于扩展)。

## 添加新材料

1. 新建文件夹(如 `xxx/`),放入自包含入口 `index.html` 与资源
2. 截一张 16:9 预览图放 `assets/preview-xxx.png`
3. 在根 `index.html` 的 `ITEMS` 数组复制一个对象:填 `cat`(分类 id)/ `title` / `status`(live·proto·concept·doc)/ `desc` / `preview` / `tags` / `href` / `accent`(purple·amber·green·teal·pink)
4. 需要新分类 → 在 `CATEGORIES` 数组加一行
5. push,约 1 分钟后启动台自动更新
