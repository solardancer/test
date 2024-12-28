# @solardancer/test

[![JSR][jsr-image]][jsr-url] [![NPM][npm-image]][npm-url] [![CI][ci-image]][ci-url]

A simple assertion function.

## Usage

```ts
import assert from '@solardancer/test';

assert(true); // doesn't throw

assert(false); // throws an AssertionError

assert(false, 'message'); // throws an AssertionError with a custom error message

assert(false, new Error('message')); // throws a custom Error

const value: string | undefined = 'hello';
assert(value !== undefined); // narrows the type of value to string;
value.toUpperCase(); // works
```

[ci-image]: https://img.shields.io/github/actions/workflow/status/solardancer/test/ci.yml?branch=main&logo=github&style=flat-square
[ci-url]: https://github.com/solardancer/test/actions/workflows/ci.yml
[npm-image]: https://img.shields.io/npm/v/@solardancer/test.svg?style=flat-square
[npm-url]: https://npmjs.org/package/@solardancer/test
[jsr-image]: https://jsr.io/badges/@solardancer/test?style=flat-square
[jsr-url]: https://jsr.io/@solardancer/test
