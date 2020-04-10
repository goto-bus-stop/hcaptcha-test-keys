# hcaptcha-test-keys
The [hCaptcha][] widget keys for testing and development environments, but as a
Node.js module with a name.

[Provided by hCaptcha in their documentation.][ref]

## Installation
```
npm install --save hcaptcha-test-keys
```

## Usage
```js
const testKeys = require('hcaptcha-test-keys')

hcaptcha.render('hcaptcha-element', {
  sitekey: process.env.NODE_ENV === 'development'
    ? testKeys.sitekey
    : yourActualSiteKey()
})

// etc
```

## API
### `testKeys.sitekey`
Site key: `10000000-ffff-ffff-ffff-000000000001`

### `testKeys.secret`
Secret key: `0x0000000000000000000000000000000000000000`

## Related
- [recaptcha-test-keys][] - Google ReCaptcha test keys as a Node.js module

## License
[Unlicense](./LICENSE)

[hCaptcha]: https://hcaptcha.com/
[ref]: https://docs.hcaptcha.com/#integrationtest
[recaptcha-test-keys]: https://github.com/goto-bus-stop/recaptcha-test-keys
