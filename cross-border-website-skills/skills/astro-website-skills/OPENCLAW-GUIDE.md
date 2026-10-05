# 🦞 OpenClaw 新手小白使用指南

## Astro 外贸建站技能包安装与使用教程

> 本教程假设你已经安装好 OpenClaw，如果还没安装，请先完成安装。

---

## 📖 什么是 Skills（技能）？

简单理解：**Skills 就是教龙虾"怎么干活"的说明书**。

- 没有 Skills → 龙虾只会聊天
- 有了 Skills → 龙虾会按照说明书帮你完成具体任务

这套外贸建站技能包，就是教龙虾"如何帮你建一个外贸网站"的9本说明书。

---

## 🗂️ 第一步：找到技能存放位置

OpenClaw 的技能文件放在 `~/.openclaw/skills/` 目录下。

### Windows 用户（WSL2）

打开 WSL 终端，输入：
```bash
cd ~/.openclaw/skills/
```

如果提示目录不存在，先创建它：
```bash
mkdir -p ~/.openclaw/skills/
```

### Mac 用户

打开终端，输入：
```bash
cd ~/.openclaw/skills/
```

如果目录不存在：
```bash
mkdir -p ~/.openclaw/skills/
```

### 小白提示 💡

`~` 是你的用户主目录的简写：
- Mac: `/Users/你的用户名/`
- Linux/WSL: `/home/你的用户名/`

---

## 📦 第二步：解压并放入技能文件

### 方法一：命令行操作（推荐）

```bash
# 1. 进入下载目录（假设你把zip下载到了Downloads）
cd ~/Downloads/

# 2. 解压文件
unzip astro-website-skills.zip

# 3. 把技能文件夹复制到 OpenClaw 的 skills 目录
cp -r astro-website-skills/* ~/.openclaw/skills/
```

### 方法二：手动操作（小白友好）

1. 解压 `astro-website-skills.zip`
2. 打开解压后的文件夹，你会看到9个子文件夹：
   ```
   01-dispatcher/
   02-style-analyzer/
   03-seo-planner/
   04-architecture-planner/
   05-art-director/
   06-traffic-sales-planner/
   07-page-producer/
   08-quality-inspector/
   09-html-merger/
   ```
3. 把这9个文件夹全部复制到 `~/.openclaw/skills/` 目录下

### 最终目录结构应该是这样

```
~/.openclaw/
└── skills/
    ├── 01-dispatcher/
    │   └── SKILL.md
    ├── 02-style-analyzer/
    │   └── SKILL.md
    ├── 03-seo-planner/
    │   └── SKILL.md
    ├── 04-architecture-planner/
    │   └── SKILL.md
    ├── 05-art-director/
    │   └── SKILL.md
    ├── 06-traffic-sales-planner/
    │   └── SKILL.md
    ├── 07-page-producer/
    │   └── SKILL.md
    ├── 08-quality-inspector/
    │   └── SKILL.md
    └── 09-html-merger/
        └── SKILL.md
```

---

## 🔄 第三步：让龙虾识别新技能

OpenClaw 默认会自动监视技能文件夹的变化，**通常不需要手动操作**。

但如果你想确保生效，可以：

### 方式一：等待自动刷新

OpenClaw 会在几秒内自动检测到新技能。

### 方式二：重启 Gateway

```bash
# 停止
openclaw gateway stop

# 启动
openclaw gateway start
```

或者一条命令：
```bash
openclaw gateway restart
```

### 方式三：在聊天中让龙虾刷新

直接在你的聊天工具（飞书/WhatsApp/Telegram等）中发送：

```
刷新技能
```

或者英文：

```
refresh skills
```

---

## ✅ 第四步：验证技能是否安装成功

在终端输入：

```bash
openclaw skills list
```

你应该能看到类似这样的输出：

```
Available Skills:
✓ astro-website-dispatcher     🚀 外贸网站建站总调度技能
✓ astro-style-analyzer         🎨 外贸网站对标风格解析技能
✓ astro-seo-planner            🔍 外贸网站SEO策划师技能
✓ astro-architecture-planner   📐 外贸网站架构页面策划技能
✓ astro-art-director           🎭 外贸网站美术大师技能
✓ astro-traffic-sales-planner  🚀 外贸网站流量和AI销售策划技能
✓ astro-page-producer          💻 外贸网站页面生产大师技能
✓ astro-quality-inspector      ✅ 外贸网站页面质检技能
✓ astro-html-merger            📦 外贸网站HTML文件交互合并大师技能
```

