---
title: Mizuki 简明使用指南
published: 2024-04-01
description: "如何使用这个博客模板。"
image: "./cover.webp"
tags: ["Mizuki", "博客", "自定义"]
category: 指南
draft: true
---

这个博客模板基于 [Astro](https://astro.build/) 构建。本指南未提到的内容，可以在 [Astro 文档](https://docs.astro.build/) 中寻找答案。

## 文章 Frontmatter

```yaml
---
title: 我的第一篇博客文章
published: 2023-09-09
description: 这是我的 Astro 新博客的第一篇文章。
image: ./cover.jpg
tags: [Foo, Bar]
category: 前端
draft: false
---
```

| 属性 | 说明 |
| --- | --- |
| `title` | 文章标题。 |
| `published` | 文章发布日期。 |
| `pinned` | 是否将文章置顶到文章列表顶部。 |
| `priority` | 置顶文章的优先级。数值越小优先级越高，例如 `0`、`1`、`2`。 |
| `description` | 文章的简短描述，会显示在首页等列表页面中。 |
| `image` | 文章封面图路径。<br/>1. 以 `http://` 或 `https://` 开头：使用网络图片。<br/>2. 以 `/` 开头：使用 `public` 目录中的图片。<br/>3. 不带以上前缀：相对于当前 Markdown 文件。 |
| `tags` | 文章标签。 |
| `category` | 文章分类。 |
| `licenseName` | 文章内容使用的许可协议名称。 |
| `author` | 文章作者。 |
| `sourceLink` | 文章内容的来源链接或参考链接。 |
| `draft` | 是否为草稿。设为 `true` 时不会在生产环境中显示。 |

## 文章文件应该放在哪里

文章文件应该放在 `src/content/posts/` 目录中。你也可以创建子目录，用来更好地组织文章和相关资源。

```text
src/content/posts/
├── post-1.md
└── post-2/
    ├── cover.webp
    └── index.md
```
