# 总裁办 / Executive Office

集团战略、经营节奏、项目组合、制度、会议决策与跨 BU 协同。

## Repository Map

| Repository | Visibility | Purpose |
|---|---:|---|
| [`knowledge-skill-library`](https://github.com/President-Office/knowledge-skill-library) | public | Knowledge summary and reusable Skill library for project planning, research, and AI development context. |
| [`meetings-and-decisions`](https://github.com/President-Office/meetings-and-decisions) | private | 总裁办会议纪要、决策日志、经营 ADR 与跨 BU 协调记录 |
| [`operating-system`](https://github.com/President-Office/operating-system) | private | 总裁办经营操作系统：组织架构、治理机制、立项/退出机制、跨 BU 协作规则 |
| [`policies`](https://github.com/President-Office/policies) | private | 总裁办制度与流程：GitHub、Issue/PR/Actions、部署、数据资产、AI Agent 与协作规范 |
| [`portfolio-management`](https://github.com/President-Office/portfolio-management) | private | 总裁办项目组合管理：BU 项目地图、repo/domain/deploy 映射、优先级与状态 |
| [`project-time-management`](https://github.com/President-Office/project-time-management) | public | Personal project time management dashboard for PeterKZhao portfolio projects. |
| [`requirements`](https://github.com/President-Office/requirements) | private | 总裁办集团级需求池：跨 BU 经营管理、项目组合、制度流程、协同机制与集团级 AI 能力需求 |

## Governance

- 具体业务代码、部署和数据资产留在对应 BU。
- 跨 BU 的战略、组合、制度和决策进入 `President-Office`。
- 平台底座和代码生成资产进入 `Business-Unit-for-Platform`。
- 生产部署默认按多机模式设计，数据库/缓存不以 `127.0.0.1` 作为生产默认。

## Naming note

- 组织名当前可用。

---

_Last updated: 2026-06-29_
