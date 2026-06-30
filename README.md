# President-Office .github

本仓库用于维护 `President-Office` 组织在 GitHub 上的公开门面、仓库导航和基础治理说明。

它是一个轻量文档仓库，不承载业务代码，也不记录具体项目进度。它的作用是让人和 AI Agent 进入 `President-Office` 后，能快速知道：

- 这个组织负责什么。
- 哪些仓库分别放什么。
- 新仓库应该如何命名和归类。
- 哪些内容应该留在 President-Office，哪些应该下放到各业务 BU。
- 维护组织 profile README 时应遵守哪些规则。

## 仓库结构

```text
.github/
├── README.md                     # 本仓库说明，面向维护者
├── AGENTS.md                     # AI Agent 操作规则
├── profile/
│   └── README.md                 # GitHub 组织首页展示内容
└── docs/
    ├── repository-map.md         # President-Office 仓库地图
    ├── repository-standards.md   # 仓库命名、归属和维护规则
    └── profile-maintenance.md    # 组织首页维护说明
```

## 当前定位

`President-Office` 是总裁办 / Executive Office 组织，主要承载：

- 集团战略和经营节奏。
- 项目组合管理。
- 制度、流程和治理规则。
- 会议决策和跨 BU 协调。
- 跨业务可复用的知识、方法和项目操作体系。

具体业务代码、部署、数据资产、业务专属知识，原则上应放在对应 `Business-Unit-for-*` 组织中。

## 快速入口

- 组织首页：`profile/README.md`
- 仓库地图：`docs/repository-map.md`
- 仓库标准：`docs/repository-standards.md`
- Profile 维护规则：`docs/profile-maintenance.md`
- Agent 规则：`AGENTS.md`

## 维护原则

1. **README 只做入口**：根 README 说明本仓库做什么，不堆所有细节。
2. **Profile 面向外部读者**：`profile/README.md` 应简洁、可读、稳定。
3. **细节进入 docs**：仓库地图、命名规则、维护流程进入 `docs/`。
4. **项目状态不放这里**：具体项目进度、Issue、PR、部署状态放回对应仓库。
5. **敏感信息不入库**：不记录 token、密码、服务器凭据、客户隐私和未授权数据。
6. **小型文档仓库直接维护 main**：简单 README/docs 更新可直接提交到 `main`，避免积累无意义分支。

## 适合作为其他 README-only 仓库的样板

如果某个仓库现在只有 README，可以先按这个最小结构补齐：

```text
<repo>/
├── README.md       # 这个仓库是什么、给谁看、怎么用
├── AGENTS.md       # AI Agent 进入仓库后的操作规则
└── docs/
    ├── overview.md # 背景、边界、核心对象
    └── workflow.md # 维护流程或使用流程
```

如果仓库继续增长，再增加：

```text
docs/decisions/     # ADR / 决策记录
docs/templates/     # 模板
docs/specs/         # 长期规则
```
