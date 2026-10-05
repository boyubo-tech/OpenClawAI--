# OpenClaw Skills Hub

**开箱即用的 AI Agent 技能包 · 面向跨境出海与内容生产**

> Practical AI Agent skills for cross-border eCommerce, B2B websites and content production.

[![License](https://img.shields.io/badge/License-MIT-green)](./LICENSE)
[![Skills](https://img.shields.io/badge/Skills-11-blue)](#仓库里有什么)
[![Language](https://img.shields.io/badge/Docs-中文%20%7C%20English-brightgreen)](#)

---

## 这是什么

OpenClaw 是一套 AI Agent 工具。**Skills（技能包）就是交给 Agent 的「工作说明书」**：

- 没有技能 → Agent 只会聊天
- 装上技能 → Agent 会按说明书，帮你把一件具体的事做完

本仓库把我们自己在跨境业务里用的技能包**陆续开源**出来。装上就能用，不需要编程。

**适合谁**：跨境电商 / 外贸 B2B / 独立站运营 / 内容创作者，尤其是**不想写代码**的人。

---

## 仓库里有什么

目前有两个技能包，都是**下载即用**：

| 技能包 | 干什么 | 技能数 |
| --- | --- | --- |
| **[跨境独立站建站](cross-border-website-skills/)** | 从品牌资料到上线，AI 全自动生成一个外贸网站 | 9 个 |
| **[AI 生图生视频](ai-image-video-skills/)** | 批量生成「去 AI 味」的图片提示词，并策划短视频分镜 | 2 套 |

---

## 技能包一：跨境独立站建站

面向**外贸 B2B、跨境电商、独立站**的自动建站流水线。给它品牌资料和竞品截图，它按顺序跑完 9 步，最后吐出一个可以上线的静态网站。

适用场景：企业官网、B2B 产品目录站、外贸独立站、品牌官网、工厂官网、产品展示站。

**9 个技能（按执行顺序）：**

| # | 技能 | 干什么 |
| --- | --- | --- |
| 01 | `dispatcher` | 总调度 —— 判断你的需求，把活分给下面 8 个 |
| 02 | `style-analyzer` | 解析品牌资料和竞品网站截图，定出视觉风格 |
| 03 | `seo-planner` | 基于市场数据做 SEO 关键词策略 |
| 04 | `architecture-planner` | 结合关键词和品牌，规划网站架构和页面清单 |
| 05 | `art-director` | 为每个页面出美术设计规范 |
| 06 | `traffic-sales-planner` | 规划流量入口和转化路径（AI 客服 / 在线询盘） |
| 07 | `page-producer` | 按设计规范生成每个页面的 HTML |
| 08 | `quality-inspector` | 逐项质检生成的页面 |
| 09 | `html-merger` | 把质检通过的页面合并成完整站点 |

**技术栈**：Astro 静态站点 · 零代码 · 生成的站点可直接部署到 GitHub Pages / Netlify / Vercel 等。

📖 [技能包详细说明](cross-border-website-skills/README.md) · [新手安装教程](cross-border-website-skills/TUTORIAL.md)

---

## 技能包二：AI 生图生视频

面向**内容创作者**的两套技能：一套解决「AI 生成的图一眼假」，一套解决「短视频不知道怎么拍」。

**① 去 AI 味提示词批量优化器**

批量生成图片提示词，并针对常见的「AI 感」做优化 —— 让出图更像真实拍摄。带细则库和自进化反馈机制，用得越久越贴合你的风格。

**② 博主类型视频分镜策划**

按博主类型给出分镜方案，目前覆盖两类：

- **A 型 · 户外边走边说** —— 动线策划
- **B 型 · 室内固定位置** —— 分镜策划

📖 [技能包详细说明](ai-image-video-skills/README.md)

---

## 快速开始

```bash
# 1. 克隆本仓库
git clone https://github.com/boyubo-tech/OpenClawAI--.git
cd OpenClawAI--

# 2. 挑一个技能包，把里面的技能复制到 OpenClaw 的技能目录
mkdir -p ~/.openclaw/skills
cp -r cross-border-website-skills/skills/astro-website-skills/* ~/.openclaw/skills/

# 3. 重启 OpenClaw Gateway 让技能生效
openclaw gateway stop && openclaw gateway start
```

装好后，直接跟 Agent 说「帮我建一个外贸网站」，它就会自动调用对应的技能。

> **不想用命令行？** 每个技能包目录里都有一个 `.zip`，下载解压后手动复制进去就行。
> 详细步骤见 [新手安装教程](cross-border-website-skills/TUTORIAL.md)。

---

## 目录结构

```text
.
├── README.md                          你在这里
├── LICENSE
├── cross-border-website-skills/       技能包一：跨境独立站建站
│   ├── README.md                      详细说明
│   ├── TUTORIAL.md                    新手安装教程
│   ├── astro-website-skills.zip       打包下载
│   ├── openclaw-quickstart.docx       图文快速上手
│   └── skills/                        技能文件（可直接阅读）
│       └── astro-website-skills/01-…09-/
└── ai-image-video-skills/             技能包二：AI 生图生视频
    ├── README.md
    ├── ai-image-video-skills.zip
    └── skills/                        技能文件（可直接阅读）
```

> 技能文件同时提供**展开的 Markdown** 和**打包的 zip**：想直接看内容就翻 `skills/`，想一键安装就下 `.zip`。

---

## 更新节奏

陆续开源，按业务价值分批发布。每次更新记录变更内容和影响范围。

---

## 安全声明

本仓库**不包含**：

- 商业源码
- Token / 密钥 / 账号密码
- 客户敏感数据

请把密钥放在本地 `.env`，永远不要提交上来。

---

## 联系我们

有问题、想提需求、想聊聊跨境出海，都欢迎：

- 微信公众号：**博屿博科技**
- 想要更多技能包：公众号回复关键词 **Skill**

也欢迎直接提 Issue 或 PR —— 新技能、场景模板、使用案例都欢迎。

---

## 许可证

[MIT](./LICENSE) —— 随便用、随便改、随便商用。

> 说明：本项目在 2026 年 2 月至 3 月期间曾短暂使用 GPL-3.0，自本版本起统一改为 MIT。
> 如果你手上有当时的副本，以那份副本附带的许可证为准。
