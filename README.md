# edX Stylelint configs
[![Build Status](https://github.com/openedx/stylelint-config-edx/workflows/Node%20CI/badge.svg?branch=master)](https://github.com/openedx/stylelint-config-edx/actions?query=workflow%3A%22Node+CI%22)

Stylelint configs for edX Sass files.

## Table of Contents

1. [Overview](#overview)
2. [License](#license)
3. [Dependencies](#dependencies)
4. [Usage](#usage)
5. [The Configs](#the-configs)

## Overview

In order to standardize and enforce edX's Sass coding style across
multiple codebases, edX has adopted Stylelint. This package provides
the rules defined by the edX development community.

## License

The code in this repository is released under the Apache 2.0 license
unless otherwise noted. Please see the [LICENSE
file](https://github.com/openedx/stylelint-config-edx/blob/master/LICENSE) for details.

## Usage

To begin using the edX Stylelint configs in a codebase, install this
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

For the most part, edX follows the recommended SCSS rules defined
by the [stylelint-config-recommended-scss package](https://www.npmjs.com/package/stylelint-config-recommended-scss).

The only changes are that the following rules have been disabled:

 - [function-comma-newline-after](https://stylelint.io/user-guide/rules/function-comma-newline-after/)
 - [function-parentheses-newline-inside](https://stylelint.io/user-guide/rules/function-parentheses-newline-inside/)
 - [max-empty-lines](https://stylelint.io/user-guide/rules/max-empty-lines/)
