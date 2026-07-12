# CodeArts IDE Design · 材料启动台

CodeArts IDE / 码道代码智能体相关的体验设计材料统一托管。

**在线启动台:** https://vinniechenyu.github.io/codearts-ide-design/

## 材料目录

| 材料 | 说明 | 链接 |
|---|---|---|
| `madao-response-deck/` | 码道·生成响应体验优化专项(40 页汇报 deck) | [在线预览](https://vinniechenyu.github.io/codearts-ide-design/madao-response-deck/) |

## 添加新材料

1. 新建一个文件夹(如 `xxx-prototype/`),放入自包含的入口 `index.html` 与其资源
2. 可选:截一张预览图放 `assets/preview-xxx.png`(16:9)
3. 在根 `index.html` 的 `ITEMS` 数组里复制一个对象,填 `title / group / status(live|proto|doc) / desc / preview / tags / actions.href`
4. push,约 1 分钟后启动台自动出现新卡片
