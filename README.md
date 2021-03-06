Grapher [![Build Status](https://travis-ci.org/ayasdi/grapher.svg)](https://travis-ci.org/ayasdi/grapher)
==============
Draw network graphs using WebGL and Canvas backup.

Download
--------

* [grapher](http://ayasdi.github.io/grapher/build/grapher.js)
* [grapher-min](http://ayasdi.github.io/grapher/build/grapher-min.js)

Installing
----------

    npm install --save git://github.com/ayasdi/grapher.git


Additional Modules
------------------

Need a specific feature? Create your own modules for Grapher!
Here are some modules we've made:

* [center](https://github.com/ayasdi/grapher-center):
    Helpful functions for centering the graph.
* [palette](https://github.com/ayasdi/grapher-palette):
    Set up custom palettes and set colors by palette indices.
* [target](https://github.com/ayasdi/grapher-target):
    Target a node or link, or find the nearest nodes and links.
* [zoom](https://github.com/ayasdi/grapher-zoom):
    Zoom adjusts Grapher's scale by ratio. Optionally target a point as the zoom center.

Examples
--------

Here are a few examples:

1. [Simple](http://ayasdi.github.io/grapher/examples/1-simple.html)
2. [Transforms](http://ayasdi.github.io/grapher/examples/2-transforms.html)
3. [Colors](http://ayasdi.github.io/grapher/examples/3-colors.html)
4. [Drag](http://ayasdi.github.io/grapher/examples/4-drag.html)
5. [Pan](http://ayasdi.github.io/grapher/examples/5-pan.html)
6. [Force (using d3's force layout)](http://ayasdi.github.io/grapher/examples/6-force.html)

These examples can be also found in the examples folder.

Developing
----------

**Installing**

Grapher uses [Node.js](http://nodejs.org/). Install Node.js then run the following command:

    npm install

This will install the development dependencies that Grapher uses to run its various tasks.

**Building**

To build Grapher, run the build script:

    npm run build

This will bundle modules/grapher.js with its dependencies and outputs the result to
grapher.js and grapher-min.js in the build folder. The build script also gets run 
during tests and in preversion.

**Testing**

Unit tests are run using Jasmine with this command:

    npm test

This will also make grapher.js. Test specs can be found in the spec folder.

**Documentation**

Documentation is generated using groc, and is also done during version upgrades.

    groc

If you need to generate docs into the gh-pages branch, you can use:

    make gh-pages

This will create a new branch off gh-pages named gh-pages-$(commit) which will
contain the build and docs generated from the current HEAD.
Please make sure to commit or stash any changes before running this command.

License
--------
Grapher.js may be freely distributed under the Apache 2.0 license.
