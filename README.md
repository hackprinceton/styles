# hp-styles
Shared Sass stylesheets for HackPrinceton websites. This package may be loaded in two different ways:

## Via Git submodule
Use this method if installing into a GitHub Pages site.

```
git submodule add https://github.com/hackprinceton/styles.git _sass/hp-styles
```

This installs a copy of the repo at `_sass/hp-styles`. Import these styles using the following lines:

```
@import 'hp-styles/settings';
@import 'hp-styles/mixins';
```

## Via NPM dependency
Use this method if installing into a Meteor site.

```
npm install --save git+https://github.com/hackprinceton/styles.git
```

This installs this repo as a NPM package. Import these styles into a Meteor site using these lines:

```
@import '{}/node_modules/hp-styles/settings';
@import '{}/node_modules/hp-styles/mixins';
```

On Rails, the following needs to be added to the Gemfile:

```ruby
gem 'browserify-rails', '~> 4.2'
gem 'foundation-rails', '~> 5.5'
```

Then, run the following:

```sh
$ bin/rails generate foundation:install
$ bin/rails yarn:install
```

And add the following to `app/assets/stylesheets/application.scss`:

```scss
@import "hp-styles/settings";
@import "foundation";
```
