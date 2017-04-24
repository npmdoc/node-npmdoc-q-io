# npmdoc-q-io

#### api documentation for  [q-io (v1.13.2)](http://github.com/kriskowal/q-io/)  [![npm package](https://img.shields.io/npm/v/npmdoc-q-io.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-q-io) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-q-io.svg)](https://travis-ci.org/npmdoc/node-npmdoc-q-io)

#### IO using Q promises

[![NPM](https://nodei.co/npm/q-io.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/q-io)

- [https://npmdoc.github.io/node-npmdoc-q-io/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-q-io/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-q-io/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-q-io/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-q-io/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-q-io/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "q-io",
    "version": "1.13.2",
    "description": "IO using Q promises",
    "homepage": "http://github.com/kriskowal/q-io/",
    "author": "Kris Kowal <kris@cixar.com> (http://github.com/kriskowal/)",
    "contributors": [
        "Montage Studio",
        "Stuart Knightley",
        "Jean-romain Prevost",
        "Andreas Pizsa (http://github.com/AndreasPizsa/)"
    ],
    "bugs": {
        "mail": "kris@cixar.com",
        "url": "http://github.com/kriskowal/q-io/issues"
    },
    "license": "MIT",
    "repository": {
        "type": "git",
        "url": "http://github.com/kriskowal/q-io.git"
    },
    "dependencies": {
        "q": "^1.0.1",
        "qs": "^1.2.1",
        "url2": "^0.0.0",
        "mime": "^1.2.11",
        "mimeparse": "^0.1.4",
        "collections": "^0.2.0"
    },
    "devDependencies": {
        "jshint": "^0.9.1",
        "cover": "^0.2.8",
        "jasmine-node": "^1.7",
        "opener": "^1.3"
    },
    "scripts": {
        "test": "jasmine-node spec",
        "test-browser": "opener spec/q-spec.html",
        "lint": "jshint q.js",
        "cover": "cover run jasmine-node spec && cover report html && opener cover_html/index.html"
    },
    "engines": {
        "node": ">=0.6.0"
    },
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
