# css-boilerplate

Fixes to various browser quirks (mostly ie). Not meant to be a replacement for a css reset.


[![Build Status](https://secure.travis-ci.org/techjacker/css-boilerplate.png)](http://travis-ci.org/techjacker/css-boilerplate)

[![Sauce Labs Browser Test Status](https://saucelabs.com/buildstatus/css-boilerplate)](https://saucelabs.com/u/css-boilerplate)
[![Sauce Labs Browser Test Status](https://saucelabs.com/browser-matrix/css-boilerplate.svg)](https://saucelabs.com/u/css-boilerplate)


### Install

#### Node

```Shell
npm install css-boilerplate
```

#### Browser

```Shell
component install css-boilerplate
```


## Usage

#### css-boilerplate.mixinInstanceProps(class, [classes])

```JavaScript
var myStaticClass = {};

/* .mixinInstanceProps() */
mitsubishi.mixinInstanceProps(myStaticClass, [{hello:true}, {world:true}]);

console.log('myStaticClass', myStaticClass);
// outputs: {{hello:true, world:true}
```

#### css-boilerplate.mixinProtoProps(class, [classes])

```JavaScript
var myDynamicClass = function () {};
var parentDynamicClass = function () {};

parentDynamicClass.prototype.awesome = blah;

mitsubishi.mixinProtoProps(myDynamicClass, [(new parentDynamicClass), {world:true}]);

console.log('myDynamicClass', myDynamicClass);
// outputs: {{awesome:"blah", world:true}
```


### Docs
[Yuidocs documentation here](docs/index.html)
- fire up the connect server ```$ grunt docs```
- navigate your browser to the [docs](http://localhost:9001)


## License
Copyright (c) 2013 Andrew Griffiths <mail@andrewgriffithsonline.com>

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