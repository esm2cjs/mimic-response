# @esm2cjs/mimic-response

This is a fork of https://github.com/sindresorhus/mimic-response, but automatically patched to support ESM **and** CommonJS, unlike the original repository.

## Install

You can use an npm alias to install this package under the original name:

```
npm i mimic-response@npm:@esm2cjs/mimic-response
```

```jsonc
// package.json
"dependencies": {
    "mimic-response": "npm:@esm2cjs/mimic-response"
}
```

but `npm` might dedupe this incorrectly when other packages depend on the replaced package. If you can, prefer using the scoped package directly:

```
npm i @esm2cjs/mimic-response
```

```jsonc
// package.json
"dependencies": {
    "@esm2cjs/mimic-response": "^ver.si.on"
}
```

## Usage

```js
// Using ESM import syntax
import mimicResponse from "@esm2cjs/mimic-response";

// Using CommonJS require()
const mimicResponse = require("@esm2cjs/mimic-response").default;
```

> **Note:**
> Because the original module uses `export default`, you need to append `.default` to the `require()` call.

For more details, please see the original [repository](https://github.com/sindresorhus/mimic-response).

## Sponsoring

To support my efforts in maintaining the ESM/CommonJS hybrid, please sponsor [here](https://github.com/sponsors/AlCalzone).

To support the original author of the module, please sponsor [here](https://github.com/sindresorhus/mimic-response).
