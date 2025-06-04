---
title: 博客写作完全指南：从标题到脚注的每一个细节
date: 2024-02-06 15:00:00
categories: 
  - 教程
tags:
  - 博客
  - 写作
  - 指南
description: 一篇全面的博客写作指南，涵盖从文章创建到发布的每一个细节，包含大量实用示例和最佳实践。
---

# 博客写作完全指南：从标题到脚注的每一个细节

## 1. 文章基本信息设置

### 1.1 Front-matter 配置
每篇博客文章的开头都需要包含 Front-matter，它定义了文章的基本信息：

```yaml
---
title: 文章标题
date: 2024-02-06 15:00:00
categories: 
  - 教程
  - 技术
tags:
  - 博客
  - 写作
  - 指南
description: 文章简介，会显示在文章列表和搜索结果中
---
```

#### 重要说明：
- `title`: 文章标题，建议简洁明了，不超过20个字
- `date`: 发布时间，格式为 YYYY-MM-DD HH:mm:ss
- `categories`: 分类，可以设置多个，但建议不超过3个
- `tags`: 标签，可以设置多个，建议5-8个
- `description`: 文章简介，建议50-100字

### 1.2 文章标题规范
标题是文章的第一印象，需要遵循以下原则：

1. 长度适中：建议15-20个字
2. 包含关键词：便于搜索引擎优化
3. 避免标题党：标题要准确反映内容

示例：
- ✅ 《深入理解 JavaScript 原型链：从原理到实践》
- ❌ 《震惊！你不知道的 JavaScript 秘密》

## 2. 文章内容结构

### 2.1 文章结构
一篇好的博客文章应该包含以下部分：

1. 开篇引言
2. 目录（可选）
3. 正文内容
4. 总结
5. 参考资料

### 2.2 目录生成
使用 Markdown 的标题语法自动生成目录：

```markdown
## 一级标题
### 二级标题
#### 三级标题
```

### 2.3 正文格式规范

#### 2.3.1 段落格式
- 段落之间空一行
- 每段建议3-5句话
- 重要内容可以加粗或使用引用

示例：
```markdown
这是第一段内容。

这是第二段内容，**这是重要内容**。

> 这是一段引用内容，用于强调重要信息。
```

#### 2.3.2 代码块
使用三个反引号包裹代码：

````markdown
```javascript
function hello() {
    console.log("Hello, World!");
}
```
````

#### 2.3.3 列表
有序列表：
```markdown
1. 第一项
2. 第二项
3. 第三项
```

无序列表：
```markdown
- 项目一
- 项目二
- 项目三
```

### 2.4 图片使用规范

#### 2.4.1 图片格式
- 优先使用 WebP 格式
- 备选 JPG/PNG 格式
- 图片大小建议不超过 800KB

#### 2.4.2 图片插入
```markdown
![图片描述](/img/example.jpg)
```

#### 2.4.3 图片说明
建议在图片下方添加说明文字：
```markdown
![图片描述](/img/example.jpg)
*图1：这是一张示例图片的说明文字*
```

## 3. 文章排版技巧

### 3.1 强调重点
- 使用加粗：`**重要内容**`
- 使用斜体：`*次要强调*`
- 使用引用：`> 引用内容`

### 3.2 分割线使用
在主题转换时使用分割线：
```markdown
---
```

### 3.3 表格规范
```markdown
| 表头1 | 表头2 | 表头3 |
|-------|-------|-------|
| 内容1 | 内容2 | 内容3 |
| 内容4 | 内容5 | 内容6 |
```

## 4. 文章底部设置

### 4.1 版权声明
在文章底部添加版权声明：
```markdown
---
版权声明：本文采用 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) 协议进行许可。
```

### 4.2 参考资料
列出文章引用的资料：
```markdown
## 参考资料
1. [参考链接1](https://example.com)
2. [参考链接2](https://example.com)
```

### 4.3 相关文章推荐
```markdown
## 相关文章
- [文章1标题](/path/to/article1)
- [文章2标题](/path/to/article2)
```

## 5. 文章发布检查清单

### 5.1 内容检查
- [ ] 标题是否准确反映内容
- [ ] 文章结构是否清晰
- [ ] 代码示例是否正确
- [ ] 图片是否清晰且大小适中
- [ ] 是否有错别字和语法错误

### 5.2 格式检查
- [ ] 段落间距是否合适
- [ ] 标题层级是否正确
- [ ] 列表格式是否统一
- [ ] 代码块格式是否正确
- [ ] 图片是否都有说明文字

### 5.3 SEO 检查
- [ ] 标题是否包含关键词
- [ ] 是否添加了合适的标签
- [ ] 是否设置了文章描述
- [ ] 图片是否添加了 alt 属性
- [ ] 内部链接是否合理

## 6. 文章发布流程

