## contentful-jekyll
This is a proof of concept static site, generated with [Jekyll](https://jekyllrb.com) using [Contentful](https://app.contentful.com) as a CMS.

## build
- `cp .env.example .env`
- update `.env` with Contentful `space` and `access` tokens
- `bundle exec jekyll serve`

## fetching content
Using Contentful's [jekyll data importer](https://github.com/contentful/jekyll-contentful-data-import) gem

- `jekyll contentful`
