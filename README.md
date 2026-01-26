# EduGrid Website

> Renewable Energy Education Project Website

[![Built with Jekyll](https://img.shields.io/badge/Built%20with-Jekyll-blue)](https://jekyllrb.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## About

This is the official website for the EduGrid project - a pioneering renewable energy education initiative funded by the European Union's Horizon 2020 research and innovation programme. Our mission is to educate and empower students, educators, and communities about sustainable energy solutions.

## Features

- 📱 **Responsive Design**: Fully responsive layout that works on all devices
- 🎨 **Modern UI**: Clean and professional design with gradient hero sections
- 📝 **Blog System**: Built-in news and blog functionality
- 🔍 **SEO Optimized**: Meta tags and SEO plugin for better search visibility
- ⚡ **Fast Loading**: Optimized assets and efficient Jekyll build
- 🌐 **Easy Content Management**: Simple markdown-based content editing

## Site Structure

```
├── _config.yml           # Jekyll configuration
├── _layouts/             # Page layouts
│   ├── default.html      # Base layout
│   ├── page.html         # Standard page layout
│   └── post.html         # Blog post layout
├── _includes/            # Reusable components
│   ├── header.html       # Site header and navigation
│   └── footer.html       # Site footer
├── _posts/               # Blog posts
├── assets/               # Static assets
│   ├── css/              # Stylesheets
│   ├── js/               # JavaScript files
│   └── images/           # Images
├── index.md              # Homepage
├── about.md              # About page
├── project.md            # Project description
├── partners.md           # Partners page
├── news.md               # News listing page
└── contact.md            # Contact page
```

## Prerequisites

- Ruby 3.0 or higher
- RubyGems
- Bundler

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/maxhock/edu-grid.github.io.git
   cd edu-grid.github.io
   ```

2. **Install dependencies**
   ```bash
   # Install bundler if you don't have it
   gem install bundler

   # Install Jekyll and dependencies
   bundle config set --local path 'vendor/bundle'
   bundle install
   ```

## Development

### Run the development server

```bash
bundle exec jekyll serve
```

The site will be available at `http://localhost:4000`

### Run with live reload

```bash
bundle exec jekyll serve --livereload
```

### Build the site

```bash
bundle exec jekyll build
```

The built site will be in the `_site/` directory.

## Content Management

### Adding a New Blog Post

1. Create a new file in `_posts/` with the format: `YYYY-MM-DD-title.md`
2. Add frontmatter:
   ```yaml
   ---
   layout: post
   title: "Your Post Title"
   date: YYYY-MM-DD
   author: Author Name
   tags: [tag1, tag2, tag3]
   ---
   ```
3. Write your content in Markdown below the frontmatter

### Editing Pages

Simply edit the corresponding `.md` file in the root directory:
- `index.md` - Homepage
- `about.md` - About page
- `project.md` - Project description
- `partners.md` - Partners page
- `contact.md` - Contact page
- `news.md` - News listing page

### Customizing Styles

Edit the CSS file at `assets/css/main.css` to customize the appearance.

### Updating Navigation

Edit the `navigation` section in `_config.yml`:

```yaml
navigation:
  - title: Home
    url: /
  - title: About
    url: /about
  # Add more items...
```

## Configuration

Key settings in `_config.yml`:

- `title`: Site title
- `description`: Site description
- `url`: Production URL
- `navigation`: Menu items
- `social_links`: Social media links

## Deployment

### GitHub Pages

This site is designed to be deployed on GitHub Pages:

1. Push your changes to the `main` branch
2. GitHub Pages will automatically build and deploy the site
3. The site will be available at `https://maxhock.github.io/edu-grid.github.io/`

### Manual Deployment

1. Build the site: `bundle exec jekyll build`
2. Deploy the contents of `_site/` to your web server

## Task Tracking

See `replication_tasks.json` for the detailed task list and completion status.

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License.

## Acknowledgments

- Funded by the European Union's Horizon 2020 research and innovation programme
- Built with [Jekyll](https://jekyllrb.com/)
- Theme based on [Minima](https://github.com/jekyll/minima)

## Support

For questions or support, please [contact us](https://edu-grid.github.io/contact) or open an issue on GitHub.

---

**EduGrid Project** - Empowering the next generation through renewable energy education
