# gulp-html-inline

[![NPM version][npm-image]][npm-url]
[![Downloads][downloads-image]][downloads-url]
![cise](http://cise.alibaba-inc.com/task/69703/status.svg)

[npm-image]: https://img.shields.io/npm/v/gulp-htmlone.svg?style=flat-square
[npm-url]: https://npmjs.org/package/gulp-htmlone
[downloads-image]: http://img.shields.io/npm/dm/gulp-htmlone.svg?style=flat-square
[downloads-url]: https://npmjs.org/package/gulp-htmlone

combo and minify `css` and `js` to html. no matter the file is online or not.

## Features

+ css, js�Զ�����
+ css��js ѡ����ѹ��
+ ֧�� ���ò���Ҫcombine��������Դ�������滻����

## Usage

```javascript
var gulp = require('gulp');
var htmlInline = require('gulp-html-inline');

gulp.src('inline.html')
    .pipe(htmlInline({ minifyCss: false, minifyJs: true }))
    .pipe(gulp.dest('dist'));
```

## Options
```javascript
gulp.src('./src/*.html')
        .pipe(htmlInline({
            minifyCss: true, // �Ƿ���Ҫѹ��css
            minifyJs: true  // �Ƿ���Ҫѹ��js
        }))
// ...
```

#License
ISC
