---
layout: default
title: How to Update Instructions
---

# How to Update Instructions

Keeping your Cuterpillar machine up to date is essential for stability and access to the latest features. Follow these general steps to update your installation.

## General Update Procedure

1.  **Backup your configuration:** Before updating, always back up your `_config.yml` and any custom assets.
2.  **Download the latest version:** Go to the [Versions page]({{ '/versions.html' | relative_url }}) and download the latest release archive.
3.  **Extract the archive:** Overwrite the existing files in your project directory with the contents of the new archive.
4.  **Install dependencies:** Run `bundle install` to ensure all required Ruby gems are up to date.
5.  **Verify configuration:** Check if there are any new configuration options required in `_config.yml` by referring to the [Setup Instructions]({{ '/setup-instructions.html' | relative_url }}).
6.  **Build and Serve:** Run `bundle exec jekyll serve` to verify that the site builds correctly.
