# 樱花 JSON 个人主页

一个樱花风格的个人主页，主站与 JSON 编辑器分开存放，数据由 `site/index.json` 驱动。

## 目录结构

```text
sakura-json-homepage/
├── README.md
├── LICENSE
├── LICENSE-CONTENT
├── .gitignore
├── site/
│   ├── index.html
│   └── index.json
└── admin/
    └── admin.html
```

功能

· 樱花飘落背景与开场过场动画
· 个人介绍卡：头像、简介、标签、链接
· 项目小卡片：标题、描述、图标、标签、超链接跳转
· 主站打开时读取一次 site/index.json
· 手动拉取刷新，不自动轮询
· 独立 JSON 编辑器，支持导入、从服务器载入、格式化、应用、导出、复制
· 响应式布局

快速开始

本地用任意静态服务器打开：

```bash
python -m http.server 8080
```

然后访问：

```text
主站：http://localhost:8080/site/
编辑器：http://localhost:8080/admin/admin.html
```

数据说明

主站读取 site/index.json。编辑器读取 ../site/index.json。
修改后请在编辑器点“导出”，用下载的 index.json 覆盖 site/index.json，再回主站点“手动拉取刷新”。

许可证

· 代码：MIT License，见 LICENSE
· 文档、文案、图片、JSON 示例内容：CC BY 4.0，见 LICENSE-CONTENT
