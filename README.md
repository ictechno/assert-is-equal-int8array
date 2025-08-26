# assert-is-equal-int8array

![GitHub release](https://img.shields.io/github/release/ictechno/assert-is-equal-int8array.svg)  
[![Visit Releases](https://img.shields.io/badge/Visit%20Releases-Here-brightgreen)](https://github.com/ictechno/assert-is-equal-int8array/releases)

## Overview

The `assert-is-equal-int8array` library provides a simple and effective way to test if two arguments are both `Int8Arrays` and have equal values. This utility is particularly useful for developers who need to perform strict type checks and value comparisons in JavaScript applications. 

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API](#api)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)
- [Support](#support)

## Features

- **Type Safety**: Ensures both arguments are `Int8Arrays`.
- **Value Comparison**: Checks if the contents of both arrays are equal.
- **Lightweight**: Minimal footprint for your applications.
- **Easy Integration**: Simple API that fits well into existing projects.

## Installation

You can install `assert-is-equal-int8array` via npm. Run the following command in your terminal:

```bash
npm install assert-is-equal-int8array
```

## Usage

To use the library, simply import it into your JavaScript file and call the function with two `Int8Array` arguments.

```javascript
const assertIsEqualInt8Array = require('assert-is-equal-int8array');

const array1 = new Int8Array([1, 2, 3]);
const array2 = new Int8Array([1, 2, 3]);

const isEqual = assertIsEqualInt8Array(array1, array2);
console.log(isEqual); // true
```

## API

### `assertIsEqualInt8Array(array1, array2)`

- **Parameters**:
  - `array1`: The first `Int8Array` to compare.
  - `array2`: The second `Int8Array` to compare.
  
- **Returns**: 
  - `true` if both arrays are equal in type and value.
  - `false` otherwise.

### Example

```javascript
const array1 = new Int8Array([1, 2, 3]);
const array2 = new Int8Array([1, 2, 3]);
const array3 = new Int8Array([4, 5, 6]);

console.log(assertIsEqualInt8Array(array1, array2)); // true
console.log(assertIsEqualInt8Array(array1, array3)); // false
```

## Examples

Here are some more examples to illustrate the usage of `assert-is-equal-int8array`.

### Example 1: Equal Arrays

```javascript
const array1 = new Int8Array([10, 20, 30]);
const array2 = new Int8Array([10, 20, 30]);

console.log(assertIsEqualInt8Array(array1, array2)); // true
```

### Example 2: Different Arrays

```javascript
const array1 = new Int8Array([1, 2, 3]);
const array2 = new Int8Array([1, 2, 4]);

console.log(assertIsEqualInt8Array(array1, array2)); // false
```

### Example 3: Different Types

```javascript
const array1 = new Int8Array([1, 2, 3]);
const notAnArray = [1, 2, 3];

console.log(assertIsEqualInt8Array(array1, notAnArray)); // false
```

## Contributing

We welcome contributions to improve `assert-is-equal-int8array`. If you want to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature/YourFeature`).
6. Open a pull request.

Please ensure your code adheres to our coding standards and includes appropriate tests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Support

For any issues or questions, please check the [Releases](https://github.com/ictechno/assert-is-equal-int8array/releases) section. If you can't find an answer, feel free to open an issue in the repository.

---

Thank you for using `assert-is-equal-int8array`. We hope this library makes your development easier and more efficient!