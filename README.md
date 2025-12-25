# reedz.name

A minimalist blog for a software engineer, built with Jekyll and hosted on GitHub Pages.

## About

This is a simple, clean blog focused on software engineering topics.

## Local Development

To run this site locally:

```bash
# Install dependencies
bundle install

# Serve the site
bundle exec jekyll serve
```

Then visit `http://localhost:4000` in your browser.

## Adding New Posts

Create a new file in the `_posts` directory with the format:

```
_posts/YYYY-MM-DD-title.md
```

Include the front matter at the top:

```yaml
---
layout: post
title: "Your Post Title"
date: YYYY-MM-DD
tags: [tag1, tag2]
---
```

Then write your content in Markdown below the front matter.

## Structure

- `_config.yml` - Site configuration
- `_layouts/` - Page templates
- `_posts/` - Blog posts
- `assets/css/` - Stylesheets
- `index.md` - Homepage
- `blog.md` - Blog listing page
- `about.md` - About page

## License

Content and design © 2025 Reedz