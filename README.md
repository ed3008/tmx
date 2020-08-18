# Tamex
TAMEX is an e-commerce platform dedicated to sell and distribution of electric material, lightning, control and distribution.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![CircleCI](https://circleci.com/gh/magma-labs/tamex.svg?style=svg)](https://circleci.com/gh/magma-labs/tamex)

# Development

## Prerequisites

- **ruby 2.4.9**, if using OSX, rbenb + rbenv-build are recommended
- Java 8 (Following this [article](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html))
- Postgresql, if using OSX, PostgresApp is recomended
- Node 13.0.1
- Yarn 1.2.1

## Install the dependencies

```
bundle install
```

## Run database
Remember to create your own copy of `database.yml` from `database.yml.example`. To do that, run in your bash:

```
cp config/database.example.yml config/database.yml
```

To create database, first, please ensure you already completed previous step and after that run:

```ruby
bundle exec rake db:setup
bundle exec rake db:migrate
```

## Run solr
- To run `solr`, first, please ensure you already completed the installation of **java 8**.
- After you install `solr`, be sure to create your own copy of `config/schema.xml.example` to `solr/configsets/sunspot/conf/schema.xml`. To do that, run in your bash:

```
cp config/schema.xml.example solr/configsets/sunspot/conf/schema.xml
```

Now you can run `solr` by running:

```ruby
bundle exec rake sunspot:solr:run
```

You can check `solr` on:

```
http://localhost:8982
```

## Run the development seeds:

```ruby
AUTO_ACCEPT=true be rake db:seed --trace
bundle exec rake importer:seed_taxonomies
bundle exec rake importer:seed_products[products]
bundle exec rake importer:seed_images['lib/assets/tamex_images']
bundle exec rake sunspot:solr:reindex

```

## Running tests

```
rake
```
