gulp-node-webkit-builder
========================

![](http://img.shields.io/badge/npm_module-v1.0.0-green.svg?style=flat)  ![](http://img.shields.io/badge/dependencies-latest-yellowgreen.svg?style=flat)
![](http://img.shields.io/badge/build-passing-brightgreen.svg?style=flat)

Help developers build their own node-webkit apps for different platforms such as win, mac and linux with gulp.
## Information

<table>
<tr> 
<td>Package</td><td>gulp-node-webkit-builder</td>
</tr>
<tr>
<td>Description</td>
<td>A simple wrapper for `node-webkit-builder`</td>
</tr>
<tr>
<td>Node Version</td>
<td>>= 0.10</td>
</tr>
</table>

## Usage

```javascript
var builder = require('gulp-node-webkit-builder');

gulp.task('scripts', function() {
  return gulp.src(['./resources/**/*'])
    .pipe(builder({
        version: 'v0.9.2',
        platforms: ['win']
     }));
});

```

This will pass all the files into `node-webkit-builder`, and generate the `node-webkit` app.

## Options

All the options will be passed into `node-webkit-builder` directly except `files`.

For detail description, see: [Options](https://github.com/mllrsohn/node-webkit-builder/blob/master/README.md)


## LICENSE

[MIT License](http://en.wikipedia.org/wiki/MIT_License)
