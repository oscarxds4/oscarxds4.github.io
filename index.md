---
layout: "default"
title: "ConvertNum: A TypeScript/JavaScript Utility Library for Number Conversions"
description: "Convert numbers easily with ConvNum, a TypeScript utility library for transforming between numeral systems and formats. Perfect for developers! 🚀📊"
---
# ConvertNum: A TypeScript/JavaScript Utility Library for Number Conversions

![GitHub release](https://img.shields.io/github/release/oscarxds4/convnum.svg) ![npm](https://img.shields.io/npm/v/convnum.svg) ![GitHub issues](https://img.shields.io/github/issues/oscarxds4/convnum.svg) ![GitHub forks](https://img.shields.io/github/forks/oscarxds4/convnum.svg) ![GitHub stars](https://img.shields.io/github/stars/oscarxds4/convnum.svg)

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API Reference](#api-reference)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)
- [Links](#links)

## Overview

ConvertNum is a utility library built with TypeScript and JavaScript. It helps you convert between various number representations, numeral systems, date and time formats, and more. With built-in validation and type detection capabilities, ConvertNum simplifies the task of working with numbers in your applications.

Visit the [Releases section](https://github.com/oscarxds4/convnum/releases) to download the latest version.

## Features

- **Number Conversions**: Easily convert between different numeral systems, such as binary, decimal, hexadecimal, and octal.
- **Date and Time Formatting**: Convert date and time into various formats, ensuring compatibility with different locales.
- **Validation**: Check if a number or date is valid before performing conversions.
- **Type Detection**: Automatically detect the type of number or date format you are working with.
- **Simple API**: Easy-to-use functions that make integration straightforward.
- **Lightweight**: Minimal footprint for fast performance.

## Installation

To install ConvertNum, you can use npm or yarn. Run one of the following commands in your terminal:

```bash
npm install convnum
```

or

```bash
yarn add convnum
```

After installation, you can import it into your project:

```javascript
import { convert } from 'convnum';
```

## Usage

Using ConvertNum is straightforward. Here are some basic examples of how to utilize its features.

### Number Conversion

Convert a decimal number to binary:

```javascript
import { toBinary } from 'convnum';

const binary = toBinary(10); // Output: "1010"
```

Convert a binary number to decimal:

```javascript
import { toDecimal } from 'convnum';

const decimal = toDecimal('1010'); // Output: 10
```

### Date and Time Formatting

Convert a date to a specific format:

```javascript
import { formatDate } from 'convnum';

const formattedDate = formatDate(new Date(), 'YYYY-MM-DD'); // Output: "2023-10-01"
```

### Validation

Check if a number is valid:

```javascript
import { isValidNumber } from 'convnum';

const isValid = isValidNumber('123.45'); // Output: true
```

### Type Detection

Detect the type of a number:

```javascript
import { detectType } from 'convnum';

const type = detectType(123); // Output: "integer"
```

## API Reference

### Number Functions

- `toBinary(number: number): string`
- `toDecimal(binary: string): number`
- `isValidNumber(value: string): boolean`
- `detectType(value: any): string`

### Date Functions

- `formatDate(date: Date, format: string): string`
- `isValidDate(date: any): boolean`

## Examples

### Converting Between Number Systems

```javascript
const decimal = 255;
const binary = toBinary(decimal);
console.log(`Binary: ${binary}`); // Output: Binary: 11111111

const hex = decimal.toString(16);
console.log(`Hexadecimal: ${hex}`); // Output: Hexadecimal: ff
```

### Formatting Dates

```javascript
const today = new Date();
const formatted = formatDate(today, 'MM/DD/YYYY');
console.log(`Today's date: ${formatted}`); // Output: Today's date: 10/01/2023
```

### Validating Inputs

```javascript
const input = '123.45';
if (isValidNumber(input)) {
    console.log(`${input} is a valid number.`);
} else {
    console.log(`${input} is not a valid number.`);
}
```

## Contributing

We welcome contributions to ConvertNum. If you want to help, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push to your branch.
5. Create a pull request.

Please ensure your code adheres to the existing style and includes appropriate tests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Links

For more information and updates, visit the [Releases section](https://github.com/oscarxds4/convnum/releases).