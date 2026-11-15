# 樱花 JSON 个人主页

一个樱花风格的个人主页，主站与 JSON 编辑器分开存放，数据由 `site/index.json` 驱动，主题由 `site/themes.json` 独立配置。

- 主站：展示个人介绍、项目卡片，支持主题切换与手动拉取刷新
- 编辑器：可在线编辑 `index.json` 和 `themes.json`，支持导入、校验、导出、复制
- 兼容旧数据：旧版 `index.json` 里的 `theme` 字段仍可作为主题回退来源

## 在线预览

- 主站：`https://nihao123bxy.github.io/sakura-json-homepage/site/`
- 编辑器：`https://nihao123bxy.github.io/sakura-json-homepage/admin/admin.html`

> 把上面的用户名和仓库名换成你自己的即可。

## 目录结构

```text
sakura-json-homepage/
├── README.md
├── LICENSE
├── LICENSE-CONTENT
├── .gitignore
├── site/
│   ├── index.html      # 主站，支持主题切换
│   ├── index.json      # 站点数据
│   └── themes.json     # 主题配置
└── admin/
    └── admin.html      # 编辑器，可编辑两个 JSON