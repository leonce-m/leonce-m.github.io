# Leonce Mollerus GitHub Pages Site

Personal portfolio site built with Jekyll and the Minimal Mistakes remote theme. The site highlights robotics, autonomous racing, graph-based SLAM, embedded systems, and selected project work.

## Local Preview

Install the Ruby dependencies:

```sh
bundle install
```

Run the local Jekyll server:

```sh
bundle exec jekyll serve --host 0.0.0.0 --port 4000
```

Then open:

```text
http://localhost:4000
```

## Content Structure

- `index.md` - homepage with video hero and selected featured projects
- `projects.md` - project overview page
- `projects/` - individual project pages
- `_data/projects.yml` - canonical project card metadata
- `_includes/project-grid.html` - reusable project card grid
- `assets/images/` - project images and page visuals
- `assets/videos/` - optimized homepage video loops
- `assets/css/main.scss` - theme import and local custom styles
