# OpenClaw Skills

Tino Chen 的 OpenClaw 技能集合，均为实际使用并验证过的技能。

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

### 🔍 debunk — 事实核查与辟谣

对公众号/社交媒体链接、图片、视频等内容进行事实核查，输出结构化分析报告和多种风格的回复话术。

- 两种场景：自查型（纯查证）和社交回复型（查证 + 回复）
- 可信度评级：☆☆☆☆☆ ~ ⭐⭐⭐⭐⭐ 六级标尺
- 四种回复风格：直言不讳 / 高级情商 / 阿谀奉承 / 敷衍了事
- 内置 Playwright 脚本，可抓取公众号反爬内容
- ClawHub：`debunk`

详细使用方法见 [debunk/SKILL.md](debunk/SKILL.md)

## 安装

### 通过 ClawHub（推荐）

```bash
openclaw skills install daily-ai-briefing
openclaw skills install note-taking
openclaw skills install debunk
```

### 手动安装

```bash
git clone https://github.com/tino-chen/openclaw-skills.git
cp -r openclaw-skills/<skill-name> ~/.openclaw/skills/
```

## 相关

- 📖 [实践笔记](https://tino-chen.github.io/notes/) — 技能的使用经验和最佳实践
- 🤖 [OpenClaw](https://github.com/openclaw/openclaw) — AI Agent 框架
