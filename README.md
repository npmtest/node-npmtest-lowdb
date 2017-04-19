# npmtest-lowdb

#### basic test coverage for  [lowdb (v0.16.2)](https://github.com/typicode/lowdb)  [![npm package](https://img.shields.io/npm/v/npmtest-lowdb.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-lowdb) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-lowdb.svg)](https://travis-ci.org/npmtest/node-npmtest-lowdb)

#### JSON database for Node and the browser powered by lodash API

[![NPM](https://nodei.co/npm/lowdb.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/lowdb)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-lowdb/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-lowdb/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-lowdb/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-lowdb/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-lowdb/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-lowdb/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-lowdb/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-lowdb/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-lowdb/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-lowdb/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-lowdb/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-lowdb/build/test-report.html](https://npmtest.github.io/node-npmtest-lowdb/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-lowdb/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-lowdb/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-lowdb/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-lowdb/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-lowdb/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-lowdb/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-lowdb/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-lowdb/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Typicode"
    },
    "browser": {
        "./src/storages/file-sync.js": "./src/storages/browser.js",
        "./lib/storages/file-sync.js": "./lib/storages/browser.js"
    },
    "bugs": {
        "url": "https://github.com/typicode/lowdb/issues"
    },
    "dependencies": {
        "graceful-fs": "^4.1.3",
        "is-promise": "^2.1.0",
        "lodash": "4",
        "steno": "^0.4.1"
    },
    "description": "JSON database for Node and the browser powered by lodash API",
    "devDependencies": {
        "babel-cli": "^6.2.0",
        "babel-eslint": "^7.0.0",
        "babel-loader": "^6.2.2",
        "babel-polyfill": "^6.9.1",
        "babel-preset-es2015": "^6.1.18",
        "babel-preset-stage-3": "^6.3.13",
        "babel-register": "^6.9.0",
        "husky": "^0.13.0",
        "lodash-id": "^0.13.0",
        "pkg-ok": "^1.0.1",
        "ramda": "^0.23.0",
        "rimraf": "^2.5.4",
        "sinon": "^1.17.2",
        "standard": "^8.5.0",
        "tap-spec": "^4.1.1",
        "tape": "^4.2.2",
        "tempfile": "^1.1.1",
        "webpack": "^2.2.1"
    },
    "directories": {},
    "dist": {
        "shasum": "a2a976eb66ec57797291970f3c87cdb61126fa3a",
        "tarball": "https://registry.npmjs.org/lowdb/-/lowdb-0.16.2.tgz"
    },
    "engines": {
        "node": ">= 0.12"
    },
    "gitHead": "4a76af0f79d900043fd5ebf0ff4b378e8404bd89",
    "homepage": "https://github.com/typicode/lowdb",
    "keywords": [
        "flat",
        "file",
        "local",
        "database",
        "storage",
        "JSON",
        "lo-dash",
        "lodash",
        "underscore",
        "localStorage",
        "embed",
        "embeddable"
    ],
    "license": "MIT",
    "main": "./lib/main.js",
    "maintainers": [
        {
            "name": "typicode"
        }
    ],
    "name": "lowdb",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/typicode/lowdb.git"
    },
    "scripts": {
        "build": "npm run build:lib && npm run build:dist",
        "build:dist": "rimraf dist && webpack && webpack -p",
        "build:lib": "rimraf lib && babel src --out-dir lib",
        "fix": "standard --fix",
        "precommit": "npm test",
        "prepublish": "npm run build && pkg-ok",
        "tape": "tape -r babel-register -r babel-polyfill test/*.js | tap-spec",
        "test": "npm run tape && standard"
    },
    "standard": {
        "parser": "babel-eslint"
    },
    "version": "0.16.2"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
