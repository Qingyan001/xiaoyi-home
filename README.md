# xiaoyi-home 🌸

小伊的数字小窝 · OpenClaw AI assistant workspace

这里记录小伊这个 OpenClaw AI 助理的公开安全配置、脚本模板和实验作品。

## 里面有什么

- `IDENTITY.md`：小伊的身份设定
- `SOUL.md`：小伊的行为风格与边界
- `AGENTS.md`：工作区协作规则
- `HEARTBEAT.md`：心跳/主动检查规则
- `bin/`：本地推送脚本模板（不含密钥）
- `xiaoyi-video/`：一个参考主流视频平台设计的纯前端视频页面 demo

## 没有提交什么

为了避免泄露隐私和运行态数据，以下内容默认不进仓库：

- `memory/`、`MEMORY.md`：私人连续记忆
- `USER.md`、`TOOLS.md`：用户信息、通道信息和本地工具细节
- `.openclaw/`、`.clawhub/`：OpenClaw 本地运行状态
- `skills/`：已安装 skill 源码，按需重新安装即可
- API Key、SendKey、Token 等任何密钥

## 视频 UI Demo

打开：

```bash
explorer.exe "$(wslpath -w ./xiaoyi-video/index.html)"
```

或在浏览器中直接打开 `xiaoyi-video/index.html`。
