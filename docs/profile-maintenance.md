# Profile Maintenance

本文说明如何维护 `profile/README.md`。该文件会展示在 GitHub 组织首页，应保持简洁、稳定、可公开阅读。

## Profile README 应包含

- `President-Office` 的一句话定位。
- 重点仓库入口。
- 简短治理原则。
- 必要的命名或归属说明。

## Profile README 不应包含

- 过长的项目说明。
- 临时项目状态。
- 内部会议细节。
- 服务器、密钥、账号、客户隐私。
- 未确认的规划或猜测。

## 推荐结构

```md
# 总裁办 / Executive Office

一句话定位。

## Repository Map

重点仓库表格。

## Governance

核心边界和原则。
```

## 更新步骤

1. 先更新 `docs/repository-map.md`。
2. 再从仓库地图中挑选适合公开展示的重点内容。
3. 修改 `profile/README.md`。
4. 检查 GitHub 页面展示是否简洁。
5. 提交到 `main`。

## 表格字段建议

```md
| Repository | Visibility | Purpose |
|---|---:|---|
| `repo-name` | public/private | 一句话用途 |
```

## Last updated

Profile README 可以保留 `_Last updated: YYYY-MM-DD_`，但不要为了更新日期而频繁提交无意义变更。
