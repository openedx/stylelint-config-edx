# Open edX Stylelint configs
[![Build Status](https://github.com/openedx/stylelint-config-edx/workflows/Node%20CI/badge.svg?branch=master)](https://github.com/openedx/stylelint-config-edx/actions?query=workflow%3A%22Node+CI%22)

# Purpose
Stylelint configs for Open edX Sass files.

## Table of Contents

- [Open edX Stylelint configs](#open-edx-stylelint-configs)
- [Purpose](#purpose)
  - [Table of Contents](#table-of-contents)
  - [Overview](#overview)
  - [License](#license)
  - [Usage](#usage)
  - [Sass Style Guide](#sass-style-guide)

## Overview

In order to standardize and enforce Open edX's Sass coding style across
multiple codebases, Open edX has adopted Stylelint. This package provides
the rules defined by the Open edX development community.

## License

The code in this repository is released under the Apache 2.0 license
unless otherwise noted. Please see the [LICENSE
file](https://github.com/openedx/stylelint-config-edx/blob/master/LICENSE) for details.

## Usage

To begin using the Open edX Stylelint configs in a codebase, install this
package from npm:

    npm install --save-dev @edx/stylelint-config-edx

Then, configure your project's Stylelint config to extend
`stylelint-config-edx` (see the ESLint docs
on [Using a Shareable
Config](https://stylelint.io/user-guide/configuration/#extends)).

The simplest option is to add the following to a file
`stylelint.config.js` at the root of your repository:

    module.exports = {
      extends: '@edx/stylelint-config-edx'
    };


## Sass Style Guide

For the most part, Open edX follows the recommended SCSS rules defined
by the [stylelint-config-recommended-scss package](https://www.npmjs.com/package/stylelint-config-recommended-scss).

The only changes are that the following rules have been disabled:

 - [function-comma-newline-after](https://stylelint.io/user-guide/rules/function-comma-newline-after/)
 - [function-parentheses-newline-inside](https://stylelint.io/user-guide/rules/function-parentheses-newline-inside/)
 - [max-empty-lines](https://stylelint.io/user-guide/rules/max-empty-lines/)
