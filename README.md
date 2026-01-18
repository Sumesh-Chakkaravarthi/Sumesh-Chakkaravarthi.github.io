# Sumesh Chakkaravarthi Portfolio

A personal portfolio website built with Jekyll, featuring a modern dark theme with purple/indigo accents.

## Local Development

### Prerequisites
- Ruby (version 2.7 or higher)
- Bundler gem

### Setup

1. **Install Ruby dependencies:**
   ```bash
   cd /Users/sumesh/Projects/Antigravity/sumesh.github.io
   bundle install
   ```

2. **Run the development server:**
   ```bash
   bundle exec jekyll serve
   ```

3. **Open in browser:**
   Navigate to `http://localhost:4000`

### Live Reload (Optional)
For automatic page refresh on changes:
```bash
bundle exec jekyll serve --livereload
```

## Project Structure

```
sumesh.github.io/
├── _config.yml          # Jekyll configuration
├── _data/
│   └── site.yml         # Site metadata (name, email, etc.)
├── _includes/
│   ├── nav.html         # Navigation component
│   └── footer.html      # Footer component
├── _layouts/
│   └── default.html     # Base layout template
├── _work/               # Work experience entries
│   ├── 2025-power-of-patients.md
│   └── 2022-cisco-aicte.md
├── _projects/           # Project entries
│   ├── university-explorer-ai.md
│   ├── traffic-stop-disparity.md
│   └── time-series-forecasting.md
├── assets/
│   └── css/
│       └── main.css     # Stylesheet
├── index.html           # Homepage
├── about.html           # About page
├── experience.html      # Experience page
├── projects.html        # Projects page
├── Gemfile              # Ruby dependencies
└── README.md            # This file
```

## Adding Content

### Add New Work Experience
Create a new markdown file in `_work/`:
```yaml
---
title: "Job Title"
company: "Company Name"
location: "City, State"
period: "Start – End"
order: 1  # Lower number = appears first
tech:
  - Technology1
  - Technology2
---

- Bullet point 1
- Bullet point 2
```

### Add New Project
Create a new markdown file in `_projects/`:
```yaml
---
title: "Project Name"
summary: "Brief description"
icon: "🤖"
period: "Start – End"
order: 1
tech:
  - Technology1
  - Technology2
---

- Detailed description point 1
- Detailed description point 2
```

## Deployment

This site is designed to be deployed on GitHub Pages:

1. Push to a repository named `sumesh.github.io`
2. GitHub Pages will automatically build and deploy

## Technologies

- **Jekyll** - Static site generator
- **HTML/CSS** - Markup and styling
- **Google Fonts (Inter)** - Typography
