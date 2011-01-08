XUI
===

A lightweight, dead simple, micro-tiny, super modular JavaScript framework for building mobile web applications. Its true: the minified code is _super tiny_. You can find more information, downloads and documentation on the [http://xuijs.com](http://xuijs.com).

If you want to build your own custom XUI or help contribute: please read on! The best documentation is in the source and the tests.

Building XUI
------------

To get the full source you need  _Git_:

    $ git clone git://github.com/xui/xui.git
    $ cd xui
    $ git submodule init
    $ git submodule update

To build XUI, you will need _Ruby_:

    $ ./build                 # Generates lib/xui.js
    $ ./build profile=bb      # Builds XUI for BlackBerry 4/5 browsers (uses Sizzle selector engine)
    $ ./build profile=ie      # Builds XUI for Internet Explorer

Source Tree
-----------

    xui
     |-README.md ................ You are reading it!
     |
     |-lib ...................... Build directory (generated by build script)
     | |-xui.js ................. Core XUI - optimized for standards-friendly browsers, i.e. webkit
     | |-xui-bb.js .............. BlackBerry implementation
     | '-xui-ie.js .............. Internet Explorer implementation
     |
     |-packages ................. Third-party libs utilized by XUI (gitsubmodules)
     | |-qunit ..................   - awesome async friendly test lib by John Resig
     | |-emile ..................   - amazing tiny effects lib by Thomas Fuchs
     | |-sizzle .................   - kickass selector engine that powers jQuery, by John Resig.
     | '-split.js ...............   - override IE bad implementation of String.split
     |
     |-spec ..................... The spec
     | |-index.html ............. Open to run the spec
     |
     |-src
     | |-base.js ................ Bare essentials for dom node retrieval
     | |
     | |-js ..................... Essentials:
     | | |-dom.js ...............   - dom node manipulation
     | | |-event.js .............   - event subscribe/publish
     | | |-fx.js ................   - animation
     | | |-style.js .............   - css hackery
     | | '-xhr.js ...............   - remoting
     | |
     | '-ie
     |   |-dom.js
     |   |-event.js
     |   |-style.js
     |
     '-util ..................... Utils for minification, obfuscation, verification

Creators
--------

- http://github.com/brianleroux
- http://github.com/silentrob
- http://github.com/sintaxi


Contributors
------------

- http://github.com/rmurphey 
- http://github.com/remy
- http://github.com/filmaj
- http://github.com/alunny
- http://github.com/gdagley
- http://github.com/slexaxton
- http://github.com/cluster
- http://github.com/joemccann
- http://github.com/mwbrooks

(If we missed you, please let us know!)

License
-------

_Copyright (c) 2008, 2009, 2010 Brian LeRoux, Brock Whitten, Rob Ellis_

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be included
in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
