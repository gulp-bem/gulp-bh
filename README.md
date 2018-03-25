gulp-bh
=======

*DEPRECATED repository, moved to mono repository [gulp-bem](https://github.com/bem/gulp-bem/tree/master/packages/gulp-bh)*

Gulp plugin for executing [https://github.com/bem/bh](bh) templates.

```js
var gulp = require('gulp'),
    bh = require('@bem/gulp-bh')();

gulp.task('default', function() {
    gulp.src('*.bh.js')
        .pipe(bh.match());

    return gulp.src('index.bemjson.js')
        .pipe(bh.apply('index.html'))
        .pipe(gulp.dest('./bundle'));
});
```
