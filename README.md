# TradingSentry Blog Content

This repository contains the blog content for TradingSentry, managed in Markdown format with frontmatter.

## Structure

- `/blogs/` - Contains all blog post Markdown files
- `/assets/blog-images/` - Contains all images used in blog posts

## Creating a New Blog Post

1. Create a new Markdown file in the `/blogs/` directory
2. Use the template below for the frontmatter
3. Add your content using Markdown formatting
4. Add any images to the `/assets/blog-images/` directory
5. Reference images in your posts using relative paths: `![Alt text](image-name.jpg)`

## Frontmatter Template

```markdown
---
title: Your Blog Post Title
slug: your-blog-post-slug
excerpt: A brief summary of your blog post that will appear in listing pages.
featuredImage: image-name.jpg
category: Category Name
tags:
  - tag1
  - tag2
  - tag3
author:
  name: Author Name
  image: author-image.jpg
  bio: Brief author bio that appears on the post page.
publishedAt: 2023-11-15T10:00:00Z
readTime: 5 min read
related:
  - other-post-slug-1
  - other-post-slug-2
---
```

## Required Fields

- `title`: The title of your blog post
- `slug`: The URL-friendly identifier for your post (use lowercase, hyphens instead of spaces)
- `excerpt`: A brief summary (1-2 sentences)
- `featuredImage`: The main image for your post (filename only, must be in `/assets/blog-images/`)
- `category`: The primary category for your post
- `tags`: An array of relevant tags
- `author`: Information about the author including name, image, and bio
- `publishedAt`: ISO 8601 formatted date when the post is published

## Updating the Website

The website automatically fetches content from this repository. After pushing changes:

1. New posts will appear on the site within 5 minutes 
2. To force an immediate refresh, visit `/blog/admin/refresh` on the website 