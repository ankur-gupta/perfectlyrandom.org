## Local build Instructions
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
