![status](https://secure.travis-ci.org/kay-is/gulp-emblem-printer.svg?branch=master)

## Information

<table>
<tr>
<td>Package</td><td>gulp-emblem-printer</td>
</tr>
<tr>
<td>Description</td>
<td>Converts Emblem to Handlebars</td>
</tr>
<tr>
<td>Node Version</td>
<td>>= 0.10</td>
</tr>
<tr>
<td>Emblem Version</td>
<td>>= 0.5.0</td>
</tr>
</table>

## Usage

```js
var emblemPrinter = require('gulp-emblem-printer');

gulp.task('scripts', function() {
  return gulp.src('./lib/*.js')
    .pipe(emblemPrinter({
      extension:'.handlebars'
    }))
    .pipe(gulp.dest('./dist/'));
});
```

This will convert Emblem files to Handlebars files and replace their extension to .handlebars (.hbs is the default).


## LICENSE

(MIT License)

Copyright (c) 2015 Kay Plößer <k@kay.is>

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.