<div align="center">

# Academic Personal Homepage Template

**A lightweight, Jekyll-based personal academic homepage template, inspired by the design style of [Kaiming He's homepage](https://people.csail.mit.edu/kaiming/).**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Jekyll](https://img.shields.io/badge/Jekyll-4.0+-red.svg)](https://jekyllrb.com/)
[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-ready-success.svg)](https://pages.github.com/)

[View Demo](https://horizonll.github.io/kaiming-style-homepage)

</div>

---

## Features

- **Clean & Minimal Design** — Arial font family, academic-friendly layout
- **Photo + Bio Section** — Prominent introduction at the top of the page
- **Rich Sections** — News, Education, Selected Talks, Teaching, Selected Publications, Professional Service, Awards and Honors
- **YAML-driven Publications** — Manage your publication list via [`_data/publications.yml`](_data/publications.yml)
- **GitHub Pages Compatible** — Deploys automatically via the `github-pages` gem

---

## Quick Start

### 1. Create Your Repository

Click **Use this template** on GitHub to create a new repository named `<your-username>.github.io`.

### 2. Clone & Install

```bash
git clone https://github.com/<your-username>/<your-username>.github.io.git
cd <your-username>.github.io
bundle install
```

### 3. Preview Locally

```bash
bundle exec jekyll serve
```

Then open [http://localhost:4000](http://localhost:4000) in your browser.

### 4. Deploy

Push to GitHub. GitHub Pages will automatically build and serve your site at `https://<your-username>.github.io/`.

---

## Customization

### Basic Info

Edit [`index.md`](index.md):

| Item         | What to Change                                            |
| ------------ | --------------------------------------------------------- |
| Photo        | Replace `img/image.jpg` with your own photo               |
| Name & Title | Update your name, title, affiliation                      |
| Contact      | Set your email and GitHub link                            |
| Bio          | Write a short introduction paragraph                      |
| Sections     | Fill in News, Education, Talks, Teaching, Service, Awards |

### Site Config

Edit [`_config.yml`](_config.yml):

| Key           | Description                         |
| ------------- | ----------------------------------- |
| `title`       | Page title shown in the browser tab |
| `description` | A short site description            |
| `author`      | Your name                           |

### Publications

Edit [`_data/publications.yml`](_data/publications.yml) to manage your publication list. Each entry follows this format:

```yaml
- title: "Paper Title"
  authors: "<b>Your Name</b>*, Coauthor A, Coauthor B"
  venue: "Conference Name, Year"
  links:
    - text: "arXiv"
      url: "https://arxiv.org/abs/xxxx.xxxxx"
    - text: "code"
      url: "https://github.com/your-repo"
      bold: true
```

> **Tip:** Use `<b>` tags to highlight your name in the author list. The `bold: true` option on a link renders it in bold on the page.

---

## Project Structure

```
kaiming-style-homepage/
├── index.md                  # Main page content (edit your info here)
├── img/
│   └── image.jpg             # Profile photo
├── _layouts/
│   └── default.html          # Page layout and inline CSS
├── _data/
│   └── publications.yml      # Publications data (YAML)
├── _includes/
│   └── publications.html     # Publications rendering template
├── _config.yml               # Jekyll configuration
└── Gemfile                   # Ruby dependencies
```

---

## Acknowledgments

The visual design of this template is inspired by [Kaiming He's personal homepage](https://people.csail.mit.edu/kaiming/).

## License

This template is provided under the **MIT License**. See [LICENSE](LICENSE) for details.
