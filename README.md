# 职业牌阵 · AI 作品起步器(翻牌测评)

一个面向求职学生的**单文件、零依赖**网页测评工具:答题 → 翻牌 → 生成一条「作品方向选择报告」AI 指令,帮学生**锚定一个对口的、可交互的作品方向**。

- 入口文件:`index.html`(双击即可本地运行)
- 无后端、无数据库;只引用 Google Fonts 与 html2canvas 两个 CDN
- 结果不调用任何外部 API:工具生成一段「VIBE CODING 指令」,由学生粘贴到自己的 AI(建议用**联网版** ChatGPT / 豆包)生成报告

## 部署

**GitHub Pages**:Settings → Pages → Source 选 `main` 分支根目录,几分钟后即可通过 `https://<用户名>.github.io/<仓库名>/` 访问。

**Vercel / Netlify**:直接导入仓库,Framework 选 “Other / 静态”,根目录即可。

## 关于 API key（重要）

本仓库**不包含任何 API key**。  
如果以后想让工具内直接调用大模型(而不是让学生复制指令),**不要把 key 写进前端**——它在公开站点上等于明文公开,会被盗刷。正确做法是用 Vercel/Netlify 的 Serverless Function 做代理,把 key 放在服务端环境变量里。

---
🤖 Generated with [Claude Code](https://claude.com/claude-code)