1. 本地预览
```bash
hexo clean
hexo generate
hexo server
```

2. 检查效果
- 访问 http://localhost:2345 预览
- 检查所有链接是否正常
- 确认图片显示正常
- 验证代码高亮效果

3. 发布文章
```bash
hexo clean
hexo generate
hexo deploy
```

## 7. 文章维护

### 7.1 定期更新
- 检查文章中的链接是否失效
- 更新过时的内容
- 补充新的相关信息

### 7.2 评论管理
- 及时回复读者评论
- 删除垃圾评论
- 收集读者反馈

## 8. 实用工具推荐

### 8.1 写作工具
- Typora：Markdown 编辑器
- VS Code：代码编辑器
- Grammarly：语法检查

### 8.2 图片处理
- TinyPNG：图片压缩
- Canva：图片设计
- Snipaste：截图工具

### 8.3 其他工具
- Git：版本控制
- Hexo：博客框架
- Fluid：博客主题

## 9. 元信息与底部信息自定义

### 9.1 作者（Author）
- **全局作者**：在 Hexo 主配置 `_config.yml` 设置 `author: 老七`
- **单篇自定义**：Front-matter 添加 `author: 张三`

### 9.2 文章发布日期（Posted on）
- 由 `date` 字段决定，格式 `YYYY-MM-DD HH:mm:ss`
- 示例：`date: 2024-02-06 15:00:00`

### 9.3 文章链接（Permalink）
- Front-matter 添加 `permalink: /my-custom-url/`

### 9.4 版权信息（License）
- 全局设置在主题配置 `_config.fluid.yml`，如：
  ```yaml
  copyright:
    enable: true
    license: CC BY-NC-SA 4.0
    license_url: https://creativecommons.org/licenses/by-nc-sa/4.0/
  ```
- 单篇文章 Front-matter 添加：
  ```yaml
  license: CC BY-NC-SA 4.0
  license_url: https://creativecommons.org/licenses/by-nc-sa/4.0/
  ```
- Markdown 末尾添加版权声明：
  ```markdown
  ---
  版权声明：本文采用 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) 协议进行许可。
  ```

### 9.5 文章简介（Description）
- Front-matter 添加 `description: 这是一篇关于如何自定义博客文章元信息的详细教程。`

### 9.6 分类与标签（Categories & Tags）
- 分类：`categories: [教程, Hexo]`
- 标签：`tags: [博客, 写作, 配置]`

### 9.7 相关文章推荐
- Markdown 末尾手动添加：
  ```markdown
  ## 相关文章
  - [Hexo Fluid 主题配置详解](/2024/02/06/hexo-fluid-guide/)
  - [Hexo 博客搭建全流程](/2024/02/06/hexo-setup/)
  ```

### 9.8 文章底部自定义内容
- Markdown 末尾添加欢迎语、二维码等：
  ```markdown
  ---
  欢迎关注我的公众号：老七的技术笔记
  ```

### 9.9 脚注底图（版权区域背景/图标）自定义

Fluid 主题文章底部的 CC 图标或背景完全可以自定义，方法如下：

**方法一：自定义 CSS 覆盖**
```css
.post-copyright {
    background-image: url('/img/my-copyright-bg.png');
    background-size: contain;
    background-repeat: no-repeat;
    background-position: right center;
}
```

**方法二：隐藏原有图标，插入自定义图片**
```css
.post-copyright .cc-icon {
    display: none;
}
.post-copyright::after {
    content: '';
    display: inline-block;
    width: 40px;
    height: 40px;
    background: url('/img/my-copyright-bg.png') no-repeat center/contain;
    vertical-align: middle;
    margin-left: 10px;
}
```

**方法三：修改主题源码**
- 编辑 `themes/fluid/layout/_partial/copyright.ejs`，将 `<svg>` 或 `<img>` 替换为你自己的图片。

**注意事项：**
- 图片建议为透明 PNG 或 SVG，尺寸建议 40x40px。
- 路径建议放在 `source/img/` 或 `source/images/` 目录下。

---

**完整 Front-matter 示例：**
```yaml
---
title: 博客写作完全指南：从标题到脚注的每一个细节
author: 老七
date: 2024-02-06 15:00:00
categories: 
  - 教程
tags:
  - 博客
  - 写作
  - 指南
description: 一篇全面的博客写作指南，涵盖从文章创建到发布的每一个细节，包含大量实用示例和最佳实践。
permalink: /blog-writing-guide/
license: CC BY-NC-SA 4.0
license_url: https://creativecommons.org/licenses/by-nc-sa/4.0/
---
```

## 结语

写作是一个不断学习和改进的过程。希望这份指南能帮助你写出更好的博客文章。记住，好的文章不仅要有好的内容，还要有好的呈现方式。持续写作，持续改进，你的博客一定会越来越好！

---
版权声明：本文采用 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) 协议进行许可。 