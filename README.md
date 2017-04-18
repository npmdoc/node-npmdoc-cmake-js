# npmdoc-cmake-js

#### api documentation for  [cmake-js (v3.4.1)](https://github.com/unbornchikken/cmake-js#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-cmake-js.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-cmake-js) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-cmake-js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-cmake-js)

#### CMake.js - a Node.js/io.js native addon build tool

[![NPM](https://nodei.co/npm/cmake-js.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/cmake-js)

- [https://npmdoc.github.io/node-npmdoc-cmake-js/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-cmake-js/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cmake-js/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cmake-js/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-cmake-js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-cmake-js/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Gábor Mező aka unbornchikken"
    },
    "bin": {
        "cmake-js": "./bin/cmake-js"
    },
    "bugs": {
        "url": "https://github.com/unbornchikken/cmake-js/issues"
    },
    "dependencies": {
        "bluebird": "^2.9.15",
        "debug": "^2.1.3",
        "fs-extra": "1",
        "is-iojs": "^1.0.1",
        "lodash": "^3.6.0",
        "memory-stream": "0",
        "npmconf": "^2.1.2",
        "npmlog": "^1.2.0",
        "request": "^2.54.0",
        "semver": "^5.0.3",
        "splitargs": "0",
        "tar": "^1.0.3",
        "traceur": "0.0.x",
        "unzip": "^0.1.11",
        "url-join": "0",
        "which": "^1.0.9",
        "yargs": "^3.6.0"
    },
    "description": "CMake.js - a Node.js/io.js native addon build tool",
    "devDependencies": {
        "gulp": "*",
        "gulp-sequence": "*",
        "gulp-sourcemaps": "*",
        "gulp-traceur": "*",
        "mocha": "*",
        "nan": "^2.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "29b57d6e5417b3a395e549b86cb9dc1f3cd97f90",
        "tarball": "https://registry.npmjs.org/cmake-js/-/cmake-js-3.4.1.tgz"
    },
    "engines": {
        "node": ">= 0.10.0"
    },
    "gitHead": "bcefb84c44742c645f39cb914f1714157848ec21",
    "homepage": "https://github.com/unbornchikken/cmake-js#readme",
    "keywords": [
        "native",
        "addon",
        "module",
        "c",
        "c++",
        "bindings",
        "build",
        "cmake",
        "nw.js",
        "electron",
        "boost"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "unbornchikken"
        }
    ],
    "name": "cmake-js",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/unbornchikken/cmake-js.git"
    },
    "scripts": {
        "compile": "gulp",
        "test": "mocha tests"
    },
    "version": "3.4.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
