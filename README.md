# {{not}} [![NPM version](https://badge.fury.io/js/handlebars-helper-not.png)](http://badge.fury.io/js/handlebars-helper-not)

> {{not}} handlebars helper, for retrieving a value from your project's package.json.

## Overview
Conditionally render a block if the condition is false. This block helper is really just a semantic alternative to `{{#isnt}}`:

```handlebars
{{#not basename "index"}}
  <title>{{title}} | Assemble</title>
  {{else}}
  <title>Assemble</title>
{{/not}}
```

Please [report any bugs or feature requests](https://github.com/helpers/handlebars-helper-not/issues/new), thanks!

## Quickstart
Install the helper with: `npm install handlebars-helper-not`

### Assemble config
If you use [Assemble config](http://assemble.io) and Grunt, in your Gruntfile simply add `handlebars-helper-not` to the `helpers` property in the [Assemble](http://assemble.io) task or target options:

```javascript
grunt.initConfig({
  assemble: {
    options: {
      // the 'handlebars-helper-not' module must also be listed in devDependencies
      // for assemble to automatically resolve the helper
      helpers: ['handlebars-helper-not', 'foo/*.js']
    }
    ...
  }
});
```
Alternatively, you can register the helper with Assemble by adding `handlebars-helper-not` to both the `devDependencies` and the `keywords` array in your project's package.json.

_Note that the 'handlebars-helper-not' module **must be listed in both devDependencies and the keywords array** for Assemble to automatically resolve the helper._

You can now use begin using the helper in your templates.

## Author

**Jon Schlinkert**

+ [github/Jon Schlinkert](http://github.com/Jon Schlinkert)
+ [twitter/Jon Schlinkert](http://twitter.com/Jon Schlinkert)

## License and Copyright

Licensed under the [MIT License](./LICENSE-MIT)
Copyright (c) Jon Schlinkert, contributors.