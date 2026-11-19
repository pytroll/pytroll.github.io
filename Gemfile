source "https://rubygems.org"

# This site is built and deployed by the GitHub Actions workflow in
# .github/workflows/pages.yml using the versions locked in Gemfile.lock.
# Run `bundle update` to update them.
#
# Run Jekyll locally with `bundle exec`, like so:
#
#     bundle exec jekyll serve
#
gem "jekyll", "~> 4.4"

# Plugins listed here are loaded automatically by Jekyll. They are also listed
# under `plugins:` in _config.yml.
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.18"
  gem "jekyll-relative-links", "~> 0.9"
  gem "jekyll-remote-theme", "~> 0.6"
  gem "jekyll-seo-tag", "~> 2.9"
end

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
install_if -> { RUBY_PLATFORM =~ %r!mingw|mswin|java! } do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1.1", :install_if => Gem.win_platform?
