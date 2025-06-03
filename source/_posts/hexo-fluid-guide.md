---
title: Hexo Fluid 主题配置详解
date: 2024-02-06 20:30:00
categories:
  - 教程
tags:
  - Hexo
  - Fluid
  - 配置
---

# Hexo Fluid 主题配置详解

## 1. 顶部导航栏配置

### 1.1 博客标题
```yaml
navbar:
  blog_title: "我的博客"  # 可修改为您想要的博客名称
```

### 1.2 毛玻璃效果
```yaml
navbar:
  ground_glass:
    enable: true    # 是否启用
    blur: 0.7      # 模糊度，范围0~1
```

### 1.3 导航菜单
```yaml
navbar:
  menu:
    - { key: "首页", link: "/" }
    - { key: "归档", link: "/archives/" }
    - { key: "分类", link: "/categories/" }
    - { key: "标签", link: "/tags/" }
    - { key: "关于", link: "/about/" }
```
您可以：
- 修改菜单项的显示文字（key）
- 添加新的菜单项
- 修改链接地址（link）

## 2. 首页横幅配置

### 2.1 横幅图片
```yaml
index:
  banner_img: /images/banner.jpg  # 图片路径
```
需要您：
1. 准备一张高质量的横幅图片（建议尺寸：1920x1080px）
2. 将图片放在 `source/images/` 目录下
3. 修改配置中的图片路径

### 2.2 横幅高度与遮罩
```yaml
index:
  banner_img_height: 85    # 高度（建议范围：60~100）
  banner_mask_alpha: 0.3   # 遮罩透明度（0~1）
```

### 2.3 首页标语
```yaml
index:
  slogan:
    enable: true
    text: "分享技术，记录生活"   # 您的口号
    font_size: 1.5rem           # 字体大小
    line_height: 1.5           # 行高
```

## 3. 文章卡片设置

### 3.1 文章信息显示
```yaml
index:
  post_meta:
    date: true      # 显示日期
    category: true  # 显示分类
    tag: true      # 显示标签
```

### 3.2 文章摘要
```yaml
index:
  article_img_align: left   # 图片位置：left/right/center
  excerpt_type: text       # 摘要类型：text/html
  excerpt_length: 200      # 摘要长度
  auto_excerpt:
    enable: true          # 自动摘要
```

## 4. 颜色主题

```yaml
color:
  body_bg_color: "#f8f9fa"        # 背景色
  board_color: "#fff"             # 板块背景色
  text_color: "#3c4858"          # 文字颜色
  link_color: "#3c4858"          # 链接颜色
  link_hover_color: "#1abc9c"    # 链接悬停颜色
```

## 5. 需要创建的页面

要使所有功能正常工作，您需要创建以下页面：

1. 分类页：
```bash
hexo new page categories
```

2. 标签页：
```bash
hexo new page tags
```

3. 关于页：
```bash
hexo new page about
```

## 6. 自定义修改步骤

1. 修改导航栏
   - 编辑 `_config.fluid.yml` 中的 `navbar` 部分
   - 设置您的博客标题
   - 调整毛玻璃效果

2. 配置首页横幅
   - 准备并添加横幅图片
   - 调整横幅高度和遮罩透明度
   - 设置个性化的首页标语

3. 调整文章显示
   - 配置文章信息的显示项
   - 设置文章摘要的显示方式
   - 调整图片对齐方式

4. 个性化配色
   - 修改背景色
   - 调整文字和链接颜色
   - 设置悬停效果

我们可以一起逐步调整这些设置，打造一个独特的博客风格。您想先从哪个部分开始修改？ 