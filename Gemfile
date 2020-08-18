# frozen_string_literal: true

source 'https://rubygems.org'

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?('/')
  "https://github.com/#{repo_name}.git"
end

ruby '2.4.9'

gem 'rails'

gem 'autoprefixer-rails'
gem 'aws-sdk-s3', '~> 1.8.2'
gem 'bootstrap-sass'
gem 'browser'
gem 'coffee-rails'
gem 'conekta'
gem 'dalli'
gem 'data_migrate'
gem 'devise-i18n'
gem 'font-awesome-sass'
gem 'gibbon'
gem 'high_voltage'
gem 'jbuilder'
gem 'jquery-rails'
gem 'jquery-slick-rails'
gem 'modernizr-rails'
gem 'multi_fetch_fragments', github: 'akshay2408/multi_fetch_fragments'
gem 'newrelic_rpm', '4.0.0.332'
gem 'pg'
gem 'puma'
gem 'puma_worker_killer'
gem 'sass-rails'
gem 'sprockets-rails'
gem 'turbolinks'
gem 'uglifier'

gem 'rack-attack'
gem 'rack-canonical-hostname', require: 'rack/canonical_host'
gem 'rack-timeout', group: :production

gem 'solidus', github: 'solidusio/solidus'
gem 'solidus_auth_devise', github: 'solidusio/solidus_auth_devise'
gem 'solidus_i18n', github: 'solidusio-contrib/solidus_i18n'
gem 'solidus_import_products', github: '2BeDigital/solidus_import_products'
gem 'solidus_slider', github: 'jtapia/solidus_slider'
gem 'solidus_trackers', github: 'solidusio-contrib/solidus_trackers'
gem 'solidus_paypal_express', github: 'jtapia/better_solidus_paypal_express'
gem 'solidus_conekta', github: 'jtapia/solidus_conekta'
gem 'solidus_dynamic_sitemaps', github: 'jtapia/solidus_dynamic_sitemaps'
gem 'solidus_active_shipping', github: 'jtapia/solidus_active_shipping'
gem 'solidus_99minutos', github: 'magma-labs/solidus_99minutos', branch: 'check-for-blocked-account'
gem 'solidus_newsletter', github: 'jtapia/solidus_newsletter'
gem 'solidus_related_products', github: 'solidusio-contrib/solidus_related_products'
gem 'solidus_reviews', github: 'solidusio-contrib/solidus_reviews'
gem 'solidus_sale_prices', github: 'nebulab/solidus_sale_prices'
gem 'solidus_static_content', github: 'solidusio-contrib/solidus_static_content'
gem 'solidus_simple_dash', github: 'magma-labs/solidus_simple_dash'
gem 'solidus_mercado_pago', github: 'ngelx/solidus_mercado_pago'
gem 'solidus_print_invoice' , github: 'solidusio-contrib/solidus_print_invoice'
gem 'solidus_banorte_payworks', github: 'magma-labs/solidus_banorte_payworks'

gem 'sunspot_rails'

group :development, :test do
  gem 'capybara'
  gem 'factory_bot_rails'
  gem 'figaro'
  gem 'pry-rails'
  gem 'rspec-activemodel-mocks'
  gem 'rspec-rails'
  gem 'rspec_tap'
  gem 'rubocop', require: false
  gem 'selenium-webdriver'
end

group :test do
  gem 'database_cleaner'
  gem 'fixture_builder'
  gem 'shoulda-matchers'
  gem 'rails-controller-testing'
  gem 'simplecov', require: false
end

group :development do
  gem 'listen'
  gem 'spring'
  gem 'spring-watcher-listen'
  gem 'spring-commands-rspec'
  gem 'sunspot_solr', '2.2.8'
  gem 'reek', require: false
  gem 'web-console'
end

group :production do
  gem 'rails_12factor'
  gem 'rails_autoscale_agent'
end

# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]

gem 'derailed_benchmarks', group: :development
gem 'stackprof', group: :development
