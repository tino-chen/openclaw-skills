# OpenClaw Skills

Tino Chen 的 OpenClaw 技能集合，均为实际使用并验证过的技能。

## 技能列表

### 📝 note-taking — 笔记创建与管理规范

结构化知识库的笔记编写规范，确保笔记层级清晰、命名统一、格式一致。

- 笔记层级：一级导航（英文 kebab-case）→ 二级分组 → 笔记文档
- 语言规范：导航/分组用英文，笔记内容用中文
- 三种文档类型：知识（knowledge）、教程（guide）、经验（experience）
- 通用模板：含 type、title、tags 的 YAML front matter
- 适配 VitePress 构建，支持 GitHub Pages 部署
- ClawHub：`note-taking`

详细使用方法见 [note-taking/SKILL.md](note-taking/SKILL.md)

### 📐 workflow-note — 流程构建笔记写作规范

为 workflows/ 分类撰写笔记时的专用写作模板，定义文章结构、内容要求和质量标准。

- 定位：记录「用 AI 搭建自动化流程的完整经验」，区别于 tools/（工具推荐）
- 文章结构：开头直击痛点 → 最终效果可感知 → 架构图 → 分步实操 → 踩坑记录
- 实操步骤必须从实际配置文件读取完整内容，不能简略描述
- 与 note-taking 分层协作：note-taking 管全局规范，workflow-note 管分类模板
- ClawHub：`workflow-note`

详细使用方法见 [workflow-note/SKILL.md](workflow-note/SKILL.md)

### 📰 daily-ai-briefing — 每日 AI 硬核进展简报

每天自动检索全球 AI 领域的重大研究、开源热点和行业动态，生成高质量中文简报并推送到飞书。

- 7 条一票否决红线规则确保质量（14 天时效、来源白名单、四要素校验等）
- 跨天去重机制，避免同一事件重复出现
- 重点关注信息源 + 多源交叉搜索策略
- 配合 OpenClaw Cron 实现全自动运行
- ClawHub：`daily-ai-briefing`

详细使用方法见 [daily-ai-briefing/SKILL.md](daily-ai-briefing/SKILL.md)

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
openclaw skills install note-taking
openclaw skills install workflow-note
openclaw skills install daily-ai-briefing
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
