# Skills

当前工作区曾安装/使用过的 OpenClaw skills 清单。

> 注意：仓库不提交 `skills/` 目录源码；需要时在本机按清单重新安装。

## 已安装

```bash
openclaw skills install auto-updater
openclaw skills install self-improving
openclaw skills install weather
openclaw skills install skill-creator
openclaw skills install n8n-workflow-automation
openclaw skills install prompt-engineering-expert
openclaw skills install markdown-converter
openclaw skills install word-docx
openclaw skills install excel-xlsx
openclaw skills install superdesign
openclaw skills install github
openclaw skills install git:https://github.com/wechat-miniprogram/ai-mode-skills.git/wxa-skills-generate --as wxa-skills-generate
# The following two skills contain CLI/dynamic execution code and may be blocked by OpenClaw's installer safety scan.
# In this workspace they were installed by copying the checked repo subdirectories into skills/ after manual inspection:
#   /tmp/ai-mode-skills/wxa-skills-validate -> skills/wxa-skills-validate
#   /tmp/ai-mode-skills/wxa-skills-eval -> skills/wxa-skills-eval
```

## 明确未安装

```text
desktop-control
xiaohongshu-mcp
```

## 本地辅助工具

- `uv` / `uvx`：供 `markdown-converter` 通过 `uvx markitdown` 转换文档。
- `gh`：GitHub CLI，供 `github` skill 使用。当前安装在 `~/.local/bin/gh`；Git SSH 已可用，`gh` API 操作仍需 `gh auth login`。

## WeChat Mini Program AI Mode Skills

来源：<https://github.com/wechat-miniprogram/ai-mode-skills>

- `wxa-skills-generate`：生成小程序 AI 原子接口/原子组件技能分包。
- `wxa-skills-validate`：校验和修复小程序 AI skills 产物；含 `child_process` 调微信开发者工具 CLI，安装器安全扫描会拦截。
- `wxa-skills-eval`：端到端评测小程序 AI skill；含动态执行/Node 工程，安装器安全扫描会拦截。
