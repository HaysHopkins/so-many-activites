# Go Wiki Application

This is a simple wiki web application built with Go, based on the [Go wiki tutorial](https://go.dev/doc/articles/wiki/).

## Features

- View wiki pages
- Edit wiki pages
- Save wiki pages to disk
- Simple HTML templates for viewing and editing

## Getting Started

1. Make sure you have Go installed (version 1.21 or later)

2. Navigate to the app directory:
   ```bash
   cd app
   ```

3. Run the application:
   ```bash
   go run wiki.go
   ```

4. Visit `http://localhost:8080/view/ANewPage` in your browser to create and edit a new page.

## Project Structure

- `wiki.go` - Main application file with handlers and page logic
- `tmpl/` - HTML templates for viewing and editing pages
  - `view.html` - Template for viewing pages
  - `edit.html` - Template for editing pages
- `data/` - Directory where wiki pages are stored as text files (created automatically)
- `go.mod` - Go module file

## Usage

- View a page: `http://localhost:8080/view/PageName`
- Edit a page: `http://localhost:8080/edit/PageName`
- Pages are automatically saved to the `data/` directory as `.txt` files

