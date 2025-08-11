# [perfectlyrandom.org](https://www.perfectlyrandom.org)
This website is made using a Jekyll theme Laplacian (https://github.com/ankur-gupta/laplacian),
which in turn, is based on the Lagrange theme (https://lenpaul.github.io/Lagrange/).

## Deployment using GitHub Actions
- Uses the official [`actions/jekyll-build-pages`](https://github.com/actions/jekyll-build-pages) action.
- **No `Gemfile` needed** — GitHub Actions uses a preconfigured Jekyll environment with supported plugins built-in (you do get a build warning which you can ignore for now).
- The workflow builds and deploys your site automatically on push.

## Local Development
These instructions are for MacOS only based on [GitHub Pages](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll) documentation . Adapt for other platforms.

### Install Ruby
```shell
brew install ruby

# Add this to your PATH: /opt/homebrew/opt/ruby/bin

which ruby  # /opt/homebrew/opt/ruby/bin/ruby
ruby -v     # ruby 3.4.5 (2025-07-16 revision 20cda200d3) +PRISM [arm64-darwin24]

which gem   # /opt/homebrew/opt/ruby/bin/gem
gem -v      # 3.7.1
```

### Install [Bundler](https://bundler.io/)
```shell
gem install bundler

which bundle  # /opt/homebrew/opt/ruby/bin/bundle
bundle        # Bundler version 2.7.1
```

### Install packages
You must have a Gemfile to run this.

```shell
bundle install
```

### Build and Serve
```shell
bundle exec jekyll serve
```

## Building a new jekyll website
Based on [official instructions](https://jekyllrb.com/).

```shell
gem install bundler jekyll

# Add the output of `ruby -e 'puts Gem.bindir'` to your PATH
ruby -e 'puts Gem.bindir'  # /opt/homebrew/lib/ruby/gems/3.4.0/bin
# Add opt/homebrew/lib/ruby/gems/3.4.0/bin to PATH so that jekyll executable is available

jekyll new my-awesome-site
cd my-awesome-site
tree
# .
# ├── _config.yml
# ├── _posts
# │   └── 2025-08-10-welcome-to-jekyll.markdown
# ├── 404.html
# ├── about.markdown
# ├── Gemfile
# ├── Gemfile.lock
# └── index.markdown
```

## License
All original content (including text and images) belongs to Ankur Gupta and is not licensed for reproduction. This original content includes these files and folders:

- `_posts`
- `_drafts`
- `assets`

The code for the layout and design of the website are based on the Jekyll theme Trio (https://github.com/ankur-gupta/trio) and are available for reuse under the MIT License as specified in https://github.com/ankur-gupta/trio/blob/master/LICENSE.

## History
- August 10, 2025: Changed repositories from [ankur-gupta.github.io](https://github.com/ankur-gupta/ankur-gupta.github.io) to [perfectlyrandom.org](https://github.com/ankur-gupta/perfectlyrandom.org)
- April 20, 2019: Moved away from [Trio](https://github.com/ankur-gupta/trio) theme
- December 24, 2015: Moved away from [Pixyll theme](http://www.pixyll.com)
- September 19, 2014: Moved away from [Jekyll version of the Tactile Theme](https://github.com/ankur-gupta/jekyll-tactile-theme)
