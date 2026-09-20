# President-Office Bootstrap

这是 `President-Office` 组织级的最小启动上下文。任何 Agent、开发者或自动化流程进入组织后，先读取本文件，再读取目标仓库自己的 `README.md`、`AGENTS.md`、`docs/`、Issues、PRs 和 CI 状态。

## 组织级判断

AI 让软件实现、重构、测试和文档沉淀的成本显著下降，但这不会自动带来更好的软件。人在时间压力、人员变化和局部目标下，容易逐步放弃边界、验证、最小权限和设计纪律。

因此，`President-Office` 把软件工程思想写成机器可读的规则、工作流和验证门槛：

```text
用户意图
  -> GitHub 事实源
  -> 明确的工程原则
  -> 可执行的工作流
  -> 测试 / 度量 / Review
  -> 可回读的结果
```

原则不是口号。每次需求、设计、编码、审查和部署，都应能指出相关原则、验证方式和剩余风险。

## 进入组织后的读取顺序

1. 读取本仓库的 [`README.md`](README.md)、[`AGENTS.md`](AGENTS.md) 和 [仓库地图](docs/repository-map.md)。
2. 读取制度层的 `President-Office/policies`，确认组织、安全、权限、部署和数据边界。
3. 读取执行层的 `President-Office/ai-project-operating-system`，确认需求、开发、测试、Review 和回写流程。
4. 读取目标仓库自己的 `README.md`、`AGENTS.md`、架构文档、Issues、PRs 和 CI。
5. 如果事实冲突，先记录冲突和依据，不凭记忆或猜测继续修改。

## 编程时的默认原则

完整知识卡位于 [`knowledge-skill-library/07-foundations/design-principles`](https://github.com/President-Office/knowledge-skill-library/tree/main/07-foundations/design-principles)。编码和 Review 时至少检查：

| 原则 | 需要追问的问题 |
| --- | --- |
| SOLID / SRP | 这个模块是否有清楚的主要职责和变化原因？ |
| Open/Closed | 新能力是否可以进入明确的扩展点，而不是反复侵入稳定核心？ |
| Dependency Inversion | 核心业务是否依赖稳定抽象，而不是数据库、SDK 或部署细节？ |
| Composition | 能否组合小能力，而不是继续加深继承树或上帝对象？ |
| Separation of Concerns | 业务、数据、展示、权限和基础设施是否越过了不该越过的边界？ |
| DRY | 是否存在多份会分叉的业务知识或规则？ |
| KISS | 是否存在没有必要的层、依赖、状态或运行时组件？ |
| YAGNI | 这项能力是否由真实需求和验收标准证明现在需要？ |
| Fail Fast | 输入、配置、权限和外部依赖是否在错误扩散前被验证？ |
| Measure First | 优化或重构是否有基线、指标和可重复证据？ |
| Least Privilege | 人、Agent、CI、服务和 Token 是否只拥有当前任务所需权限？ |

这些原则需要结合上下文使用，不能机械套用。过度抽象、过度拆分和无证据优化同样是工程退化。

## 归属和写回

- 组织战略、制度、组合、决策和跨 BU 规则写入 `President-Office` 对应仓库。
- AI 项目执行流程、模板、检查清单和 Agent 工作流写入 `ai-project-operating-system`。
- 通用工程知识和可迁移的原则说明写入 `knowledge-skill-library`。
- 具体业务事实、代码、部署、数据和验收结果写入对应 `Business-Unit-for-*` 仓库。
- 稳定结论要回写 GitHub；聊天上下文、临时猜测和未经验证的状态不能充当事实源。

## 最小交付门槛

- 先读事实，再修改。
- 小步修改，避免无关重构。
- 代码或配置变更必须有实际验证结果。
- 影响安全、权限、数据、部署或生产的动作要缩小权限并明确风险。
- 文档写入后回读远端内容，确认链接、边界和事实没有漂移。
