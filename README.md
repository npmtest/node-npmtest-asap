# npmtest-asap

#### basic test coverage for  [asap (v2.0.5)](https://github.com/kriskowal/asap#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-asap.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-asap) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-asap.svg)](https://travis-ci.org/npmtest/node-npmtest-asap)

#### High-priority task queue for Node.js and browsers

[![NPM](https://nodei.co/npm/asap.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/asap)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-asap/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-asap/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-asap/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-asap/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-asap/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-asap/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-asap/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-asap/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-asap/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-asap/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-asap/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-asap/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-asap/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-asap/build/test-report.html](https://npmtest.github.io/node-npmtest-asap/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-asap/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-asap/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-asap/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-asap/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-asap/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-asap/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-asap/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-asap/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "browser": {
        "./asap": "./browser-asap.js",
        "./asap.js": "./browser-asap.js",
        "./raw": "./browser-raw.js",
        "./raw.js": "./browser-raw.js",
        "./test/domain.js": "./test/browser-domain.js"
    },
    "bugs": {
        "url": "https://github.com/kriskowal/asap/issues"
    },
    "dependencies": {},
    "description": "High-priority task queue for Node.js and browsers",
    "devDependencies": {
        "benchmark": "^1.0.0",
        "events": "^1.0.1",
        "jshint": "^2.5.1",
        "knox": "^0.8.10",
        "mr": "^2.0.5",
        "opener": "^1.3.0",
        "q": "^2.0.3",
        "q-io": "^2.0.3",
        "saucelabs": "^0.1.1",
        "wd": "^0.2.21",
        "weak-map": "^1.0.5"
    },
    "directories": {},
    "dist": {
        "shasum": "522765b50c3510490e52d7dcfe085ef9ba96958f",
        "tarball": "https://registry.npmjs.org/asap/-/asap-2.0.5.tgz"
    },
    "files": [
        "raw.js",
        "asap.js",
        "browser-raw.js",
        "browser-asap.js"
    ],
    "gitHead": "e7f3d29eed4967ecfcaddbfc9542e2ee12b76227",
    "homepage": "https://github.com/kriskowal/asap#readme",
    "keywords": [
        "event",
        "task",
        "queue"
    ],
    "license": "MIT",
    "main": "./asap.js",
    "maintainers": [
        {
            "name": "kriskowal"
        },
        {
            "name": "forbeslindesay"
        }
    ],
    "name": "asap",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/kriskowal/asap.git"
    },
    "scripts": {
        "benchmarks": "node benchmarks",
        "lint": "jshint raw.js asap.js browser-raw.js browser-asap.js $(find scripts -name '*.js' | grep -v gauntlet)",
        "test": "npm run lint && npm run test-node",
        "test-browser": "node scripts/publish-bundle.js test/asap-test.js | xargs opener",
        "test-node": "node test/asap-test.js",
        "test-publish": "node scripts/publish-bundle.js test/asap-test.js | pbcopy",
        "test-saucelabs": "node scripts/saucelabs.js test/asap-test.js scripts/saucelabs-spot-configurations.json",
        "test-saucelabs-all": "node scripts/saucelabs.js test/asap-test.js scripts/saucelabs-all-configurations.json",
        "test-saucelabs-worker": "node scripts/saucelabs-worker-test.js scripts/saucelabs-spot-configurations.json",
        "test-saucelabs-worker-all": "node scripts/saucelabs-worker-test.js scripts/saucelabs-all-configurations.json",
        "test-travis": "npm run lint && npm run test-node && npm run test-saucelabs && npm run test-saucelabs-worker"
    },
    "version": "2.0.5",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
