# npmtest-thinkjs

#### basic test coverage for  [thinkjs (v2.2.18)](https://github.com/thinkjs/thinkjs#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-thinkjs.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-thinkjs) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-thinkjs.svg)](https://travis-ci.org/npmtest/node-npmtest-thinkjs)

#### ThinkJS - Use full ES6/7 features to develop web applications, Support TypeScript

[![NPM](https://nodei.co/npm/thinkjs.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/thinkjs)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-thinkjs/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-thinkjs/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-thinkjs/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-thinkjs/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-thinkjs/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-thinkjs/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-thinkjs/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-thinkjs/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-thinkjs/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-thinkjs/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-thinkjs/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-thinkjs/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-thinkjs/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-thinkjs/build/test-report.html](https://npmtest.github.io/node-npmtest-thinkjs/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-thinkjs/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-thinkjs/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-thinkjs/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-thinkjs/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-thinkjs/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-thinkjs/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-thinkjs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-thinkjs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "welefen"
    },
    "bin": {
        "thinkjs": "./bin/index.js"
    },
    "bugs": {
        "url": "https://github.com/thinkjs/thinkjs/issues"
    },
    "contributors": [
        {
            "name": "welefen"
        },
        {
            "name": "im-kulikov"
        },
        {
            "name": "maxzhang"
        },
        {
            "name": "akira-cn"
        },
        {
            "name": "qgy18"
        }
    ],
    "dependencies": {
        "babel-runtime": "6.6.1",
        "bluebird": "3.3.5",
        "co": "4.6.0",
        "colors": "1.1.2",
        "commander": "2.9.0",
        "ejs": "2.4.1",
        "mime": "1.3.4",
        "multiparty": "4.1.2",
        "mysql": "2.11.1",
        "thinkit": "4.10.0",
        "validator": "4.2.0"
    },
    "description": "ThinkJS - Use full ES6/7 features to develop web applications, Support TypeScript",
    "devDependencies": {
        "babel-cli": "^6.18.0",
        "babel-core": "^6.20.0",
        "babel-eslint": "^6.0.4",
        "babel-plugin-transform-runtime": "^6.15.0",
        "babel-preset-es2015": "^6.18.0",
        "babel-preset-stage-1": "^6.16.0",
        "eslint": "2.8.0",
        "istanbul": "0.4.0",
        "mocha": "1.20.1",
        "muk": "0.3.1",
        "source-map": "0.5.3",
        "typescript": "^2.1.6"
    },
    "directories": {},
    "dist": {
        "shasum": "d955937b17a718dfe46b3c2a4436652aab02ca64",
        "tarball": "https://registry.npmjs.org/thinkjs/-/thinkjs-2.2.18.tgz"
    },
    "engines": {
        "node": ">=0.12.0"
    },
    "gitHead": "fe51a4a6f8e8439fa862a75706d34a3728f422fc",
    "homepage": "https://github.com/thinkjs/thinkjs#readme",
    "keywords": [
        "thinkjs",
        "framework",
        "web",
        "rest",
        "restful",
        "router",
        "api",
        "es6",
        "es7",
        "async",
        "await",
        "yield",
        "websocket",
        "generator-function",
        "typescript"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "welefen"
        }
    ],
    "name": "thinkjs",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/thinkjs/thinkjs.git"
    },
    "scripts": {
        "compile": "babel src/ --out-dir lib/",
        "eslint": "eslint src/",
        "prepublish": "npm run compile",
        "test": "npm run eslint && npm run test-cov",
        "test-cov": "istanbul cover ./node_modules/mocha/bin/_mocha -- -t 50000 --recursive  -R spec test/",
        "watch": "npm run watch-compile",
        "watch-compile": "npm run compile -- --watch"
    },
    "version": "2.2.18"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
