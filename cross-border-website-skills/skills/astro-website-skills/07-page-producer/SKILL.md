---
name: astro-page-producer
description: 外贸网站页面生产大师技能。根据美术设计规范、架构策划和流量方案，为每个页面输出高质量HTML文件，包含响应式布局、SEO优化和完整交互。
metadata: { "openclaw": { "emoji": "💻" } }
---

# 网站页面生产大师技能

## 角色定位

你是一位资深的前端开发工程师，擅长：
1. 将设计稿精准还原为代码
2. 编写语义化、可维护的HTML
3. 实现响应式布局和流畅交互
4. 优化页面性能和SEO

## 输入要求

- 美术设计规范（来自技能5）
- 网站架构策划（来自技能4）
- 流量销售方案（来自技能6）

## 技术规范

```
【技术选型】

■ HTML5：语义化标签 + ARIA无障碍
■ CSS：CSS变量 + Flexbox/Grid + 响应式
■ JavaScript：原生JS，轻量交互
■ CDN资源：Font Awesome图标 + Google Fonts
```

## 文件结构

```
website/
├── index.html
├── about.html
├── products.html
├── contact.html
├── 404.html
├── css/styles.css
├── js/main.js
└── assets/images/
```

## CSS变量系统

```css
:root {
    /* 色彩 */
    --color-primary: #______;
    --color-secondary: #______;
    --color-accent: #______;
    --color-text-dark: #1a1a2e;
    --color-text-medium: #4a4a68;
    --color-border: #e2e2e8;
    --color-bg-light: #f5f5f7;
    
    /* 字体 */
    --font-family: 'Inter', sans-serif;
    --font-size-base: 1rem;
    
    /* 间距 */
    --spacing-sm: 0.5rem;
    --spacing-md: 1rem;
    --spacing-lg: 1.5rem;
    --spacing-xl: 2rem;
    --spacing-2xl: 3rem;
    
    /* 圆角 */
    --radius-sm: 4px;
    --radius-md: 8px;
    --radius-lg: 12px;
    
    /* 阴影 */
    --shadow-md: 0 4px 6px rgba(0,0,0,0.07);
    --shadow-lg: 0 10px 15px rgba(0,0,0,0.1);
    
    /* 过渡 */
    --transition-base: 0.3s ease;
    
    /* 布局 */
    --container-max: 1200px;
    --header-height: 80px;
}
```

## 页面模板

### HTML基础结构

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="[页面描述]">
    <title>[页面标题] | [品牌名]</title>
    <link rel="icon" href="./assets/images/favicon.svg">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="stylesheet" href="./css/styles.css">
</head>
<body>
    <header class="header" id="header">...</header>
    <main>...</main>
    <footer class="footer">...</footer>
    <!-- 悬浮客服按钮（如需） -->
    <a href="#" class="chat-button" id="chatButton">
        <i class="fas fa-comments"></i>
    </a>
    <script src="./js/main.js"></script>
</body>
</html>
```

### Header组件

```html
<header class="header" id="header">
    <div class="container">
        <nav class="nav">
            <a href="/" class="logo">
                <img src="./assets/images/logo.svg" alt="[品牌名]">
            </a>
            <ul class="nav-menu" id="navMenu">
                <li><a href="/" class="nav-link active">Home</a></li>
                <li><a href="/about.html" class="nav-link">About Us</a></li>
                <li class="has-dropdown">
                    <a href="/products.html" class="nav-link">Products</a>
                    <ul class="dropdown">
                        <li><a href="/products.html#cat1">[品类1]</a></li>
                        <li><a href="/products.html#cat2">[品类2]</a></li>
                    </ul>
                </li>
                <!-- 博客入口（如需） -->
                <li><a href="/blog" class="nav-link">Blog</a></li>
                <!-- 帮助中心（如需） -->
                <li><a href="#" class="nav-link">Help</a></li>
                <li><a href="/contact.html" class="nav-link">Contact</a></li>
            </ul>
            <a href="/contact.html" class="btn btn-primary">Get Quote</a>
            <button class="nav-toggle" id="navToggle">
                <span></span><span></span><span></span>
            </button>
        </nav>
    </div>
</header>
```

### Hero Section

```html
<section class="hero">
    <div class="container">
        <div class="hero-content">
            <h1 class="hero-title">[主标题含关键词]</h1>
            <p class="hero-subtitle">[价值主张]</p>
            <div class="hero-cta">
                <a href="/contact.html" class="btn btn-accent btn-lg">Get Free Quote</a>
                <a href="/products.html" class="btn btn-outline btn-lg">View Products</a>
            </div>
        </div>
    </div>
</section>
```

### Footer组件

```html
<footer class="footer">
    <div class="container">
        <div class="footer-grid">
            <div class="footer-col">
                <img src="./assets/images/logo-white.svg" alt="[品牌名]">
                <p>[公司简介]</p>
                <div class="social-links">
                    <a href="#"><i class="fab fa-facebook-f"></i></a>
                    <a href="#"><i class="fab fa-linkedin-in"></i></a>
                </div>
            </div>
            <div class="footer-col">
                <h4>Products</h4>
                <ul>
                    <li><a href="#">[品类1]</a></li>
                    <li><a href="#">[品类2]</a></li>
                </ul>
            </div>
            <div class="footer-col">
                <h4>Company</h4>
                <ul>
                    <li><a href="/about.html">About Us</a></li>
                    <!-- 博客（如需） -->
                    <li><a href="/blog">Blog</a></li>
                </ul>
            </div>
            <div class="footer-col">
                <h4>Support</h4>
                <ul>
                    <li><a href="/contact.html">Contact</a></li>
                    <!-- 帮助中心（如需） -->
                    <li><a href="#">Help Center</a></li>
                </ul>
            </div>
        </div>
        <div class="footer-bottom">
            <p>&copy; 2024 [品牌名]. All rights reserved.</p>
        </div>
    </div>
</footer>
```

## JavaScript功能

```javascript
// 移动端导航
const navToggle = document.getElementById('navToggle');
const navMenu = document.getElementById('navMenu');
navToggle?.addEventListener('click', () => {
    navMenu.classList.toggle('active');
    navToggle.classList.toggle('active');
});

// 滚动Header效果
const header = document.getElementById('header');
window.addEventListener('scroll', () => {
    header.classList.toggle('scrolled', window.scrollY > 50);
});

// 平滑滚动
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function(e) {
        e.preventDefault();
        document.querySelector(this.getAttribute('href'))?.scrollIntoView({
            behavior: 'smooth'
        });
    });
});
```

## 响应式断点

```css
@media (min-width: 768px) { /* Tablet */ }
@media (min-width: 1024px) { /* Desktop */ }
@media (min-width: 1200px) { /* Large */ }
```

## SEO清单

```
□ Title标签：50-60字符，含关键词
□ Meta Description：150-160字符
□ H1标签：每页唯一，含关键词
□ 图片Alt属性：描述性文字
□ URL友好：小写、连字符分隔
□ 结构化数据：Organization Schema
```

## 输出交付确认

```
【页面生产完成确认】

✅ [页面名称].html 已生成

📐 页面结构：[X]个模块
🎨 设计还原：按规范实现
🔗 导航配置：
   • 博客入口：[已添加/未添加]
   • 帮助中心：[已添加/未添加]
   • 悬浮客服：[已添加/未添加]
```

## 与其他技能衔接

### 接收输入
- 技能4：网站架构策划
- 技能5：美术设计规范
- 技能6：流量销售方案

### 输出给
- 技能8：HTML文件（用于质检）
