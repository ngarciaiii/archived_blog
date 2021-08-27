# frozen_string_literal: true

source "https://rubygems.org"

require 'json'
require 'open-uri'
versions = JSON.parse(open('https://pages.github.com/versions.json').read)

git_source(:github) {|repo_name| "https://github.com/#{repo_name}" }

# gem "rails"

gem 'jekyll-paginate'
gem 'github-pages', versions['']
gem 'kramdown', versions['kramdown']
gem 'rake'
gem 'jekyll-assets', group: :jekyll_plugins
gem "sprockets", "~> 3.7"

gem "webrick", "~> 1.7"
