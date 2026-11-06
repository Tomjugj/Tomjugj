# 认知地图 Knowledge Atlas

一个不需要构建工具、无需账号的中文通识学习网站。涵盖哲学、历史、社会、艺术、科幻五个模块，共 25 个学习单元，以及跨学科概念地图、8 周阅读路线、精选外部资源链接。

## 使用

直接打开 `index.html`；也可以执行 `python3 -m http.server 8000` 并浏览 `http://localhost:8000`。

## 进度存储和隐私

进度通过浏览器 `localStorage` 保存，笔记不传往任何服务器。无跨设备自动同步；可在“学习进度”导出 JSON，再在另一设备导入。无账号系统、服务器数据库或分析脚本。清除浏览器站点数据会删除本地记录。

## GitHub Pages 发布

1. 创建一个**公开**仓库，例如 `knowledge-atlas`。
2. 把 `index.html`、`README.md` 上传到仓库根目录。
3. 在 GitHub `Settings → Pages → Build and deployment` 选择 `Deploy from a branch`、`main`、`/(root)` 并保存。
4. 等待 GitHub Pages 完成构建后访问 `https://<用户名>.github.io/knowledge-atlas/`；准确地址以 Pages 设置页为准。

**注意：**部署公开只意味着网站代码对所有人可见，不代表所有人的进度公开；进度仅留在访问者本机。

## 设计说明

- 无外部依赖；移动端适配；不使用外部字体、跟踪脚本。
- 内容为原创精炼导读，不包含版权书籍正文。
- 学科概念互相关联，但不把社会现象简单还原为物理公式。