# npmdoc-foreman

#### api documentation for  [foreman (v2.0.0)](http://strongloop.github.io/node-foreman/)  [![npm package](https://img.shields.io/npm/v/npmdoc-foreman.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-foreman) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-foreman.svg)](https://travis-ci.org/npmdoc/node-npmdoc-foreman)

#### Node Implementation of Foreman

[![NPM](https://nodei.co/npm/foreman.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/foreman)

- [https://npmdoc.github.io/node-npmdoc-foreman/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-foreman/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-foreman/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-foreman/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-foreman/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-foreman/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "StrongLoop, Inc."
    },
    "bin": {
        "nf": "nf.js"
    },
    "bugs": {
        "url": "https://github.com/strongloop/node-foreman/issues"
    },
    "dependencies": {
        "commander": "~2.9.0",
        "http-proxy": "~1.11.1",
        "mustache": "^2.2.1",
        "shell-quote": "~1.4.2"
    },
    "description": "Node Implementation of Foreman",
    "devDependencies": {
        "chai": "~1.9.1",
        "jshint": "^2.6.3",
        "rimraf": "~2.2.8",
        "tap": "^0.7.1"
    },
    "directories": {},
    "dist": {
        "shasum": "00acd20f9dbbe2f79d04697bcca2a77ee00ee031",
        "tarball": "https://registry.npmjs.org/foreman/-/foreman-2.0.0.tgz"
    },
    "engines": {
        "node": ">=0.6.9"
    },
    "files": [
        "forward.js",
        "nf.js",
        "proxy.js",
        "lib/"
    ],
    "gitHead": "008f16259bcbee5b1f39a83d214f42806e0470d0",
    "homepage": "http://strongloop.github.io/node-foreman/",
    "keywords": [
        "foreman",
        "upstart",
        "commandline",
        "env",
        "Procfile"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "bajtos"
        },
        {
            "name": "chandadharap"
        },
        {
            "name": "ibmcloud-admin"
        },
        {
            "name": "kraman"
        },
        {
            "name": "octet"
        },
        {
            "name": "rfeng"
        },
        {
            "name": "ritch"
        },
        {
            "name": "rmg"
        },
        {
            "name": "setogit"
        },
        {
            "name": "strongloop"
        },
        {
            "name": "superkhau"
        }
    ],
    "name": "foreman",
    "optionalDependencies": {},
    "preferGlobal": true,
    "repository": {
        "type": "git",
        "url": "git+https://github.com/strongloop/node-foreman.git"
    },
    "scripts": {
        "pretest": "jshint .",
        "test": "tap test/*.test.*"
    },
    "version": "2.0.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
