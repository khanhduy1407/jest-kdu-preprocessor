# jest-kdu-preprocessor

> This package supports both ES6 (Babel) and TypeScript.

Portions both preprocessors are heavily based [kduify](https://github.com/kdutifyjs/kduify) (Copyright (c) 2021-present NKDuy).

### Installation

  1.  add package you your project
    
   *  `yarn add --dev jest-kdu-preprocessor` or  `npm install --saveDev jest-kdu-preprocessor`
 
  2.  modify package.json's **jest** section by adding/editing **moduleFileExtensions** and **transform** properites:

      ```javascript
      "jest": {
        "moduleFileExtensions": [
          "js",
          "kdu"
        ],
        "transform": {
          "^.+\\.js$": "<rootDir>/node_modules/babel-jest",
          ".*\\.(kdu)$": "<rootDir>/node_modules/jest-kdu-preprocessor"
        }
      }
      ```
  3.  Start writing test that can import `*.kdu` components - see example **./tests/index.spec.js**
  4.  Profit!

  ### License: MIT
