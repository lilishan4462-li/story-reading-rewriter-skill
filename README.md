# 追剧式读书改写器

把难读书改写成追剧式知识小说的 AI 助手工作流。

这个仓库包含两个版本：

- **专业版 Skill**：面向 Codex、Claude Code、Cursor、WorkBuddy、ChatGPT Agent 等助手型工具。
- **轻量版 Lite**：面向豆包、DeepSeek、Kimi、通义、普通 ChatGPT 等大模型对话框。

它不提供模型、不提供云服务、不上传或解析用户书籍。它提供的是一套方法论、提示词、内容大纲规则、质量闸门和定向修复流程。

## 核心原则

不要把知识包进故事里。

让知识从人物冲突、选择、规则、代价和后果中长出来。

## 两个版本怎么选

| 版本 | 适合人群 | 使用环境 | 优点 | 限制 |
| --- | --- | --- | --- | --- |
| 专业版 Skill | 会使用 AI 助手、Agent、代码工作区的人 | Codex、Claude Code、Cursor、WorkBuddy、ChatGPT Agent | 能维护文件、规则、章节计划和修复记录，适合长期项目 | 需要会配置助手或项目规则 |
| 轻量版 Lite | 只会使用大模型聊天框的人 | 豆包、DeepSeek、Kimi、通义、普通 ChatGPT | 上传或粘贴单文件规则包即可开始 | 上下文和文件能力受平台限制，需要状态卡续写 |

## 快速开始：专业版

适合你已经在使用 Codex、Claude Code、Cursor、WorkBuddy 或 ChatGPT Agent。

1. 把 `professional/` 目录作为 Skill 或项目规则加入你的助手。
2. 让助手读取：
   - `professional/SKILL.md`
   - `professional/references/rewrite-rules.md`
3. 提供书籍目录和第一章正文。
4. 要求助手先建立内容大纲，不要直接写正文。
5. 先试写第一章，运行质量闸门，通过后再继续。

推荐启动语：

```text
请使用 story-reading-rewriter 专业版方法。
我会提供一本难读书的目录和正文。
请先判断正文材料，再建立内容大纲，不要直接开始写第一章。
```

## 快速开始：轻量版

适合你使用豆包、DeepSeek、Kimi、通义、普通 ChatGPT 等对话框。

1. 上传或粘贴 `lite/story-reading-rewriter-lite.md`。
2. 发送：

```text
请读取这个规则包。读完后，你来主持整本书的追剧式改写流程。
```

3. 按模型要求上传书籍、目录或第一章。
4. 要求它先建立内容大纲，再试写第一章。

Lite 版会要求模型每轮输出“项目状态卡”，方便断点续写和换平台继续。

## 目录结构

```text
story-reading-rewriter/
  README.md
  LICENSE
  professional/
    SKILL.md
    references/
      rewrite-rules.md
    agents/
      openai.yaml
    install-guides/
      README.md
      workbuddy.md
  lite/
    story-reading-rewriter-lite.md
    quick-start.md
    state-card-template.md
    platform-notes.md
  docs/
    version-differences.md
    usage-boundaries.md
```

## 适合改写什么书

- 哲学、历史、文学、心理学、商业、成长类难读书。
- 适合个人学习、读书会、内部训练、知识内容实验。
- 适合公版书、已授权材料、个人有权处理的文本。

## 不适合什么场景

- 想一键生成整本书且不做人工判断。
- 想跳过版权授权，把受版权保护书籍的整本改写版公开商业发布。
- 想让本项目处理 OCR、阅读器、支付、会员、云部署或模型调用。

## 版权提醒

请确保你有权处理输入文本。

本项目提供改写方法和工作流，不授予任何第三方书籍的改写、复制、发行或商业发布权利。

## 开源协议

本仓库代码和文档采用 MIT License。

