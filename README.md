# OpenClaw Skills

Ty Chen 的 OpenClaw 技能集合，均为实际协作中使用并验证过的技能。

## 技能列表

### 📰 daily-ai-briefing — 每日 AI 硬核进展简报

每天自动检索全球 AI 领域的重大研究、开源热点和行业动态，生成高质量简报并推送到飞书。

- 7 条红线规则确保质量（一票否决）
- 跨天去重、来源白名单、四要素校验
- 配合 OpenClaw Cron 实现全自动运行

详细使用方法见 [daily-ai-briefing/SKILL.md](daily-ai-briefing/SKILL.md)

### 📝 note-taking — 笔记创建与管理规范

结构化知识库的笔记编写规范，包含层级结构、语言规范、命名规则和通用模板。

详细使用方法见 [note-taking/SKILL.md](note-taking/SKILL.md)

## 安装

### 通过 ClawHub（推荐）

```bash
openclaw skills install daily-ai-briefing
openclaw skills install note-taking
```

### 手动安装

```bash
git clone https://github.com/tino-chen/openclaw-skills.git
cp -r openclaw-skills/<skill-name> ~/.openclaw/skills/
```

## 相关

- 📖 [实践笔记](https://tino-chen.github.io/notes/) — 技能的使用经验和最佳实践
- 🤖 [OpenClaw](https://github.com/openclaw/openclaw) — AI Agent 框架
