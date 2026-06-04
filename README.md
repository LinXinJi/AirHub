# 🌐 AirHub

> 林欣稷 (Air) 的个人数字空间、知识体系与项目实践管理中心。
> 融合物联网工程实践，探索事物所蕴含的“道”与“德”。

## 📂 站点目录 (Monorepo)

本仓库采用单体仓库架构，统一管理多个独立站点：

- 🏛️ **稷下学宫**：核心知识库 (Docs) 与项目实践 (Projects) 展示站。
- 📝 **Air.log**：个人博客，记录技术短文、学习心得与生活感悟。
- 📦 **future-site**：未来扩展站点的预留目录。 

```
AirHub/
├── .venv/                  # uv 创建的虚拟环境（建议在 .gitignore 中忽略）
├── pyproject.toml          # uv 的核心依赖配置文件（管理 zensical 等工具版本）
├── uv.lock                 # uv 的依赖锁定文件
├── .gitignore              # Git 忽略文件配置
├── README.md               # AirHub 总览说明
│
├── JiXia/                  # 🏛️ 站点 1：稷下学宫 (主站：知识体系 + 项目)
│   ├── config.toml         # 站点配置（title: "稷下学宫"）
│   ├── content/            # 核心内容目录
│   │   ├── index.md        # 首页
│   │   ├── about.md        # 关于 Air
│   │   ├── docs/           # 知识体系 (物联网、寻道问德等)
│   │   └── projects/       # AirHub 项目实践展示
│   └── static/             # 该站点专属的静态资源 (图片、自定义 CSS)
│
├── Blog/                   # 📝 站点 2：Air.log (个人博客)
│   ├── config.toml         # 站点配置（title: "Air.log"）
│   ├── content/
│   │   ├── index.md
│   │   └── posts/          # 按年份或分类存放博客文章 (如: 2026/06-xxx.md)
│   └── static/
│
└── future-site/            # 📦 站点 3：未来可能扩展的其他站点 (占位)
```

## ☯️ 设计理念

- Air (空气)：轻盈、无形，却孕育万物，连接一切（契合物联网与知识流动）。
- 稷下学宫：兼容并蓄，自由探索，是沉淀技术与思考“道与德”的数字殿堂。

## 🛠️ 开发经历

本项目使用 `uv` 进行依赖管理，`zensical` 作为静态站点生成器，`jj`、`git` 进行版本管理。