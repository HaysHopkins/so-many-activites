# So Many Activities

This repository contains two separate applications:

1. **Jekyll GitHub Pages Site** (`site/`) - A static site deployed to GitHub Pages
2. **Go Wiki Application** (`app/`) - A web-based wiki application built with Go

## Project Structure

```
.
├── site/          # Jekyll GitHub Pages site
│   ├── _config.yml
│   ├── index.md
│   ├── Gemfile
│   └── ...
├── app/           # Go wiki web application
│   ├── wiki.go
│   ├── tmpl/
│   ├── data/
│   └── go.mod
└── .github/
    └── workflows/
        └── jekyll.yml  # GitHub Pages deployment workflow
```

## Jekyll Site (`site/`)

### Getting Started

1. Navigate to the site directory:
   ```bash
   cd site
   ```

2. Install Jekyll and Bundler:
   ```bash
   gem install bundler
   ```

3. Install dependencies:
   ```bash
   bundle install
   ```

4. Build and serve the site locally:
   ```bash
   bundle exec jekyll serve
   ```

5. Visit `http://localhost:4000` in your browser.

### Deployment

The Jekyll site is automatically deployed to GitHub Pages when you push to the `main` branch. The workflow builds from the `site/` directory.

### Adding Content

#### Adding a New Page

Create a new `.md` file in the `site/` directory with the following front matter:

```yaml
---
layout: page
title: "Your Page Title"
permalink: /your-url-path/
---
```

#### Adding a New Post

Create a new file in the `site/_posts/` directory with the format `YYYY-MM-DD-post-name.md`:

```yaml
---
layout: post
title: "Your Post Title"
date: YYYY-MM-DD hh:mm:ss -0000
categories: category1 category2
---
```

## Go Wiki Application (`app/`)

A simple wiki web application based on the [Go wiki tutorial](https://go.dev/doc/articles/wiki/).

### Getting Started

1. Navigate to the app directory:
   ```bash
   cd app
   ```

2. Make sure you have Go installed (version 1.21 or later)

3. Run the application:
   ```bash
   go run wiki.go
   ```

4. Visit `http://localhost:8080/view/ANewPage` in your browser to create and edit a new page.

### Features

- View wiki pages
- Edit wiki pages
- Save wiki pages to disk
- Simple HTML templates for viewing and editing

For more details, see the [app/README.md](app/README.md) file.

## Deployment

- **Jekyll Site**: Automatically deployed to GitHub Pages when pushing to the `main` branch. The workflow builds from the `site/` directory.
- **Go Wiki**: This is a standalone application that needs to be deployed separately (e.g., to a cloud service, VPS, or container platform).

For more information about Jekyll and GitHub Pages:
- [Creating a GitHub Pages site with Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll)
- [Adding content to your GitHub Pages site using Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-content-to-your-github-pages-site-using-jekyll)

