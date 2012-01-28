node-bindings
=============
### Helper module for loading your native module's bindings in a cross-platform way.

This is a helper module for authors of native addon node.js modules. In node >=
0.7.0, it is encouraged to statically precompile your native addons for your
various supported platforms and architectures, rather than depend on the users to
do that. This adds an additional burden on the developer since we now have to
compile the bindings ourselves, before publishing the module. We also have to
figure out which version of the bindings to load at runtime, and that's where
`node-bindings` comes into play.

This module solves the organizational problem of how to store these bindings files
with a simple directory convention:

```
<module root>/compiled/<platform>/<arch>/<node_version>/bindings.node
```


Installation
------------

Install with `npm`:

``` bash
$ npm install bindings
```


Example
-------

``` js
```


License
-------

(The MIT License)

Copyright (c) 2012 Nathan Rajlich &lt;nathan@tootallnate.net&gt;

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
