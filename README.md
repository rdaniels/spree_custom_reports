SpreeCustomReports
==================

Introduction goes here.

## Installation

1. Add this extension to your Gemfile with this line:

  ```ruby
  gem 'spree_custom_reports', github: 'engarcia/spree_custom_reports', branch: '3-0-stable'
  ```
  or
  ```ruby
  gem 'spree_custom_reports', github: 'engarcia/spree_custom_reports', branch: '3-4-stable'
  ```

  The `branch` option is important: it must match the version of Spree you're using.
  For example, use `3-0-stable` if you're using Spree `3-0-stable` or any `3.0.x` version.

2. Copy & run migrations
  ```ruby
  bundle exec rails g spree_custom_reports:install
  ```

3. Restart your server

  If your server was running, restart it so that it can find the assets properly.

## Testing

First bundle your dependencies, then run `rake`. `rake` will default to building the dummy app if it does not exist, then it will run specs. The dummy app can be regenerated by using `rake test_app`.

```shell
bundle
bundle exec rake
```

When testing your applications integration with this extension you may use it's factories.
Simply add this require statement to your spec_helper:

```ruby
require 'spree_custom_reports/factories'
```

Copyright (c) 2017 Enrique Garcia C, released under the New BSD License
