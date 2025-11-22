# Jekyll GitHub Pages Site

This is a Jekyll-based GitHub Pages site. 

## Getting Started

1. Install Jekyll and Bundler:
   ```bash
   gem install bundler
   ```

2. Install dependencies:
   ```bash
   bundle install
   ```

3. Build and serve the site locally:
   ```bash
   bundle exec jekyll serve
   ```

4. Visit `http://localhost:4000` in your browser.

## Project Structure

- `_config.yml` - Jekyll configuration file
- `index.md` - Home page
- `about.md` - About page
- `_posts/` - Directory containing blog posts
- `Gemfile` - Ruby dependencies managed by Bundler

## Adding Content

### Adding a New Page

Create a new `.md` file in the root directory with the following front matter:

```yaml
---
layout: page
title: "Your Page Title"
permalink: /your-url-path/
---
```

### Adding a New Post

Create a new file in the `_posts/` directory with the format `YYYY-MM-DD-post-name.md`:

```yaml
---
layout: post
title: "Your Post Title"
date: YYYY-MM-DD hh:mm:ss -0000
categories: category1 category2
---
```

## Deployment

This site is configured to work with GitHub Pages. Once you push to your repository and configure GitHub Pages in the repository settings, your site will be automatically built and deployed.

For more information, see:
- [Creating a GitHub Pages site with Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll)
- [Adding content to your GitHub Pages site using Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-content-to-your-github-pages-site-using-jekyll)

