## Vittorio Caggiano — Personal Site

This repository contains the source for my personal website, built with Jekyll and served via GitHub Pages.

---

## Requirements

- macOS (or any Unix-like system)
- Ruby (via Homebrew is recommended)
- Bundler

Install Ruby and Bundler (if you don’t have them already):

```bash
brew install ruby
gem install bundler
```

You may need to open a new terminal window after installing Ruby so that your shell picks up the updated `PATH`.

---

## Setup

Clone the repository (if you haven’t already) and install dependencies with Bundler:

```bash
cd /path/to/Vittorio-Caggiano.github.io
bundle install
```

This uses the `Gemfile` in the repo to install Jekyll and all required plugins.

---

## Running the site locally

From the project root:

```bash
bundle exec jekyll serve --livereload
```

Then open the site in your browser:

- `http://127.0.0.1:4000` (default Jekyll address)

Useful flags:

- Change port (e.g., if 4000 is busy):

  ```bash
  bundle exec jekyll serve --livereload --port 4001
  ```

- Build without serving:

  ```bash
  bundle exec jekyll build
  ```

The generated static site will be in the `_site` directory.

---

## Deployment

This repo is configured for GitHub Pages. After committing your changes:

```bash
git add .
git commit -m "Update site content"
git push
```

GitHub Pages will automatically rebuild and deploy the site based on your repository settings. It may take a minute or two for changes to appear live.

---

## Content structure (quick reference)

- `_pages/` — top-level pages (e.g., `about.md`, `cv.md`, etc.)
- `_posts/` — blog posts (if enabled)
- `_layouts/` — HTML layouts
- `_includes/` — reusable HTML snippets
- `assets/` — CSS, JS, fonts, and images

Most content editing will happen in `_pages/` and `_posts/`.

