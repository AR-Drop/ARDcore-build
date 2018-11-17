# ARDcore-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install ARDcore-build
```

and use and require in your gulp file:

```javascript
var gulp = require('gulp');
var ARDcoreTasks = require('ARDcore-build');

ARDcoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var ARDcoreTasks = require('ARDcore-build');
ARDcoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/wkibbler/ARDcore) on the main ravencore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/wkibbler/ARDcore/blob/master/LICENSE).

