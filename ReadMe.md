## intro
[html-packer](https://github.com/Rozbo/html-packer.git) 's gulp support

## Install
```shell
npm install gulp-html-packer
```


## UseIt
```js
var gulp = require('gulp');
var packer = require('gulp-html-packer');

gulp.task('packer', function () {
    var options = {
        compress: false
    };

    return gulp.src('./src/*.html')
        .pipe(packer(options))
        .pipe(gulp.dest('./out'));
});
```