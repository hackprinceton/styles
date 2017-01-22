# hp-styles
Shared Sass stylesheets for HackPrinceton websites. This package may be loaded in two different ways:

## Via Git submodule
Use this method if installing into a GitHub Pages site.

```
git submodule add git@github.com:princetoneclub/hp-styles.git _sass/hp-styles
```

This installs a copy of the repo at `_sass/hp-styles`. Import these styles using the following lines:

```
@import 'hp-styles/settings';
@import 'hp-styles/mixins';
```

## Via NPM dependency
Use this method if installing into a Meteor site.

```
npm install --save git+https://github.com/princetoneclub/hp-styles.git
```

This installs this repo as a NPM package. Import these styles into a Meteor site using these lines:

```
@import '{}/node_modules/hp-styles/settings';
@import '{}/node_modules/hp-styles/mixins';
```
