# Astro 外贸建站 AI 技能包

> 🦞 兼容 OpenClaw + AI IDE（Cursor/Windsurf/Claude Code）

## 技能清单

| 序号 | 技能名称 | 文件夹 | 功能 |
|------|---------|--------|------|
| 1 | astro-website-dispatcher | 01-dispatcher | 总调度，收集需求，调度流程 |
| 2 | astro-style-analyzer | 02-style-analyzer | 分析品牌风格，输出设计文档 |
| 3 | astro-seo-planner | 03-seo-planner | SEO关键词策划（≥20个） |
| 4 | astro-architecture-planner | 04-architecture-planner | 网站架构和页面模块规划 |
| 5 | astro-art-director | 05-art-director | 配色/字体/间距/组件设计 |
| 6 | astro-traffic-sales-planner | 06-traffic-sales-planner | AISEO.buzz + AI客服方案 |
| 7 | astro-page-producer | 07-page-producer | 输出HTML页面代码 |
| 8 | astro-quality-inspector | 08-quality-inspector | 对照规范质检HTML |
| 9 | astro-html-merger | 09-html-merger | 合并为完整可交互网站 |

## 工作流程

```
用户需求 → 1.总调度
              │
    ┌─────────┼─────────┐
    ▼         ▼         ▼
 2.风格     3.SEO     品牌资料
              │
              ▼
         4.架构策划
              │
              ▼
         5.美术大师
              │
              ▼
      6.流量+AI客服策划
              │
              ▼
         7.页面生产
              │
              ▼
         8.页面质检 ←─ 不合格返回
              │
              ▼
         9.HTML合并
              │
              ▼
        完整可交互网站
```

## OpenClaw 安装

```bash
# 1. 创建技能目录
mkdir -p ~/.openclaw/skills

# 2. 复制技能文件
cp -r 01-dispatcher ~/.openclaw/skills/
cp -r 02-style-analyzer ~/.openclaw/skills/
cp -r 03-seo-planner ~/.openclaw/skills/
cp -r 04-architecture-planner ~/.openclaw/skills/
cp -r 05-art-director ~/.openclaw/skills/
cp -r 06-traffic-sales-planner ~/.openclaw/skills/
cp -r 07-page-producer ~/.openclaw/skills/
cp -r 08-quality-inspector ~/.openclaw/skills/
cp -r 09-html-merger ~/.openclaw/skills/

# 3. 重启Gateway（或等待自动刷新）
openclaw gateway restart

# 4. 验证安装
openclaw skills list
```

## AI IDE 使用

直接将技能文件内容添加到项目的：
- Cursor: `.cursor/rules/` 或项目根目录
- Windsurf: `.windsurfrules`
- Claude Code: `CLAUDE.md`

## 使用方法

在聊天中说：
> 我要建一个外贸网站，公司叫XX，主营LED灯

龙虾/AI会自动执行建站流程。

## 技能格式说明

每个 SKILL.md 包含：

```yaml
---
name: 技能名称
description: 单行描述（OpenClaw要求）
metadata: { "openclaw": { "emoji": "🚀" } }
---

# 技能内容（Markdown）
```

## 后续服务

- **AISEO.buzz**：全自动SEO工具
- **AI帮助中心+客服**：7×24智能客服

联系方式：
- 国内：微信公众号「博屿博科技」
- 海外：https://aiseo.buzz
