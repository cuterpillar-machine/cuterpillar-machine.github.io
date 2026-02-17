# Project TODO List

This list contains tasks and ideas for the Cuterpillar machine project, categorized by priority and type.

## 🛠 What Should Be Fixed
- [ ] **License File**: The repository is missing a clear `LICENSE` file. This should be added to clarify how others can use the code.
- [ ] **Security Policy**: Create a `security.txt` file (according to RFC 9116) and a `SECURITY.md` to define how to report vulnerabilities.
- [ ] **Google Analytics Version**: The `_includes/footer.html` uses an older `analytics.js` snippet, but `_config.yml` provides a `G-` ID (Google Analytics 4). This should be updated to use the `gtag.js` snippet for GA4 compatibility.
- [ ] **Favicon Paths**: Verify if all favicon sizes defined in `_config.yml` and `head.html` actually exist in the `assets/` directory (e.g., check for 128x128, 192x192, etc.).
- [ ] **Documentation Links**: Ensure all links to documentation pages are consistent. For example, check if `documentation/how-to-update-instructions` needs the `.html` extension in all environments.
- [ ] **Empty Meta Tags**: In `_config.yml`, some Facebook meta tags (like `app_id`, `publisher`, `admins`) are empty and might cause warnings in SEO crawlers.

## ⚙️ Can Be Changed / Improved
- [ ] **Contribution Guidelines**: Add a `CONTRIBUTING.md` file to help new contributors get started with the project.
- [ ] **SEO Enhancements**: Improve the `jekyll-seo-tag` configuration in `_config.yml` to include more specific social media metadata.
- [ ] **Sitemap**: Generate and optimize `sitemap.xml` for better search engine indexing.
- [ ] **Social Sharing Images**: Ensure that `og:image` and `twitter:image` are properly configured and point to high-quality preview images.
- [ ] **Responsive Tables**: Improve the responsiveness of the versions table on very small screens.
- [ ] **Version History Sorting**: Ensure the version history table in `versions.html` always sorts by date correctly, even if dates are missing or formatted differently.
- [ ] **Tailwind Optimization**: Review `tailwind.config.js` to ensure only used styles are included in the final build (purge/content configuration).
- [ ] **Breadcrumbs**: Add breadcrumb navigation to `_layouts/documentation.html` and `_layouts/version.html` to help users navigate back to the main lists.
- [ ] **RSS Feed for Versions**: Implement an RSS feed specifically for project version updates.
- [ ] **Localization (i18n)**: Implement multi-language support to make the documentation accessible to a global audience.

## ✨ Nice To Have
- [ ] **Automated Testing**: Add a basic test suite (e.g., using GitHub Actions and a link checker) to verify that no broken links are introduced.
- [ ] **Dark Mode Flash Prevention**: Currently, the theme script is at the bottom of the body. Moving the initial theme check to the head could prevent a flash of unstyled content (FOUC) when loading the page in dark mode.
- [ ] **Search Functionality**: Implement a simple client-side search (like Lunr.js or Simple-Jekyll-Search) to help users find documentation quickly.
- [ ] **LLM Instructions**: Add a `llm-instructions.md` (or similar) file to provide context and instructions for AI-based coding assistants.
- [ ] **Version Comparison**: Add a feature to see what changed between the latest version and the previous one directly on the versions page.
- [ ] **Dockerization**: Add a `Dockerfile` and `docker-compose.yml` for easier local development and deployment.

## 💡 Ideas
- [ ] **Analytics Dashboard**: Set up a simple dashboard (e.g., Google Search Console) to monitor site performance and search visibility.
- [ ] **Interactive Getting Started Guide**: Create an interactive or step-by-step guide for new users on the home page.
- [ ] **Newsletter**: Add an email subscription form for users who want to be notified of new releases via email.
- [ ] **Blog Section**: Add a blog section to share news, updates, and deep dives into the Cuterpillar machine project.
- [ ] **Community Showcase**: Add a section where users can submit and show off how they are using Cuterpillar machine.
- [ ] **Discord/Slack Integration**: Add a link to a community chat platform for real-time support and discussion.
