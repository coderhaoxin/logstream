logfilestream [![Build Status](https://secure.travis-ci.org/fengmk2/logstream.png)](http://travis-ci.org/fengmk2/logstream) [![Coverage Status](https://coveralls.io/repos/fengmk2/logstream/badge.png)](https://coveralls.io/r/fengmk2/logstream)
=========

[![NPM](https://nodei.co/npm/logfilestream.png?downloads=true&stars=true)](https://nodei.co/npm/logfilestream)

![logo](https://raw.github.com/fengmk2/logstream/master/logo.png)

Log file stream, including auto rolling feature, support multiprocess `append` write at the same time.

## Install

```sh
$ npm install logfilestream
```

## Usage

```js
var writestream = logfilestream({
  logdir: '/tmp/logs',
  nameformat: '[info.]YYYY-MM-DD[.log]'
});

writestream.write('hello');
writestream.write(' world\n');
writestream.end();
```

## License

(The MIT License)

Copyright (c) 2012 - 2013 fengmk2 <fengmk2@gmail.com>.

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
