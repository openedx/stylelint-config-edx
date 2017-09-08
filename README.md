# edX Stylelint configs
[![Build Status](https://travis-ci.org/edx/stylelint-config-edx.svg?branch=master)](https://travis-ci.org/edx/eslint-config-edx)

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
file](https://github.com/edx/eslint-config-edx/blob/master/LICENSE) for
details.

## Dependencies

[ESLint](http://eslint.org) is required to use either config, and NodeJS
4.0 or greater is required to use ESLint. Both configs are tested with
the Node version bundled in the [most recent edX devstack
setup](http://edx.readthedocs.io/projects/edx-installing-configuring-and-running/en/latest/installation/devstack/install_devstack.html).

## Usage

To begin using the edX ESLint configs in a codebase, install this
package from npm:

    npm install --save-dev stylelint-config-edx

Then, configure your project's ESLint config to extend
`stylelint-config-edx` (see the ESLint docs
on [Using a Shareable
Config](http://eslint.org/docs/developer-guide/shareable-configs#using-a-shareable-config)).
If you do not plan on adding custom rules beyond those in
`eslint-config-edx` to your project, the easiest place to configure this
is probably in your `package.json`:

    "devDependencies": {
        "eslint-config-edx": "^2.0.0"
    },
    "eslintConfig": {
        "extends": "eslint-config-edx"
    }

If you plan on adding additional customization, you can [configure your
project with an `.eslintrc.js`/`.eslintrc.json`
file](http://eslint.org/docs/user-guide/configuring#configuration-file-formats).

## The Configs

More documentation on the rules specified by each config is available in:

- [the README for `eslint-config-edx`](https://github.com/edx/eslint-config-edx/blob/master/packages/eslint-config-edx/README.md)
- [the README for `eslint-config-edx-es5`](https://github.com/edx/eslint-config-edx/blob/master/packages/eslint-config-edx-es5/README.md)
