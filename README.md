# Chulapa remote-theme example

This example uses [Chulapa v2.3.0](https://github.com/dieghernan/chulapa/releases/tag/v2.3.0)
through `jekyll-remote-theme`. Clone or fork this repository to reuse the example,
or use [Chulapa 101](https://github.com/dieghernan/chulapa-101/generate) for the
ready-to-publish blog template. For the RubyGems installation example, see
[chulapa-jekyll-gem](https://github.com/dieghernan/chulapa-jekyll-gem).

Contains basic configuration to get you a site with:

- [Sample posts](./_posts/) and [paginated blog index](./blog/index.html).
- [Sample collection](./_cheatsheet/) with Markdown and kramdown cheatsheets and [collection index](./_pages/cheatsheet.md).
- Archive pages for posts grouped by year, category, and tag.
- [GitHub Actions workflows](.github/workflows/) for deploying the site.
- Demo page with the different Bootstrap components and how they look with the actual skin settings.
- Sample 404 page.
- Site search with Lunr.
- Sample [`_config.yml`](_config.yml) with the pinned theme and optional settings.
- Atom, RSS and JSON Feed, with a subscription page at `/subscribe/`.
- Sample [`algolia-search.yml`](algolia-search.yml) for using Algolia+GitHub Actions. More guidance in the top of the file.
- Sample files for extending the theme with your [own scripts](./_includes/custom/) and [css](./assets/css/).

Edit your site details in `_config.yml` and replace the sample content.
Run `bundle install` and `bundle exec jekyll serve` to preview your site. To
upgrade the theme, change the tag on `remote_theme` and rebuild.
[Configuration reference](https://dieghernan.github.io/chulapa/docs/02-config)
