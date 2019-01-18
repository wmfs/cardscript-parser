# cardscript-parser

[![Tymly Cardscript](https://img.shields.io/badge/tymly-cardscript-blue.svg)](https://tymly.io/)
[![Build Status](https://travis-ci.com/wmfs/cardscript-parser.svg?branch=master)](https://travis-ci.com/wmfs/cardscript-parser)
[![npm (scoped)](https://img.shields.io/npm/v/@wmfs/cardscript-parser.svg)](https://www.npmjs.com/package/@wmfs/cardscript-parser) 
[![codecov](https://codecov.io/gh/wmfs/cardscript-parser/branch/master/graph/badge.svg)](https://codecov.io/gh/wmfs/cardscript-parser) 
[![CodeFactor](https://www.codefactor.io/repository/github/wmfs/cardscript-parser/badge)](https://www.codefactor.io/repository/github/wmfs/cardscript-parser) 
[![Dependabot badge](https://img.shields.io/badge/Dependabot-active-brightgreen.svg)](https://dependabot.com/) 
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/) 
[![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com) 
[![license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/wmfs/tymly/blob/master/packages/concrete-paths/LICENSE)

> Like JSON.parse(), but for Cardscript. And it supports YAML.

## <a name="install"></a>Install
```bash
$ npm install cardscript-parser --save
```

## <a name="usage"></a>Usage

```javascript
const parser = require('@wmfs/cardscript-parser')

const cardscriptObject = parser(
  `{
    "type": "AdaptiveCard",
    "body": [
      {
        "type": "TextBlock",
        "text": "Change me!",
        "color": "attention",
        "horizontalAlignment": "center"
      }
    ],
    "$schema": "http://adaptivecards.io/schemas/adaptive-card.json",
    "version": "1.0"
  }`
)

```

## <a name="test"></a>Testing

```bash
$ npm test
```

## <a name="license"></a>License
[MIT](https://github.com/wmfs/cardscript/blob/master/LICENSE)
