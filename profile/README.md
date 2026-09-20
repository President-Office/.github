# 总裁办 / Executive Office

集团战略、经营节奏、项目组合、制度、会议决策与跨 BU 协同。

`President-Office` 用于承载集团层面的战略、治理、项目组合和跨业务协作资产；具体业务代码、部署和数据资产原则上归属对应 `Business-Unit-for-*`。

## Key Repositories

| Repository | Purpose |
|---|---|
| [`knowledge-skill-library`](https://github.com/President-Office/knowledge-skill-library) | 项目对比知识、技术选型、业务理解和可复用 skills |
| [`project-time-management`](https://github.com/President-Office/project-time-management) | 个人项目时间管理 dashboard |
| [`.github`](https://github.com/President-Office/.github) | 组织 profile、仓库地图和轻量治理说明 |

更多仓库说明见：[`docs/repository-map.md`](https://github.com/President-Office/.github/blob/main/docs/repository-map.md)。

## Governance

- 总裁办负责战略、组合、制度、会议决策和跨 BU 协调。
- 编程和 Review 遵守可验证的工程原则，知识卡见 [`knowledge-skill-library/07-foundations`](https://github.com/President-Office/knowledge-skill-library/tree/main/07-foundations)。
- 具体业务代码、部署和数据资产留在对应 BU。
- 平台底座、clone-bot、codegen-bot 等归 `Business-Unit-for-Platform`。
- 简单知识库 / README-only 仓库可以直接维护 `main`；代码、部署、CI、架构性变更优先走 PR。
- 不在 GitHub 仓库中保存 token、密码、服务器凭据、客户隐私和未授权数据。

---

_Last updated: 2026-09-20_
