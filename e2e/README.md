# @rsdoctor/e2e

This folder contains the e2e test cases of Rsbuild.

## Tech Stack

- [playwright](https://github.com/microsoft/playwright): The e2e test framework.

## Commands

```bash
# Run all test cases, including Rspack and Webpack
pnpm run test
```

## Add Test Cases

### Add test cases for common capabilities

Test cases added using the `test` method will run in webpack and Rspack.

```ts
import { expect, test } from '@playwright/test';
// will passed in webpack, and rspack
test('test 1 + 1', () => {
  expect(1 + 1).toBe(2);
});
```