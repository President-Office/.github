# Agent Instructions

本仓库是 `President-Office` 组织的 GitHub profile / repository map 仓库。Agent 处理本仓库时必须遵守以下规则。

## 仓库定位

- 本仓库只维护组织门面、仓库导航和轻量治理说明。
- 不保存具体业务项目进度。
- 不保存生产部署细节、密钥、服务器凭据或客户隐私。
- 具体业务代码、部署、数据资产应归属对应 `Business-Unit-for-*`。
- 总裁办层面的战略、组合、制度、会议决策和跨 BU 规则归属 `President-Office`。

## Source of Truth

- 根 README：`README.md`
- 组织首页展示：`profile/README.md`
- 仓库地图：`docs/repository-map.md`
- 仓库标准：`docs/repository-standards.md`
- Profile 维护说明：`docs/profile-maintenance.md`

## 修改规则

1. 修改前先读取 `README.md`、`profile/README.md` 和相关 `docs/`。
2. Profile README 应保持简洁，只放组织定位、重点仓库入口和核心治理原则。
3. 长说明不要塞进 profile，放到 `docs/`。
4. 仓库地图更新时，应同步检查：仓库名称、可见性、用途、归属边界。
5. 不要凭记忆更新仓库列表；应以 GitHub 当前仓库状态或用户明确说明为准。
6. 简单文档更新可以直接提交到 `main`。
7. 不要为小型 README/docs 更新积累长期分支。

## 内容边界

应放在本仓库：

- `President-Office` 是什么。
- 组织首页展示内容。
- 总裁办仓库地图。
- 仓库命名、归属、导航和维护规则。

不应放在本仓库：

- 某个业务项目的详细需求。
- 某个项目的部署配置。
- 项目实时进度和临时任务。
- 业务代码。
- 敏感信息。

## 验证要求

修改后至少检查：

```bash
git status --short
git diff --check
```

并确认：

- `profile/README.md` 仍适合公开展示。
- 根 README 与 `docs/` 不冲突。
- 仓库地图没有明显过期或误导信息。
