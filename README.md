**jsonc is a JSON compression library**


## Installation
    
To install jsonc, use [npm](http://github.com/isaacs/npm):

        $ npm install jsonc

## Usage

```coffee-script
jsonc = require '../lib/main.coffee'

list = []
list.push {my: 'choni', your: 'chachi', his: 'chocha', her: 'choochi'}
list.push {my: 'chooni', your: 'chaachi', his: 'choocha', her: 'chooochi'}
list.push {my: 'choooni', your: 'chaaachi', his: 'chooocha', her: 'choooochi'}
console.log 'Original: ' + JSON.stringify list

packed = jsonc.pack list
console.log 'Packed: ' + JSON.stringify packed

unpacked = jsonc.unpack packed
console.log 'Unpacked: ' + JSON.stringify unpacked
```

## Examples

You can view further examples in the [example folder.](https://github.com/wearefractal/jsonc/tree/master/examples)

## LICENSE

(MIT License)

Copyright (c) 2011 Fractal <contact@wearefractal.com>

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
