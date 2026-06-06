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
```

## 明确未安装

```text
desktop-control
xiaohongshu-mcp
```

## 本地辅助工具

- `uv` / `uvx`：供 `markdown-converter` 通过 `uvx markitdown` 转换文档。
- `gh`：GitHub CLI，供 `github` skill 使用。当前安装在 `~/.local/bin/gh`；Git SSH 已可用，`gh` API 操作仍需 `gh auth login`。
