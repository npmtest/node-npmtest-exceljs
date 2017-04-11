# test coverage for  [exceljs (v0.4.3)](https://github.com/guyonroche/exceljs#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-exceljs.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-exceljs) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-exceljs.svg)](https://travis-ci.org/npmtest/node-npmtest-exceljs)
#### Excel Workbook Manager - Read and Write xlsx and csv Files.

[![NPM](https://nodei.co/npm/exceljs.png?downloads=true)](https://www.npmjs.com/package/exceljs)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-exceljs/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-exceljs/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-exceljs/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-exceljs/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-exceljs/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-exceljs/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-exceljs/tree/gh-pages/build)|

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-exceljs/build/screenCapture.buildCustomOrg.browser.coverage.html.png)](https://npmtest.github.io/node-npmtest-exceljs/build/coverage.html/index.html)

[![test-report](https://npmtest.github.io/node-npmtest-exceljs/build/screenCapture.buildCustomOrg.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmtest%252Fnode-npmtest-exceljs%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-exceljs/build/test-report.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-exceljs/build/screenCapture.buildApidoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-exceljs%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-exceljs/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-exceljs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-exceljs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Guyon Roche"
    },
    "bugs": {
        "url": "https://github.com/guyonroche/exceljs/issues"
    },
    "dependencies": {
        "archiver": "^1.3.0",
        "fast-csv": "^2.4.0",
        "jszip": "3.1.3",
        "moment": "^2.17.1",
        "promish": ">=5.0.2",
        "sax": "^1.2.2",
        "unzip2": "^0.2.5"
    },
    "description": "Excel Workbook Manager - Read and Write xlsx and csv Files.",
    "devDependencies": {
        "babel-eslint": "^7.2.0",
        "babel-polyfill": "^6.23.0",
        "babel-preset-es2015": "^6.22.0",
        "bluebird": "^3.4.7",
        "browserify": "^14.1.0",
        "chai": "*",
        "chai-datetime": "*",
        "chai-xml": "*",
        "eslint": "^3.18.0",
        "eslint-config-airbnb": "^14.1.0",
        "eslint-plugin-import": "^2.2.0",
        "eslint-plugin-jsx-a11y": "^3.0.2",
        "eslint-plugin-react": "^6.10.3",
        "express": "*",
        "grunt": "^1.0.1",
        "grunt-babel": "^6.0.0",
        "grunt-browserify": "^5.0.0",
        "grunt-contrib-jasmine": "^1.1.0",
        "grunt-contrib-uglify": "^2.1.0",
        "grunt-contrib-watch": "^1.0.0",
        "jshint": "*",
        "memorystream": "*",
        "mocha": "*",
        "request": "*",
        "uglifyjs": "^2.4.10",
        "underscore": "^1.8.3"
    },
    "directories": {},
    "dist": {
        "shasum": "a6768ff1483b71e7dced97c1551b73ad25b7c022",
        "tarball": "https://registry.npmjs.org/exceljs/-/exceljs-0.4.3.tgz"
    },
    "files": [
        "excel.js",
        "lib",
        "dist",
        "LICENSE",
        "README.md",
        "MODEL.md"
    ],
    "gitHead": "7fde8ee62f87e6d8130cb7cccfde40760c9ce23f",
    "homepage": "https://github.com/guyonroche/exceljs#readme",
    "keywords": [
        "xlsx",
        "json",
        "csv",
        "excel",
        "font",
        "border",
        "fill",
        "number",
        "format",
        "number format",
        "alignment",
        "office",
        "spreadsheet",
        "workbook",
        "defined names",
        "data validations",
        "rich text",
        "in-cell format",
        "outlineLevel",
        "views",
        "frozen",
        "split",
        "pageSetup"
    ],
    "license": "MIT",
    "main": "./excel.js",
    "maintainers": [
        {
            "name": "guyonroche",
            "email": "cyber.sapiens@hotmail.com"
        }
    ],
    "name": "exceljs",
    "optionalDependencies": {},
    "private": false,
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/guyonroche/exceljs.git"
    },
    "scripts": {
        "browser-test": "grunt jasmine",
        "build": "grunt build",
        "clean": "rm -rf build/ && rm -rf dist",
        "clean-build": "npm run clean && npm run build",
        "end-to-end-test": "mocha spec/end-to-end --recursive",
        "integration-test": "mocha spec/integration --recursive",
        "lint": "eslint --ext .js lib spec",
        "manual-test": "node spec/manual/app.js",
        "prepublish": "npm run build && npm test",
        "test": "npm run unit-test && npm run integration-test && npm run end-to-end-test && npm run browser-test",
        "unit-test": "mocha spec/unit --recursive"
    },
    "version": "0.4.3"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
