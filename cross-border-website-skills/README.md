# OpenClaw-Astro-Website-Skills 🦞

> AI 自动建站技能包 | AI Website Builder Skills | 零代码建站 | No-Code Website Generator

[![OpenClaw](https://img.shields.io/badge/OpenClaw-Skills-blue)](https://openclaw.ai)
[![License](https://img.shields.io/badge/License-MIT-green)](../LICENSE)
[![中文](https://img.shields.io/badge/语言-中文-red)](README.md)

---

## 项目介绍 | Introduction

一套面向**零基础小白**的开源 **AI 建站**工具包：让 OpenClaw 这个 AI Agent 帮你**全自动生成网站**。

装上之后，你不用学 Astro，也不用懂静态网站生成（SSG）—— 跟 Agent 说一句「帮我建一个外贸网站」，它就会按 9 个技能的顺序，从品牌风格分析一路跑到页面合并，最后给你一个能直接上线的站点。

**无需编程，对话即可建站。** 适合这些场景：

- 🏢 **企业官网** —— 公司介绍、品牌展示
- 🛒 **B2B 网站** —— 产品目录、询盘系统
- 🌐 **独立站** —— 跨境电商、DTC 品牌站
- 📦 **产品展示站** —— 产品详情、规格参数
- 🏭 **工厂官网** —— 制造业、供应商展示
- 💼 **品牌官网** —— 品牌故事、形象展示
- 🛍️ **外贸网站** —— 多语言、海外市场

生成的站点是纯静态 HTML，部署方便、加载快、对搜索引擎友好。

---

## 核心优势 | Features

| 特性 | 说明 |
|-----|------|
| 🤖 **AI 全自动** | 对话式建站，无需写代码 |
| 🎨 **智能设计** | AI 分析风格，自动配色排版 |
| 🔍 **SEO 优化** | 自动生成关键词，搜索引擎友好 |
| 📱 **响应式** | 自适应 PC / 平板 / 手机 |
| ⚡ **高性能** | 基于 Astro，静态生成，秒开 |
| 🌍 **多语言** | 支持中英文等多语言网站 |
| 🔧 **可定制** | 开源可改，灵活扩展 |

---

## 适用人群 | Who is this for

- ✅ 不会写代码的 **创业者 / 老板**
- ✅ 需要快速建站的 **外贸 / 跨境从业者**
- ✅ 想降低建站成本的 **中小企业**
- ✅ 学习 AI 建站的 **产品经理 / 运营**
- ✅ 探索 AI Agent 的 **技术爱好者**

---

## 前置条件 | Prerequisites

- ✅ 已安装 OpenClaw（版本 ≥ 1.0）
- ✅ 系统支持：MacOS / Linux / Windows (WSL2)
- ✅ 基础终端操作能力（小白可参考「手动安装」流程）

---

## 快速安装 | Installation

### 方式 1：命令行安装（推荐）

```bash
# 1. 克隆本仓库
git clone https://github.com/jovian6661/AI-.git

# 2. 进入目录
cd AI-/跨境独立站

# 3. 解压技能包
unzip astro-website-skills.zip

# 4. 创建 OpenClaw 技能目录（若不存在）
mkdir -p ~/.openclaw/skills/

# 5. 复制所有技能文件到指定目录
cp -r astro-website-skills/* ~/.openclaw/skills/
```

### 方式 2：手动安装（小白友好）

1. 下载本仓库 `astro-website-skills.zip` 并解压
2. 找到解压后的 9 个技能文件夹（`01-dispatcher` ~ `09-html-merger`）
3. 将这 9 个文件夹复制到 OpenClaw 技能目录：
   - **Mac**：`/Users/你的用户名/.openclaw/skills/`
   - **Linux/WSL**：`/home/你的用户名/.openclaw/skills/`

4. 确认目录结构：

```
~/.openclaw/
└── skills/
    ├── 01-dispatcher/SKILL.md
    ├── 02-style-analyzer/SKILL.md
    ├── 03-seo-planner/SKILL.md
    ├── 04-architecture-planner/SKILL.md
    ├── 05-art-director/SKILL.md
    ├── 06-traffic-sales-planner/SKILL.md
    ├── 07-page-producer/SKILL.md
    ├── 08-quality-inspector/SKILL.md
    └── 09-html-merger/SKILL.md
```

---

## 生效技能 | Activate Skills

OpenClaw 会自动监听技能文件变化，若未生效可手动重启：

```bash
# 重启 OpenClaw Gateway
openclaw gateway restart
```

或在聊天工具中发送指令：

```
刷新技能        # 中文
refresh skills  # 英文
```

---

## 验证安装 | Verify Installation

执行以下命令，查看 9 个技能是否全部加载：

```bash
openclaw skills list
```

✅ **成功标识**：输出中包含以下 9 个技能（均显示 ✓）：

```
Available Skills:
✓ astro-website-dispatcher     🚀 网站建站总调度技能
✓ astro-style-analyzer         🎨 网站对标风格解析技能
✓ astro-seo-planner            🔍 网站SEO策划师技能
✓ astro-architecture-planner   📐 网站架构页面策划技能
✓ astro-art-director           🎭 网站美术大师技能
✓ astro-traffic-sales-planner  🚀 网站流量和AI销售策划技能
✓ astro-page-producer          💻 网站页面生产大师技能
✓ astro-quality-inspector      ✅ 网站页面质检技能
✓ astro-html-merger            📦 网站HTML文件交互合并大师技能
```

---

## 快速使用 | Quick Start

在已配置的聊天工具（飞书 / WhatsApp / Telegram / Discord / Slack 等）中，向 OpenClaw 发送指令即可启动建站流程：

### 场景示例

```
# 企业官网
我要建一个企业官网，公司叫"XX科技"，主营软件开发服务

# B2B 网站
我要建一个B2B产品网站，公司是做工业零配件的

# 外贸独立站
我要建一个外贸网站，公司叫"深圳光明LED"，主营LED灯带，目标市场是欧美

# 品牌官网
我要建一个品牌官网，展示我们的护肤品品牌故事和产品系列

# 工厂官网
我要建一个工厂官网，展示生产能力和产品目录
```

---

## 建站流程 | Workflow

OpenClaw 会自动完成以下步骤（全程 20-30 分钟，只需回答问题）：

| 步骤 | 说明 |
|-----|------|
| 1️⃣ 需求收集 | 询问公司 / 产品 / 设计偏好 |
| 2️⃣ 风格解析 | 对标参考网站生成设计风格 |
| 3️⃣ SEO 策划 | 输出 20+ 精准关键词 |
| 4️⃣ 架构规划 | 设计网站结构与页面模块 |
| 5️⃣ 美术设计 | 输出配色 / 字体 / 间距规范 |
| 6️⃣ 增值服务 | 可选 AI SEO 博客、AI 客服 |
| 7️⃣ 代码生成 | 输出各页面 HTML 代码 |
| 8️⃣ 质量检测 | 校验代码符合设计规范 |
| 9️⃣ 打包合并 | 生成完整可用的网站包 |

---

## 技能列表 | Skills List

| 技能名称 | 核心功能 |
|---------|---------|
| astro-website-dispatcher | 建站全流程总调度 |
| astro-style-analyzer | 参考网站风格解析 |
| astro-seo-planner | 网站 SEO 关键词策划 |
| astro-architecture-planner | 网站结构 / 页面模块设计 |
| astro-art-director | 配色 / 字体 / 间距等美术规范 |
| astro-traffic-sales-planner | 流量规划 + AI 销售功能策划 |
| astro-page-producer | 各页面 HTML 代码生成 |
| astro-quality-inspector | 代码 / 设计规范质检 |
| astro-html-merger | HTML 文件合并打包 |

---

## 常见问题 | FAQ

### Q1：技能安装后未生效？

1. 检查文件路径：`ls ~/.openclaw/skills/` 确认 9 个技能文件夹存在
2. 检查文件完整性：`ls ~/.openclaw/skills/01-dispatcher/` 确认包含 SKILL.md
3. 重启 Gateway：`openclaw gateway restart`

### Q2：OpenClaw 未按技能流程执行？

请在指令中明确指定技能：

```
我要建一个网站，请按照 astro-website-dispatcher 技能流程执行
```

### Q3：支持哪些 AI 模型？

全兼容 Claude / DeepSeek / Qwen / OpenAI / GPT-4 等 OpenClaw 支持的模型，技能逻辑通用。

### Q4：如何禁用某个技能？

编辑 `~/.openclaw/openclaw.json`，添加禁用配置：

```json
{
  "skills": {
    "entries": {
      "astro-website-dispatcher": {
        "enabled": false
      }
    }
  }
}
```

### Q5：生成的网站如何部署？

生成的是静态 HTML 文件，可部署到：
- Vercel（推荐，免费）
- Netlify（免费）
- GitHub Pages（免费）
- 阿里云 / 腾讯云 OSS
- 任意支持静态托管的服务器

---

## 技能加载优先级 | Priority

OpenClaw 按以下优先级加载技能（高→低）：

| 优先级 | 位置 | 说明 |
|-------|------|------|
| 最高 | `<workspace>/skills/` | 仅当前项目生效 |
| 中等 | `~/.openclaw/skills/` | 本技能包默认路径，全项目生效 |
| 最低 | 内置技能 | OpenClaw 原生自带技能 |

---

## 进阶配置 | Advanced Configuration

编辑 `~/.openclaw/openclaw.json` 自定义技能行为：

```json
{
  "skills": {
    "load": {
      "watch": true,
      "watchDebounceMs": 250
    },
    "entries": {
      "astro-website-dispatcher": {
        "enabled": true
      }
    }
  }
}
```

| 配置项 | 说明 |
|-------|------|
| `watch: true` | 自动监听技能文件变化 |
| `watchDebounceMs` | 监听延迟（毫秒） |
| `enabled` | 启用/禁用指定技能 |

---

## 文件清单 | Files

| 文件 | 说明 |
|-----|------|
| `astro-website-skills.zip` | Astro 建站技能包（9个技能） |
| `OpenClaw新手使用指南独立站.docx` | 详细安装使用教程 |
| `新手轻松建站！OpenClaw Astro 外贸技能包全流程教程` | 全流程图文教程 |

---

## 相关技术 | Tech Stack

- **OpenClaw** - AI Agent 框架
- **Astro** - 现代静态网站生成器
- **HTML5 / CSS3** - 网页标准
- **Tailwind CSS** - 原子化 CSS 框架
- **AI Models** - Claude / GPT-4 / DeepSeek / Qwen

---

## 贡献指南 | Contributing

本项目开源欢迎贡献！无论是修复 Bug、新增功能、优化文档，都可通过以下方式参与：

1. Fork 本仓库
2. 创建特性分支：`git checkout -b feature/YourFeature`
3. 提交修改：`git commit -m 'Add some feature'`
4. 推送分支：`git push origin feature/YourFeature`
5. 提交 Pull Request

---

## 许可证 | License

本项目基于 **MIT 许可证** 开源，详见 LICENSE 文件。

---

## 支持与反馈 | Support

- 📚 OpenClaw 官方文档：https://docs.openclaw.ai/zh-CN
- 📞 建站相关问题：关注微信公众号「博屿博科技」
- 🌐 海外支持：https://aiseo.buzz
- 🐛 Bug 反馈 / 功能建议：提交 GitHub Issue

---

## Star History

如果这个项目对你有帮助，请给一个 ⭐ Star！

---

<p align="center">
  Made with ❤️ for 创业者 & 中小企业 & OpenClaw 用户
</p>

---

## 相关搜索 | Related Keywords

`AI建站` `AI网站生成器` `AI Website Builder` `AI Website Generator` `智能建站` `自动建站` `一键建站` `零代码建站` `无代码建站` `No-Code Website` `Low-Code` `Astro` `静态网站` `Static Site Generator` `SSG` `企业官网` `B2B网站` `品牌官网` `产品展示站` `独立站` `跨境电商` `外贸网站` `DTC品牌站` `工厂官网` `OpenClaw` `OpenClaw Skills` `AI Agent` `Claude` `GPT-4` `DeepSeek` `Qwen` `网站模板` `Website Template` `HTML生成` `SEO优化` `响应式网站` `Responsive Website`
