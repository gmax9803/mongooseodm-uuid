<h1 align="center">Welcome to mongooseodm-uuid 👋</h1>
<p>
  <a href="https://www.npmjs.com/package/mongooseodm-uuid" target="_blank">
    <img alt="Version" src="https://img.shields.io/npm/v/mongooseodm-uuid.svg">
  </a>
  <a href="https://github.com/gmax9803/mongoose-uuid#readme" target="_blank">
    <img alt="Documentation" src="https://img.shields.io/badge/documentation-yes-brightgreen.svg" />
  </a>
  <a href="https://github.com/gmax9803/mongoose-uuid/graphs/commit-activity" target="_blank">
    <img alt="Maintenance" src="https://img.shields.io/badge/Maintained%3F-yes-green.svg" />
  </a>
  <a href="https://github.com/gmax9803/mongoose-uuid/blob/master/LICENSE" target="_blank">
    <img alt="License: ISC" src="https://img.shields.io/github/license/gmax9803/mongooseodm-uuid" />
  </a>
</p>

> A Custom Mongoose UUID SchemaType, to use for MongoDB Binary UUIDs (Subtype 0x03 and 0x04)
> (Subtype 0x03 follows the Java Driver implementation.)

> Please note that inserting subtype **0x03** Binary UUIDs to the db is currently not supported

### 🏠 [Homepage](https://github.com/gmax9803/mongoose-uuid#readme)

## Install

```sh
npm i mongooseodm-uuid
```

## Run tests

```sh
npm run test
```

## Usage
1\) Register the SchemaType (insert somewhere like your index.js):
```js
require('mongooseodm-uuid');
```
2\) Use the SchemaType in a Mongoose Schema
```js
const mongoose = require("mongoose");
const {MUUID} = require('mongooseodm-uuid');

const Schema = mongoose.Schema;

const HavocPunishmentSchema = new Schema({
    uuid: MUUID,
});
```
OR
```js
const mongoose = require("mongoose");
const {MUUID} = require('mongooseodm-uuid');

const Schema = mongoose.Schema;

const HavocPunishmentSchema = new Schema({
    uuid: mongoose.Types.MUUID,
});
```
## Author

👤 **Max (https://github.com/gmax9803) (gmax@fourthfruit.com)**

* Website: https://fourthfruit.com (currently down)
* Store: https://cpukeychains.com (Buy some CPUKeychains!)
* Github: [@gmax9803](https://github.com/gmax9803)

## 🤝 Contributing

Contributions, issues and feature requests are welcome!<br />Feel free to check [issues page](https://github.com/gmax9803/mongoose-uuid/issues). You can also take a look at the [contributing guide](https://github.com/gmax9803/mongoose-uuid/blob/master/CONTRIBUTING.md).

## Show your support

Give a ⭐️ if this project helped you!

## 📝 License

Copyright © 2020 [Max (https://github.com/gmax9803) (gmax@fourthfruit.com)](https://github.com/gmax9803). <br />
This project is [ISC](https://github.com/gmax9803/mongoose-uuid/blob/master/LICENSE) licensed.

***
_This README was generated with ❤️ by [readme-md-generator](https://github.com/kefranabg/readme-md-generator)_