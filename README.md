# ml-regression-multivariate-linear

[![NPM version][npm-image]][npm-url]
[![npm download][download-image]][download-url]

Multivariate linear regression. [edited for Angular 2+ usage]

## Installation

`npm install --save ngx-regression-multivariate-linear`

## API ([ See ml-regression-multivariate-linear ](https://www.npmjs.com/package/ml-regression-multivariate-linear))

### new MLR(x, y[, options])

**Arguments**

* `x`: Matrix containing the inputs
* `y`: Matrix containing the outputs

**Options**

* `intercept`: boolean indicating if intercept terms should be computed (default: true)
* `statistics`: boolean for calculating and returning regression statistics (default: true)

## Usage

```js
import MLR from 'ngx-regression-multivariate-linear';

const x = [[0, 0], [1, 2], [2, 3], [3, 4]];
// Y0 = X0 * 2, Y1 = X1 * 2, Y2 = X0 + X1
const y = [[0, 0, 0], [2, 4, 3], [4, 6, 5], [6, 8, 7]];
const mlr = new MLR(x, y);
console.log(mlr.predict([3, 3]));
// [6, 6, 6]
```

## License

[MIT](./LICENSE)

[npm-image]: https://img.shields.io/npm/v/ngx-regression-multivariate-linear.svg?style=flat-square
[npm-url]: https://npmjs.org/package/ngx-regression-multivariate-linear
[download-image]: https://img.shields.io/npm/dm/ngx-regression-multivariate-linear.svg?style=flat-square
[download-url]: https://npmjs.org/package/ngx-regression-multivariate-linear
