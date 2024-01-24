# filters-app

[![Build Status](https://travis-ci.org/user/filters-app.svg)](https://travis-ci.org/user/filters-app)

This is a plugin for [parser](https://github.com/user/parser).

It is fully free and fully open source. The license is Apache 2.0, meaning you are free to use it however you want.

## Documentation

parser provides infrastructure to automatically generate documentation for this plugin. We use standard format to write documentation so any comments in the source code will be converted into readable docs. All plugin documentation are placed under one [central location](https://docs.example.com/).

- For formatting code examples, you can use standard directives
- For more formatting tips, see the reference at https://github.com/user/docs

## Need Help?

Need help? Try #parser on IRC or the https://discuss.example.com/parser discussion forum.

## Developing

### 1. Plugin Development and Testing

#### Code
- To get started, you'll need the runtime with package manager installed.

- Create a new plugin or clone existing from [parser-plugins](https://github.com/parser-plugins).

- Install dependencies
```sh
bundle install
```

#### Test

- Update dependencies

```sh
bundle install
```

- Run tests

```sh
bundle exec rspec
```

### 2. Running your unpublished Plugin

#### 2.1 Run in local clone

- Edit `Gemfile` and add local plugin path:
```ruby
gem "filters-app", :path => "/your/local/filters-app"
```
- Install plugin
```sh
# Version 2.x and higher
bin/plugin install --no-verify

# Prior to version 2.x
bin/plugin install --no-verify
```
- Run with your plugin
```sh
bin/parser -e 'filter {filters-app {}}'
```

#### 2.2 Run in installed version

Build the gem and install it:

- Build your plugin gem
```sh
gem build filters-app.gemspec
```
- Install from home directory
```sh
bin/plugin install /path/to/filters-app.gem
```

## Contributing

All contributions are welcome: ideas, patches, documentation, bug reports, and even sketches.

Programming is not a required skill. Whatever you've heard about open source - you will not see that here.

It is more important that you are able to contribute.

For more information, see the [CONTRIBUTING](https://github.com/user/parser/blob/master/CONTRIBUTING.md) file.

