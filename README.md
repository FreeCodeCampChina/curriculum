# freeCodeCamp Curriculum

[![Build Status](https://travis-ci.org/freeCodeCamp/curriculum.svg?branch=master)](https://travis-ci.org/freeCodeCamp/curriculum) [![npm (scoped)](https://img.shields.io/npm/v/@freecodecamp/curriculum.svg)](https://www.npmjs.com/package/@freecodecamp/curriculum)

> This package contains the "seed" files used in the freeCodeCamp Curriculum.

## Installation

```sh
npm i @freecodecamp/curriculum
# or
yarn add @freecodecamp/curriculum
```

## Usage

```js
import { getChallenges } from '@freecodecamp/curriculum';

// fetch an array of blocks
// i.e. basic CSS, functional programming, etc.
getChallenges()
```

### `block` Structure

```js
{
  "name": "ES6",
  "order": 2,
  "time": "5 hours",
  "helpRoom": "Help",
  "challenges": [/*<challenge>*/],
  "fileName": "02-javascript-algorithms-and-data-structures/es6.json",
  "superBlock": "javascript-algorithms-and-data-structures",
  "superOrder": 2
}
```

### `challenge` Structure

```js
{
  "id": "ObjectId()",
  "title": "Declare a Read-Only Variable with the const Keyword",
  "description": [
    "A Description of the challenge and what is required to pass"
  ],
  "tests": [
    {
      "text": "should return \"foo\"",
      "testString": "a stringified function using Chai asserts"
    }
  ],
  "challengeType": 1,
  "translations": {},
  "files": {
    "indexjs": {
      "key": "indexjs",
      "ext": "js",
      "name": "index",
      "contents": [
        "Initial editor seed"
      ],
      "head": [
        "A place for test set up",
        "Can be thought of as mocha's beforeEach()"
      ],
      "tail": [
        "A place for test tear down",
        "Can be thought of as mocha's afterEach()"
        ]
    }
  }
},
```

## 翻译流程：

1. 从 “issue” 中选择 “**Translation request**” 模板，并填写你想要翻译的章节（以独立 JSON 文件为最小单位），然后提交。

2. 用该 “issue” 来跟踪自己的翻译进度。翻译完成后请提交 PR，并选择 **“S1ngS1ng”** 与 **“wudifeixue”** 两位童鞋进行评审。

   ​

   **注意：**翻译文件不要在源文件上改动，请创建新的翻译文件并以 **“-cn”** 作为文件名后缀结尾。