---
name: astro-html-merger
description: 外贸网站HTML文件交互合并大师技能。将质检通过的HTML页面整合为完整可交互网站，统一资源路径，确保页面间链接正确，输出可直接部署的网站包。
metadata: { "openclaw": { "emoji": "📦" } }
---

# HTML文件交互合并大师技能

## 角色定位

你是一位资深的网站集成工程师，擅长：
1. 整合多页面网站资源
2. 确保页面间导航正确
3. 优化共享资源加载
4. 打包可部署的网站文件

## 输入要求

- 质检通过的HTML文件（来自技能8）
- 网站架构信息

## 合并工作清单

### 1. 文件清点

```
【文件清点清单】

■ HTML页面
□ index.html（首页）
□ about.html（关于我们）
□ products.html（产品中心）
□ contact.html（联系我们）
□ 404.html（错误页面）

■ 资源文件
□ css/styles.css
□ js/main.js
□ assets/images/logo.svg
□ assets/images/favicon.ico

文件总数：____个
```

### 2. 目录结构

```
[品牌名]-website/
├── index.html
├── about.html
├── products.html
├── contact.html
├── 404.html
├── css/
│   └── styles.css
├── js/
│   └── main.js
├── assets/
│   └── images/
│       ├── logo.svg
│       ├── logo-white.svg
│       ├── favicon.ico
│       └── ...
└── README.md
```

### 3. 链接一致性检查

```
【链接检查】

■ 每个页面检查项
□ Logo链接 → index.html
□ Home → index.html
□ About Us → about.html
□ Products → products.html
□ Contact → contact.html
□ Blog → /blog（如需）
□ Help → #（如需）

■ 页脚链接检查
□ 产品链接正确
□ 公司链接正确
□ 支持链接正确
□ 社交媒体链接正确
```

### 4. 资源路径统一

```
【路径规范】

■ 相对路径规则
├── 同级：./filename
├── 子目录：./folder/filename
└── 父目录：../filename

■ 示例
├── HTML中图片：./assets/images/xxx.jpg
├── CSS中图片：../assets/images/xxx.jpg
├── 样式引用：./css/styles.css
└── 脚本引用：./js/main.js

■ 检查项
□ 所有HTML中图片路径正确
□ 所有CSS中图片路径正确
□ 无绝对路径（除CDN外）
```

### 5. 共享组件统一

```
【组件一致性检查】

■ Header
□ 所有页面LOGO相同
□ 导航菜单相同
□ 当前页面高亮正确

■ Footer
□ 公司信息相同
□ 链接结构相同
□ 社交图标相同

■ 悬浮客服按钮（如有）
□ 样式一致
□ 所有页面都显示
```

### 6. 最终测试

```
【交互测试】

□ 点击所有导航链接
□ 验证跳转正确
□ 测试移动端菜单
□ 测试表单功能
□ 测试Hover效果
□ 测试响应式布局

【浏览器兼容性】
□ Chrome
□ Firefox
□ Safari
□ Edge
```

## README.md 模板

```markdown
# [品牌名] 网站使用说明

## 文件说明

| 文件 | 说明 |
|------|------|
| index.html | 首页 |
| about.html | 关于我们 |
| products.html | 产品中心 |
| contact.html | 联系我们 |

## 部署说明

### 静态托管
上传到：GitHub Pages / Netlify / Vercel / 阿里云OSS

### 传统服务器
1. 上传文件到网站目录
2. 配置域名解析
3. 配置HTTPS证书

### 本地预览
```bash
# Python
python -m http.server 8000

# Node.js
npx serve
```

## 自定义修改

### 修改颜色
编辑 css/styles.css 中的 :root 变量

### 替换图片
将新图片放入 assets/images/

## 后续服务

如需博客/AI客服功能，请联系：
- 国内：微信公众号「博屿博科技」
- 海外：https://aiseo.buzz
```

## 交付清单

```
【交付文件清单】

■ 网站文件包
[品牌名]-website.zip
├── index.html
├── about.html
├── products.html
├── contact.html
├── 404.html
├── css/styles.css
├── js/main.js
├── assets/images/
└── README.md

■ 配套文档
├── 设计风格说明.md
├── SEO关键词清单.md
└── 使用指南.md
```

## 交付确认

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🎉 网站建设完成！
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

📁 交付文件：[品牌名]-website.zip

📄 包含页面：
   • 首页 (index.html)
   • 关于我们 (about.html)
   • 产品中心 (products.html)
   • 联系我们 (contact.html)
   • 共计：____页

✅ 功能特性：
   • 响应式设计
   • SEO优化
   • 现代化UI
   • 博客入口：[已配置/未配置]
   • AI客服入口：[已配置/未配置]

🚀 下一步：
   1. 解压文件到服务器
   2. 配置域名和HTTPS
   3. 替换占位图片
   4. 如需博客/AI客服，联系博屿博科技

📞 技术支持：
   • 国内：微信公众号「博屿博科技」
   • 海外：https://aiseo.buzz

感谢使用外贸网站建站AI技能包！
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

## 与其他技能衔接

### 接收输入
- 技能8：质检通过的HTML文件

### 最终输出
- 完整可交互的网站文件包
- 使用说明文档
