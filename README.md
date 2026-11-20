# 一键破甲 · Jailbreak

**一句话：把你电脑上 20 个 AI 客户端「自己改不到的内置提示词」，换成你自己写的那份。**

| 换完之后 | 说明 |
|---|---|
| 用**你的**身份设定 | 而不是软件自带的默认人格 |
| **20 个客户端一份口径** | 共用一份人格文本，不用各改各的 |
| **当场能自证** | 发一句固定口令验证真载入，不靠「感觉好像生效了」 |
| **随时能还原** | 一键回官方原版，改前备份一直都在 |

## 支持的目标（20 个）

| 目标 | 落点 |
|---|---|
| `dsh` | DeepSeek Harness：Desktop / npm 全局 / npx 缓存 / 便携版 |
| `wb` / `wbintl` | WorkBuddy 国内版 / 国际版（模板 + 账号级云记忆） |
| `zcode` | ZCode：`AGENTS.md` / Memory / 技能 / 可选 cjs 系统提示词 |
| `codex` | Codex CLI：`config.toml` 的 `model_instructions_file` |
| `cursor` | Cursor：`.cursor/rules/*.mdc` |
| `claude` | Claude Code：`CLAUDE.md` |
| `antigravity` | Antigravity：CLI `agy` / IDE / 桌面端，共用 `~/.gemini` |
| `qwen` | Qwen Code：`~/.qwen/QWEN.md` |
| `iflow` | iFlow CLI：`~/.iflow/IFLOW.md` |
| `trae` / `traecn` | Trae / Trae CN：`~/.trae`、`~/.trae-cn`，两者分开认 |
| `codebuddy` | CodeBuddy：`~/.codebuddy/CODEBUDDY.md` |
| `opencode` | OpenCode：`~/.config/opencode/AGENTS.md` |
| `windsurf` | Windsurf：`memories/global_rules.md` |
| `cline` | Cline：`~/Documents/Cline/Rules/jailbreak-inject.md` |
| `copilot` | Copilot CLI：`~/.copilot/copilot-instructions.md` |
| `kiro` | Kiro：`~/.kiro/steering/jailbreak-inject.md` |
| `reasonix` | Reasonix Studio：`%APPDATA%\reasonix/AGENTS.md` |
| `qodercn` | Qoder CN：`~/.qoder-cn/agents/jailbreak/`，附 `skills/jailbreak/SKILL.md` |

## 自证

在客户端**新会话**里单独发一句 `破甲自检`（整条消息只有这四个字），只回一行就说明人格真载入了：

```
破甲已生效
```

回了解释、加戏或拒答 → 没生效。改的是磁盘文件，运行中的进程不会重读，**先确认目标已重启**。
