# Siddharth Syal's Personal Website

A modern, fast personal website built with [Hugo](https://gohugo.io/) and the [Stack theme](https://github.com/CaiJimmy/hugo-theme-stack).

## 🚀 Quick Start

### Development Server

```bash
hugo server -D
```

Visit `http://localhost:1313` to see your site with live reload.

### Build for Production

```bash
hugo --minify
```

The built site will be in the `public/` directory.

## 📁 Project Structure

```
personalWebsite/
├── content/              # All content files
│   ├── _index.md        # Homepage content
│   ├── posts/           # Blog posts
│   │   ├── welcome/
│   │   └── getting-started-with-hugo/
│   └── page/            # Static pages
│       ├── about/
│       ├── archives/
│       └── search/
├── static/              # Static assets (images, etc.)
│   └── img/
│       └── avatar.png   # Your profile picture
├── themes/              # Hugo themes
│   └── hugo-theme-stack/
├── hugo.toml           # Site configuration
└── public/             # Generated site (gitignored)
```

## ✍️ Creating Content

### New Blog Post

```bash
hugo new posts/my-new-post/index.md
```

Then edit the file with your content. Front matter example:

```yaml
---
title: "My Post Title"
description: "A brief description"
date: 2026-02-13
slug: my-post
categories:
    - Category Name
tags:
    - tag1
    - tag2
draft: false
---

Your content here...
```

### New Page

```bash
hugo new page/my-page/index.md
```

## 🎨 Customization

### Update Configuration

Edit `hugo.toml` to change:
- Site title, URL, and description
- Social media links
- Menu items
- Theme settings

### Add Your Avatar

Replace `static/img/avatar.png` with your photo.

### Custom Styling

Create custom CSS in `assets/scss/custom.scss`:

```scss
// Your custom styles here
```

## 📝 Content Tips

1. **Use Front Matter** - Always include complete front matter
2. **Images** - Place images next to your markdown files
3. **Draft Posts** - Set `draft: true` to hide from production
4. **Categories & Tags** - Use for organization and discovery
5. **Descriptions** - Write good descriptions for SEO

## 🌐 Deployment

### Netlify

1. Connect your GitHub repository
2. Set build command: `hugo --minify`
3. Set publish directory: `public`

### GitHub Pages

Use the included GitHub Actions workflow (create `.github/workflows/deploy.yml`).

### Vercel

Simply connect your repository - Vercel auto-detects Hugo.

## 📚 Resources

- [Hugo Documentation](https://gohugo.io/documentation/)
- [Stack Theme Docs](https://stack.jimmycai.com)
- [Markdown Guide](https://www.markdownguide.org/)

## 🔧 Development

### Requirements

- Hugo Extended v0.87.0 or higher
- Git (for theme management)

### Installing Hugo

**macOS:**
```bash
brew install hugo
```

**Windows:**
```bash
choco install hugo-extended
```

**Linux:**
```bash
snap install hugo
```

## 📄 License

This site's content is yours. The Stack theme is licensed under GPL v3.0.

---

Built with ❤️ using Hugo