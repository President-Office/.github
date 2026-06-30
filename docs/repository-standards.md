# Repository Standards

本文记录 `President-Office` 组织下仓库的命名、用途和维护规则。

## 命名原则

仓库名应清楚表达用途，避免过泛。

推荐：

```text
knowledge-skill-library
project-time-management
portfolio-management
meetings-and-decisions
policies
requirements
operating-system
```

避免：

```text
misc
new-project
test
readme
all-docs
```

## README-only 仓库最小结构

如果仓库目前只有 README，建议至少补齐：

```text
<repo>/
├── README.md
├── AGENTS.md
└── docs/
    ├── overview.md
    └── workflow.md
```

各文件职责：

- `README.md`：说明这个仓库是什么、给谁看、怎么用。
- `AGENTS.md`：说明 AI Agent 进入仓库后应如何读取、修改、验证。
- `docs/overview.md`：放背景、边界、核心对象。
- `docs/workflow.md`：放维护流程或使用流程。

如果仓库只是非常轻量的组织门面，`docs/overview.md` 和 `docs/workflow.md` 可以换成更具体的文档，例如本仓库的 `repository-map.md` 和 `profile-maintenance.md`。

## 什么时候继续扩展结构

当仓库出现以下情况时，再增加目录：

```text
docs/specs/         # 长期规则
docs/decisions/     # ADR / 决策记录
docs/templates/     # 模板
docs/assets/        # 非敏感图片、示意图或公开附件
```

不要一开始为所有仓库创建复杂目录。先用最小结构跑通，再按需要扩展。

## 分支规则

- 小型知识库、profile 仓库、README/docs 更新：可以直接维护 `main`。
- 代码、部署、CI、架构性变更：优先走分支和 PR。
- 不要为简单文档修改积累一堆长期分支。

## 安全规则

不得提交：

- token、密码、SSH key。
- 服务器登录信息。
- 客户隐私。
- 未授权数据。
- 生产环境 secret 值。

## AI Agent 规则

Agent 修改仓库前应先判断：

1. 这是总裁办仓库、平台仓库，还是业务 BU 仓库？
2. 当前修改应直接进 `main`，还是需要 PR？
3. 是否会影响公开展示？
4. 是否包含敏感信息？
5. 是否需要同步更新仓库地图或 profile README？
