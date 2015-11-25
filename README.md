# electron-installer-run [![travis][travis_img]][travis_url] [![npm][npm_img]][npm_url] [![][inch_img]][inch_url]

> Run child processes safely handling all sorts of edge cases.

## Example

```javascript
var run = require('electron-installer-run');
var args = ['--verify', process.env.APP_PATH];
run('codesign', args, function(err){
  if(err){
    console.error('codesign verification failed!');
    process.exit(1);
  }
  console.log('codesign verification succeeded!');
});
```

## License

Apache 2.0

[travis_img]: https://img.shields.io/travis/mongodb-js/electron-installer-run.svg
[travis_url]: https://travis-ci.org/mongodb-js/electron-installer-run
[npm_img]: https://img.shields.io/npm/v/electron-installer-run.svg
[npm_url]: https://npmjs.org/package/electron-installer-run
[inch_img]: http://inch-ci.org/github/mongodb-js/electron-installer-run.svg?branch=master
[inch_url]: http://inch-ci.org/github/mongodb-js/electron-installer-run
