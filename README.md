## contentful-jekyll
This is a proof of concept static site, generated with [Jekyll](https://jekyllrb.com) using [Contentful](https://app.contentful.com) as a CMS and [Glimmer](https://glimmerjs.com/) components.

## build
- `cp .env.example .env`
- update `.env` with Contentful `space` and `access` tokens
- `bundle exec jekyll serve`

## fetching content
Using Contentful's [jekyll data importer](https://github.com/contentful/jekyll-contentful-data-import) gem

- `jekyll contentful`

## glimmer component
[This](https://github.com/jonpitch/DemoGlimmer) is the dummy component.

As of this commit, the Glimmer publish strategy isn't crystal clear to me. For now:
- `yarn install`
- `cd node_modules/demo-glimmer`
- `yarn install && ember build --production`
- `cp -R dist/ ../../assets/demo-glimmer`

## testing
based off of [this article](https://jekyllrb.com/docs/continuous-integration/travis-ci/)

had to:
```
brew unlink xz
bundle install
brew link xz
```