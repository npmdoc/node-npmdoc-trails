# npmdoc-trails

#### basic api documentation for  [trails (v2.0.2)](http://trailsjs.io)  [![npm package](https://img.shields.io/npm/v/npmdoc-trails.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-trails) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-trails.svg)](https://travis-ci.org/npmdoc/node-npmdoc-trails)

#### Modern Web Application Framework for Node.js

[![NPM](https://nodei.co/npm/trails.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/trails)

- [https://npmdoc.github.io/node-npmdoc-trails/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-trails/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-trails/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-trails/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-trails/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-trails/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Trails.js Team"
    },
    "bugs": {
        "url": "https://github.com/trailsjs/trails/issues"
    },
    "bundleDependencies": [
        "trails-controller",
        "trails-model",
        "trails-policy",
        "trails-service"
    ],
    "contributors": [
        {
            "name": "Travis Webb",
            "url": "https://github.com/tjwebb"
        },
        {
            "name": "Konstantin Zolotarev",
            "url": "https://github.com/konstantinzolotarev"
        },
        {
            "name": "Weyland Joyner",
            "url": "https://github.com/weyj4"
        },
        {
            "name": "Jimmy Aumard",
            "url": "https://github.com/jaumard"
        },
        {
            "name": "Robert Rossmann",
            "url": "https://github.com/Alaneor"
        },
        {
            "name": "Mike Hostetler"
        }
    ],
    "dependencies": {
        "hoek": "^4.1.0",
        "i18next": "^3.4.1",
        "joi": "^10.2.2",
        "lodash": "^4.17.2",
        "mkdirp": "^0.5.1",
        "trails-controller": "^2",
        "trails-model": "^2",
        "trails-policy": "^2",
        "trails-service": "^2"
    },
    "description": "Modern Web Application Framework for Node.js",
    "devDependencies": {
        "eslint": "^3.15.0",
        "eslint-config-trails": "^2.0.8",
        "istanbul": "^0.4.5",
        "mocha": "^3.2.0",
        "pre-commit": "^1.2.2",
        "smokesignals": "^2.1.0",
        "trailpack": "^2",
        "winston": "^2.3.1"
    },
    "directories": {},
    "dist": {
        "shasum": "58b4b4bc0f49f18a279a0aa3afce813ab4594431",
        "tarball": "https://registry.npmjs.org/trails/-/trails-2.0.2.tgz"
    },
    "engines": {
        "node": ">= 4.0.0",
        "npm": ">= 2.14.2"
    },
    "eslintConfig": {
        "extends": "trails"
    },
    "gitHead": "308dac16768f8d90f21924cb7824e5f4a4282744",
    "homepage": "http://trailsjs.io",
    "keywords": [
        "framework",
        "platform",
        "rest",
        "api",
        "rails",
        "grails",
        "sails",
        "trails",
        "trailsjs",
        "server",
        "graphql"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "trails"
        }
    ],
    "name": "trails",
    "optionalDependencies": {},
    "pre-commit": [
        "test"
    ],
    "publishConfig": {
        "tag": "next"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/trailsjs/trails.git"
    },
    "runkitExample": "test/runkitExample.js",
    "scripts": {
        "ci": "cd .. && ci",
        "coverage": "istanbul cover node_modules/mocha/bin/_mocha",
        "test": "eslint --ignore-path .gitignore . && istanbul cover node_modules/mocha/bin/_mocha",
        "test-performance": "eslint . && mocha test-performance"
    },
    "version": "2.0.2",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
