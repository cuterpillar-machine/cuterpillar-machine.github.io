# Cuterpillar machine

Visit our site https://cuterpillar-machine.github.io/

[![Support](https://img.shields.io/badge/Support-Project-orange)](https://cuterpillar-machine.github.io/support.html)

## Local Development

To run this website locally, you need to have Ruby and Jekyll installed.

### Prerequisites

- Ruby (version 3.0 or higher recommended)
- Bundler (`gem install bundler`)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/cuterpillar-machine/cuterpillar-machine.github.io.git
   cd cuterpillar-machine.github.io
   ```

2. Install dependencies:
   ```bash
   bundle install
   ```

### Running Locally

To start the Jekyll server locally:
```bash
bundle exec jekyll serve --incremental --trace
```

### Access the Site
Open your browser and navigate to:
[http://localhost:4000](http://localhost:4000)

## Maintenance

### Adding a New Version
You can add a new version using the GitHub Action "Add New Version":
1. Go to the **Actions** tab in the GitHub repository.
2. Select **Add New Version** workflow.
3. Click **Run workflow** and fill in the version details.
4. The action will automatically create the version and documentation files in both languages:
   `_versions/<version>.md` and `_documentations/<version>.md` (Ukrainian, from `description`) and
   `_versions/en/<version>.md` and `_documentations/en/<version>.md` (English, from `description_en`,
   falling back to `description`).

## Languages
The site is Ukrainian at `/` and English at `/en/`.
- UI strings live in `_data/i18n/uk.yml` and `_data/i18n/en.yml` (same keys in both).
- A page's language comes from `_config.yml` `defaults`: everything under `en/`, `_versions/en/` and `_documentations/en/` is English.
- Page markup lives once in `_includes/pages/`; `index.html` and `en/index.html` (and the other top-level pages) only set front matter.
- Translations of a page share a front matter `ref`; versions and documentations are matched by `version`.