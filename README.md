# Backend-Solution-Design 后端解决方案设计 Skill

一个技能为你后端项目的 Bug 修复、新功能添加、旧功能修改/优化提供高质量解决方案。将后端 Bug 修复、新功能开发、旧功能修改与优化统一纳入一套结构化的解决方案方法论，通过“现象（发生了什么？）—机制（为什么会发生？）—契约（正确行为应该是什么？）—影响（修改会波及哪里？）—验证（如何证明方案正确？）”五步分析视角，以及“上游生产者 → 接入与转换 → 应用与领域逻辑 → 状态与副作用 → 下游消费者”的双向影响分析，帮助模型在编码前识别真实根因、领域不变量、外部契约、数据与状态流、事务边界和潜在回归风险；同时根据任务实际风险按需分析兼容、并发、幂等、重试、迁移、缓存、消息、安全、容量、可观测性与回滚，既避免只修表象、局部打补丁、重复维护业务事实和无价值优化，又不过度限制模型的判断空间，从而使 Codex、Claude Code 等 Agent 输出更完整、可实施、可验证且更符合后端工程实际的高质量解决方案。

Skill 名称：

```text
backend-solution-design
```

该 Skill 只读分析后端变更并输出解决方案，不实施代码、数据、配置、迁移、提交、部署或发布。

## Codex 项目级安装

在 Codex 输入下列内容：

```text
请检查并安装此链接（https://github.com/VenusFennn/Backend-Solution-Design）中的 backend-solution-design 技能为当前仓库的项目级 Codex Skill。
安装目标为 .agents/skills/backend-solution-design。

不要覆盖已有同名技能；如已存在，先比较并报告。
安装后验证 SKILL.md、全部中文参考文件和 SHA256SUMS，并确认可通过 $backend-solution-design 调用。
不要修改任何项目业务代码、数据或配置。
```

## Codex 用户级安装

在 Codex 输入下列内容：

```text
请把此链接（https://github.com/VenusFennn/Backend-Solution-Design）中的 backend-solution-design 技能安装为用户级 Codex Skill，
目标目录为 ~/.agents/skills/backend-solution-design。

安装前检查同名技能；如已存在，先比较并报告。
不要覆盖已有同名技能；
安装后验证完整性并确认可通过 $backend-solution-design 调用。
```

## Claude Code 项目级安装

在 Claude Code 输入下列内容：

```text
请检查并安装此链接（https://github.com/VenusFennn/Backend-Solution-Design）中的 backend-solution-design 技能为当前仓库的项目级 Claude Code Skill。
安装目标为 .claude/skills/backend-solution-design。

不要覆盖已有同名技能；如已存在，先比较并报告。
安装后验证 SKILL.md、全部中文参考文件和 SHA256SUMS，并确认可通过 /backend-solution-design 调用。
不要修改任何项目业务代码、数据或配置。
```

## Claude Code 用户级安装

在 Claude Code 输入下列内容：

```text
请将此链接（https://github.com/VenusFennn/Backend-Solution-Design）中的 backend-solution-design 技能安装为用户级 Claude Code Skill，
目标目录为 ~/.claude/skills/backend-solution-design。

不要覆盖已有同名技能；如已存在，先比较并报告。
安装后验证完整性并确认可通过 /backend-solution-design 调用。
```

## 完整性检查

安装前后应验证：

- `backend-solution-design/SKILL.md` 存在；
- `references/后端解决方案方法论.md` 存在；
- `references/后端风险与验证指南.md` 存在；
- `references/内容覆盖清单.md` 中所有章节均已勾选；
- `SHA256SUMS` 与实际文件一致；
- 没有覆盖未经确认的同名技能；
- 显式调用后只输出方案，不修改项目、数据、配置或外部系统状态。

## 升级

升级前先比较现有版本和新版本。不要直接覆盖用户自行修改的 Skill。确认差异后再替换完整技能目录，并重新执行哈希与调用验证。
