# 岭南红艾 · 独立 GitHub Pages 发布

此仓库**只负责发布**岭南红艾静态交互原型，本仓库不是产品源码的第二真相源。

## 预览
https://sanchuang-dev.github.io/lingnan-red-mugwort-pages/

## 唯一产品源码

- 仓库：[sanchuang-dev/base-prototype](https://github.com/sanchuang-dev/base-prototype)
- 分支：`feat/lingnan-red-mugwort-prototype`
- 文件：`index.html`、`app.css`、`app.js`
- 本仓库通过 GitHub Actions 检出上述分支，从最新源码生成 Pages 静态产物，不存放另一份可编辑产品代码。

## 更新与部署

- [Pages 工作流](./.github/workflows/pages.yml)：首次提交 / 手动 `Run workflow` 立即发布。
- 每两小时自动重新读取原型分支并发布；无需跨仓库密钥。
- 源码需要立即对客查看时，在本仓库 Actions → Publish Lingnan Demo to GitHub Pages → Run workflow 手动触发。
- GitHub Pages 状态以 Actions 的 `deploy` job 成功以及网站实际 HTTP 响应为准。

## 业务隔离

- 本仓库无后端，无支付、订单、登录、客户资料提交；所有交互均为演示。
- 原社区健康演示仍由 `sanchuang-dev/base-prototype` 的 `main` 独立管理和发布，原有站点不变。
- 不向原仓库 `main` 合并原型，不修改其 `.github/workflows/pages.yml`。
- 此发布仓库的 `main` 是纯静态演示**发布配置分支**，不承载原型业务源代码；这是组织标准环境模型的文档化例外。
