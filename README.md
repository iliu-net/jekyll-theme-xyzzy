# xyzzy

Xyzzy is a geeky Jekyll theme for bloggers.

[Live preview](https://jonaskay.github.io/jekyll-theme-xyzzy/)

![xyzzy theme preview](/screenshot.png)

## Installation

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem "xyzzy"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: xyzzy
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install jekyll-theme-xyzzy

## Usage

Like Jekyll's default theme, [minima](https://raw.githubusercontent.com/jekyll/minima/), Xyzzy has been scaffolded by the `jekyll new-theme` command. You can have a new Jekyll site up and running with zero-configuration.

### Layouts

Refers to `.html` files within the `_layouts` directory.

  - `default.html` &mdash; The base layout that lays the foundation for subsequent layouts.
  - `home.html` &mdash; The layout for your index-page.
  - `page.html` &mdash; The layout for your documents that contain FrontMatter, but are not posts.
  - `post.html` &mdash; The layout for your posts.

### Includes

Refers to the `.html` files within the `_includes` directory.

  - `footer.html` &mdash; Defines the site's footer section.
  - `github-link.html` &mdash; Inserts GitHub link with icon
  - `google-analytics.html` &mdash; Inserts Google Analytics (active only in production environment).
  - `head.html` &mdash; Defines the `<head></head>` in *default* layout.
  - `header.html` &mdash; Defines the site's main header section.
  - `twitter-link.html` &mdash; Inserts Twitter link with icon

### Sass

Refers to `.scss` files within the `_sass` directory.
  - `xyzzy.scss` &mdash; The core file imported by preprocessed `styles.scss`; it defines the variable defaults and imports Sass partials.
  - `xyzzy/_base.scss` &mdash; Resets and defines base styles.
  - `xyzzy/_components.scss` &mdash; Defines component styles.
  - `xyzzy/_syntax.scss` &mdash; Defines syntax highlighting styles.
  - `xyzzy/_utility.scss` &mdash; Defines utility styles.
  - `xyzzy/layout/_article.scss` &mdash; Defines `article` layout styles.
  - `xyzzy/layout/_footer.scss` &mdash; Defines `footer` layout styles.
  - `xyzzy/layout/_header.scss` &mdash; Defines `header` layout styles.
  - `xyzzy/layout/_main.scss` &mdash; Defines `main` layout styles.
  - `xyzzy/layout/_nav.scss` &mdash; Defines `nav` layout styles.

### Assets

Refers to various asset files within the `assets` directory.

Contains the `styles.scss` that imports sass files from within the `_sass` directory. This `styles.scss` is what gets processed into the theme's main stylesheet `styles.css` called by `_layouts/default.html` via `_includes/head.html`.

TODO: Write usage instructions here. Describe your available layouts, includes, sass and/or assets.

### Enabling Google Analytics

To enable Google Anaytics, add the following lines to `_config.yml`:

```yaml
  google_analytics: UA-NNNNNNNN-N
```

Google Analytics will only appear in production, i.e., `JEKYLL_ENV=production`

## Contributing

Bug reports and pull requests are welcome on GitHub at <https://github.com/jonaskay/jekyll-theme-xyzzy>. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## Development

To set up your environment to develop this theme, run `bundle install`.

Your theme is setup just like a normal Jekyll site! To test your theme, run `bundle exec jekyll serve` and open your browser at `http://localhost:4000`. This starts a Jekyll server using your theme. Add pages, documents, data, etc. like normal to test your theme's contents. As you make modifications to your theme and to your content, your site will regenerate and you should see the changes in the browser after a refresh, just like normal.

When your theme is released, only the files in `_layouts`, `_includes`, `_sass` and `assets` tracked with Git will be bundled.
To add a custom directory to your theme-gem, please edit the regexp in `jekyll-theme-xyzzy.gemspec` accordingly.

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
