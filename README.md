# AIN Publication

Weekly insights on finance and technology for professionals who need to stay informed without noise.

## Features

- **Static Site**: Built with Hugo for fast loading and easy maintenance
- **Responsive Design**: Works on desktop, tablet, and mobile
- **Categories**: Finance and Technology articles
- **Newsletter**: Subscribe for weekly updates
- **RSS Feed**: Stay updated with your favorite reader
- **SEO Optimized**: Built-in sitemap and meta tags

## Tech Stack

- **Site Generator**: Hugo
- **Theme**: PaperMod
- **Hosting**: GitHub Pages (auto-deploy via GitHub Actions)
- **Newsletter**: Buttondown

## Local Development

### Prerequisites

- Hugo Extended (v0.147.0+)
- Git

### Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/ain-publication/ain-publication.git
   cd ain-publication
   ```

2. Initialize submodules:
   ```bash
   git submodule update --init --recursive
   ```

3. Start the development server:
   ```bash
   hugo server -D
   ```

4. Open http://localhost:1313 in your browser.

## Content Structure

```
content/
├── finance/           # Finance articles
│   └── article.md
├── technology/        # Technology articles
│   └── article.md
├── newsletter.md      # Newsletter signup page
└── archive.md         # Article archive
```

## Adding Articles

1. Create a new Markdown file in the appropriate category folder
2. Add frontmatter with title, date, categories, and tags
3. Write your content in Markdown
4. Commit and push to deploy

### Article Template

```markdown
---
title: "Article Title"
date: 2026-06-03T10:00:00Z
draft: false
categories: ["Finance"]
tags: ["tag1", "tag2"]
description: "Brief description of the article"
---

Your article content here...
```

## Deployment

The site automatically deploys to GitHub Pages when you push to the `main` branch.

### Manual Deployment

1. Build the site:
   ```bash
   hugo --minify
   ```

2. The output will be in the `public/` directory.

## Newsletter Integration

The newsletter uses Buttondown for email delivery. To configure:

1. Create a Buttondown account
2. Update the form action URL in `layouts/partials/newsletter-signup.html`
3. Test the subscription flow

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

MIT License - see [LICENSE](LICENSE) for details.