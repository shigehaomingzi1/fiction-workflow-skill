# Fiction Workflow Skill

一个用于 Codex 的小说写作工作流 skill。它把碎片文本、聊天记录、草稿或已有小说整理成结构化创作流程，并支持生成酒馆 AI / TavernAI / SillyTavern 角色卡。

## 功能概览

- 从原始文本中提取角色设定，并保留原文锚定证据。
- 支持扩写、续写、仅生成角色卡、扩写后续写、扩写后生成角色卡等分支。
- 提供风格与篇幅设定流程，包括叙事节奏、描写尺度、情感浓度、对白风格、环境描写权重和整体基调。
- 在续写前规划剧情走向、事件列表、优先级和填充模式。
- 生成结构文档、一致性校验清单、小说正文和角色卡 JSON。
- 附带风格示例参考文档。

## 仓库结构

```text
.
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    └── style-examples.md
```

## 安装方式

把本仓库复制到 Codex skills 目录中，例如：

```powershell
Copy-Item -Recurse . "$env:USERPROFILE\.codex\skills\fiction-workflow"
```

然后在 Codex 中使用：

```text
使用 fiction-workflow 根据我提供的文本素材写小说并生成角色卡。
```

## 注意事项

- 请不要把包含私人原文、API Key、账号密码或未脱敏聊天记录的内容提交到公开仓库。
- 本 skill 只包含工作流说明和参考模板，不包含模型调用代码或 API 密钥。
- 如果公开发布，请先确认其中的写作规则、示例和用途符合你希望公开展示的范围。

## License

尚未指定许可证。公开仓库如需允许他人复用，建议添加 MIT、Apache-2.0 或自定义许可证。
