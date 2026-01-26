# EduGrid Website

This is the Jekyll-based website for the EduGrid renewable energy education project.

## Setup

1. Install Ruby and Bundler
2. Run `bundle install` to install dependencies
3. Run `bundle exec jekyll serve` to start the development server
4. Visit `http://localhost:4000` to view the site

## Project Structure

```
├── _config.yml          # Jekyll configuration
├── _layouts/            # Page layouts
├── _includes/           # Reusable components (header, footer)
├── _team/              # Team member profiles
├── _publications/      # Publications collection
├── assets/
│   ├── css/            # Stylesheets
│   └── images/         # Images and media
├── index.md            # Home page
├── about.md            # About page
├── team.md             # Team page
├── resources.md        # Resources page
├── contact.md          # Contact page
└── tasks.json          # Task tracking for website replication
```

## Task Tracking

The `tasks.json` file tracks progress on replicating content from www.edu-grid.org.

## Building

To build the site:

```bash
bundle exec jekyll build
```

The built site will be in the `_site` directory.

## Deployment

This site is configured for GitHub Pages and will automatically deploy when pushed to the main branch.