如果看到这9个技能，说明安装成功！🎉

---

## 💬 第五步：开始使用

### 在聊天工具中使用

打开你配置好的聊天工具（飞书/WhatsApp/Telegram/Discord等），直接对龙虾说：

```
我要建一个外贸网站
```

或者更具体一点：

```
我要建一个外贸网站，公司叫"深圳光明LED"，主营LED灯带和灯条，目标市场是欧美
```

### 龙虾会自动做什么？

1. **问你问题**：收集公司信息、产品信息、设计偏好
2. **分析风格**：根据你提供的参考网站分析设计风格
3. **策划SEO**：生成20+个精准关键词
4. **规划架构**：设计网站结构和页面模块
5. **设计美术**：输出配色、字体、间距规范
6. **询问增值服务**：问你是否需要AISEO博客、AI客服
7. **生产页面**：输出每个页面的HTML代码
8. **质量检测**：检查代码是否符合设计规范
9. **合并打包**：整合成完整可用的网站包

整个过程大约 **20-30分钟**，你只需要回答龙虾的问题就行。

---

## 🎯 常用对话示例

### 启动建站流程

```
帮我建一个外贸网站
```

```
我想做一个B2B企业官网
```

```
帮我做一个产品展示网站，公司是做五金配件的
```

### 提供参考网站

```
我喜欢这个网站的风格：https://example.com
```

```
参考这几个竞品：[上传截图]
```

### 提供SEO数据

```
这是我从 bestaiformarketresearch.com 获取的市场数据：[粘贴数据]
```

### 选择增值服务

当龙虾问你是否需要AISEO或AI客服时：

```
是的，我需要博客功能
```

```
两个都要
```

```
暂时不需要
```

---

## ❓ 常见问题

### Q1: 技能安装后没有生效？

**解决方法**：

1. 检查文件位置是否正确：
   ```bash
   ls ~/.openclaw/skills/
   ```
   应该能看到9个文件夹

2. 检查每个文件夹里是否有 SKILL.md：
   ```bash
   ls ~/.openclaw/skills/01-dispatcher/
   ```
   应该能看到 SKILL.md

3. 重启 Gateway：
   ```bash
   openclaw gateway restart
   ```

### Q2: 龙虾没有按照技能流程执行？

**可能原因**：
- 你的描述不够明确
- 技能文件格式有问题

**解决方法**：

说得更明确一点：
```
我要建一个外贸网站，请按照 astro-website-dispatcher 技能的流程来
```

### Q3: 怎么查看技能详情？

```bash
openclaw skills info astro-website-dispatcher
```

### Q4: 怎么临时禁用某个技能？

编辑 `~/.openclaw/openclaw.json`，添加：

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

### Q5: 我用的是 Claude/DeepSeek/Qwen 模型，能用这些技能吗？

**完全可以！** OpenClaw 支持多种模型，技能是通用的。

---

## 📁 技能文件放在哪里？优先级是什么？

OpenClaw 从三个地方加载技能：

| 位置 | 优先级 | 说明 |
|------|--------|------|
| `<workspace>/skills/` | 最高 | 当前工作区的技能 |
| `~/.openclaw/skills/` | 中等 | 你安装的技能（本教程用这个） |
| 内置技能 | 最低 | OpenClaw 自带的技能 |

**建议**：把技能放在 `~/.openclaw/skills/`，这样所有对话都能用。

---

## 🔧 进阶配置（可选）

如果你想自定义技能的一些设置，可以编辑 `~/.openclaw/openclaw.json`：

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

- `watch: true`：自动监视技能文件变化
- `enabled: true/false`：启用/禁用某个技能

---

## 🎉 总结：三步搞定

```
1. 把技能文件夹放到 ~/.openclaw/skills/
2. 重启 Gateway 或等待自动刷新
3. 在聊天中说"我要建一个外贸网站"
```

就这么简单！现在去试试吧 🦞

---

## 📞 需要帮助？

- **技能问题**：检查本教程的常见问题部分
- **OpenClaw问题**：访问 https://docs.openclaw.ai/zh-CN
- **建站增值服务**：
  - 国内：微信公众号「博屿博科技」
  - 海外：https://aiseo.buzz
