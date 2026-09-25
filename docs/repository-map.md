# Repository Map

本文记录 `President-Office` 组织下仓库的用途和边界。组织首页 `profile/README.md` 只保留精简入口；详细说明以本文为准。

## 当前公开可见仓库

| Repository | Purpose | Notes |
| --- | --- | --- |
| `.github` | 组织 profile、仓库地图和轻量治理说明 | 本仓库 |
| `knowledge-skill-library` | 项目对比知识、技术选型、业务理解和可复用 skills | 适合直接维护 `main` |
| `project-time-management` | 个人项目时间管理 dashboard | 主业/副业共用视图但逻辑分离 |

## 当前私有仓库

以下仓库可能是私有仓库或后续需要补齐的总裁办资产：

| Repository | Purpose | Boundary |
| --- | --- | --- |
| `requirements` | 集团级 / 跨 BU 需求池 | 不替代具体业务仓库 Issue |
| `portfolio-management` | 项目组合管理、BU 项目地图、repo/domain/deploy 映射 | 不保存具体业务代码 |
| `meetings-and-decisions` | 会议纪要、决策日志、经营 ADR | 不保存聊天流水账 |
| `policies` | GitHub、Issue/PR、Actions、部署、数据资产、AI Agent 协作规范 | 不保存密钥 |
| `ai-project-operating-system` | GitHub-first 的 AI 项目执行流程、模板、Specs、ADR、Harness 和 Agent 工作流 | 不替代公司级制度 |
| `operating-system` | 总裁办经营操作系统 | 不替代业务执行仓库 |

## 归属判断

### 留在 President-Office

- 战略、组合、制度、治理机制。
- 跨 BU 协作规则。
- 总裁办会议决策。
- 公共知识、通用方法、AI 项目操作体系。

### 下放到 Business-Unit-for-*

- 具体业务代码。
- 具体业务部署。
- 具体业务数据资产。
- 业务专属知识库和 skills。
- 业务自身需求、Issue、PR 和运行状态。

### 放到 Business-Unit-for-Platform

- 平台底座。
- clone-bot / codegen-bot。
- 通用脚手架。
- 可复用工程基础设施。`r`n- 跨业务可复用的行业监测公共组件，例如`r`n  `Business-Unit-for-Platform/industry-monitor-core`。`r`n`r`n`President-Office/industry-monitor-core` 已于 2026-09-25 归档，`r`n仅作为历史镜像保留；后续以平台组织仓库为唯一维护入口。

## 更新流程

1. 查询 GitHub 当前仓库列表。
2. 判断新增或变化仓库的归属。
3. 更新本文和 `BOOTSTRAP.md` 中受影响的入口。
4. 必要时同步更新 `profile/README.md`。
5. 提交到 `main`。
