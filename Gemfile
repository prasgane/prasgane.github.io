source "https://rubygems.org"

# GitHub Pages manages Jekyll and all core plugin versions.
# To upgrade, run: bundle update github-pages
gem "github-pages", group: :jekyll_plugins

# Required for Jekyll 4.x on Ruby 3.x (removed from stdlib in Ruby 3.0)
gem "webrick", "~> 1.8"

group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
  gem "jekyll-paginate"
  gem "jekyll-seo-tag"
  gem "jekyll-sitemap"
end

# Windows/JRuby timezone support — tzinfo 2.x fixes CVE-2022-31163
install_if -> { RUBY_PLATFORM =~ %r!mingw|mswin|java! } do
  gem "tzinfo", "~> 2.0"
  gem "tzinfo-data"
end

# Performance booster for watching directories on Windows
gem "wdm", "~> 0.1.1", :install_if => Gem.win_platform?
