# 专业版安装指南

不同助手的具体安装方式不同，但核心思路相同：

1. 让助手能读取 `professional/SKILL.md`。
2. 让助手能读取 `professional/references/rewrite-rules.md`。
3. 把书籍材料、内容大纲、章节计划、成稿和修复记录放在同一个项目空间里。

## Codex

把 `professional/` 作为 Skill 目录或项目规则目录使用。

启动时要求 Codex 读取 `SKILL.md` 和 `references/rewrite-rules.md`。

## Claude Code

把专业版规则复制到项目的 Skill 或项目说明文件中。

要求 Claude Code 先建立内容大纲，再进入章节改写。

## Cursor

把专业版规则放进项目文档或规则文件。

建议单独维护：

- `content-outline.md`
- `chapter-plan.md`
- `repair-log.md`

## ChatGPT Agent

把专业版文件加入项目文件或长期上下文。

先跑小样，不要一次生成整本。

