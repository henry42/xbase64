xbase64
=======

## Basics

xbase64 is a fast javascript base64 encoder and decoder;

## Is it the fastest?

As far as I know it's fast enough. Although it depends on far too many variables to enumerate, I wrote a test, the result below is for reference.
Tell me if you know a faster one.

------ Chrome ( 1000 TIMES ) ------

BASE64 encode from https://github.com/mshang/base64-js costs 604
BASE64 encode from https://github.com/dankogai/js-base64 costs 4
BASE64 encode from https://github.com/carlo/jquery-base64 costs 24
xbase64 encode time costs 4
BASE64 decode from https://github.com/mshang/base64-js costs 250
BASE64 decode from https://github.com/dankogai/js-base64 costs 10
BASE64 decode from https://github.com/carlo/jquery-base64 costs 51
xbase64 decode time costs 6

------ IE6 ( 10 TIMES ) ------

BASE64 encode from https://github.com/mshang/base64-js costs 109
BASE64 encode from https://github.com/dankogai/js-base64 costs 32
BASE64 encode from https://github.com/carlo/jquery-base64 costs 15
xbase64 encode time costs 32
BASE64 decode from https://github.com/mshang/base64-js ERROR
BASE64 decode from https://github.com/dankogai/js-base64 costs 15
BASE64 decode from https://github.com/carlo/jquery-base64 costs 16
xbase64 decode time costs 15

------ IE9 ( 1000 TIMES ) -----

BASE64 encode from https://github.com/mshang/base64-js costs 3497
BASE64 encode from https://github.com/dankogai/js-base64 costs 2
BASE64 encode from https://github.com/carlo/jquery-base64 costs 1797
xbase64 encode time costs 11
BASE64 decode from https://github.com/mshang/base64-js costs 1316
BASE64 decode from https://github.com/dankogai/js-base64 costs 18
BASE64 decode from https://github.com/carlo/jquery-base64 costs 1700
xbase64 decode time costs 15


## Why use XBase64

It is fast.
It supports Unicode Characters. ( to UTF-8 )

## Usage

```js

XBase64.encode('hello world');
XBase64.decode('aGVsbG8gd29ybGQ=');

```

## See Also
[http://en.wikipedia.org/wiki/Utf8](http://en.wikipedia.org/wiki/Utf8)
[https://developer.mozilla.org/en-US/docs/Web/API/window.btoa](https://developer.mozilla.org/en-US/docs/Web/API/window.btoa)
