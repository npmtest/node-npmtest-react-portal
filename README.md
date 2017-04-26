# npmtest-react-portal

#### basic test coverage for  [react-portal (v3.1.0)](https://github.com/tajo/react-portal#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-react-portal.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-react-portal) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-react-portal.svg)](https://travis-ci.org/npmtest/node-npmtest-react-portal)

#### React component for transportation of modals, lightboxes, loading bars... to document.body

[![NPM](https://nodei.co/npm/react-portal.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-portal)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-react-portal/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-portal/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-react-portal/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-react-portal/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-react-portal/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-react-portal/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-react-portal/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-react-portal/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-react-portal/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-react-portal/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-react-portal/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-portal/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-react-portal/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-react-portal/build/test-report.html](https://npmtest.github.io/node-npmtest-react-portal/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-react-portal/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-react-portal/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-react-portal/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-portal/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-portal/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-portal/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-react-portal/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-react-portal/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Vojtech Miksu"
    },
    "bugs": {
        "url": "https://github.com/tajo/react-portal/issues"
    },
    "dependencies": {
        "prop-types": "^15.5.8"
    },
    "description": "React component for transportation of modals, lightboxes, loading bars... to document.body",
    "devDependencies": {
        "babel-cli": "^6.8.0",
        "babel-core": "^6.8.0",
        "babel-eslint": "^6.0.4",
        "babel-loader": "^6.2.1",
        "babel-plugin-add-module-exports": "^0.2.1",
        "babel-preset-es2015": "^6.3.13",
        "babel-preset-react": "^6.3.13",
        "babel-preset-react-hmre": "^1.0.1",
        "babel-register": "^6.8.0",
        "cross-env": "^1.0.7",
        "enzyme": "^2.3.0",
        "eslint": "^2.9.0",
        "eslint-config-airbnb": "^9.0.1",
        "eslint-plugin-import": "^1.8.0",
        "eslint-plugin-jsx-a11y": "^1.2.0",
        "eslint-plugin-react": "^5.1.1",
        "express": "^4.13.3",
        "jsdom": "^9.0.0",
        "mocha": "^2.3.4",
        "mocha-eslint": "^2.0.2",
        "react": "^15.2.0",
        "react-addons-test-utils": "^15.2.0",
        "react-dom": "^15.2.0",
        "rimraf": "^2.5.0",
        "sinon": "^1.17.4",
        "tween.js": "^16.3.1",
        "webpack": "^1.13.0",
        "webpack-dev-middleware": "^1.6.1",
        "webpack-hot-middleware": "^2.6.0"
    },
    "directories": {},
    "dist": {
        "shasum": "865c44fb72a1da106c649206936559ce891ee899",
        "tarball": "https://registry.npmjs.org/react-portal/-/react-portal-3.1.0.tgz"
    },
    "files": [
        "*.md",
        "LICENSE",
        "lib",
        "build"
    ],
    "gitHead": "5ebaf66ae5127abaa0fdcf8a36b9db5b5c22356b",
    "homepage": "https://github.com/tajo/react-portal#readme",
    "keywords": [
        "react",
        "react-component",
        "modal",
        "lightbox",
        "react-portal",
        "portal",
        "transportation"
    ],
    "license": "MIT",
    "main": "build/portal",
    "maintainers": [
        {
            "name": "miksu"
        }
    ],
    "name": "react-portal",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/tajo/react-portal.git"
    },
    "scripts": {
        "build": "mkdir -p build && babel ./lib/portal.js --out-file ./build/portal.js",
        "build:examples": "npm run clean && npm run build:examples:webpack",
        "build:examples:webpack": "cross-env NODE_ENV=production webpack --config webpack.config.prod.babel.js",
        "clean": "rimraf build",
        "lint": "mocha test/eslint_spec.js",
        "prepublish": "cross-env NODE_ENV=production npm run build",
        "start": "node devServerIndex.js",
        "test": "mocha"
    },
    "tags": [
        "react"
    ],
    "version": "3.1.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
