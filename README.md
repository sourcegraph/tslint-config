
# Sourcegraph TSLint config

[![npm](https://img.shields.io/npm/v/@sourcegraph/tslint-config.svg)](https://www.npmjs.com/package/@sourcegraph/tslint-config)
[![downloads](https://img.shields.io/npm/dt/@sourcegraph/tslint-config.svg)](https://www.npmjs.com/package/@sourcegraph/tslint-config)
[![build](https://travis-ci.org/sourcegraph/tslint-config.svg?branch=master)](https://travis-ci.org/sourcegraph/tslint-config)
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)

The last remaining TSLint rules for TypeScript projects at Sourcegraph that are not yet supported by ESLint.
Must be used in conjunction with [`@sourcegraph/eslint-config`](https://www.npmjs.com/package/@sourcegraph/eslint-config).

## Usage

```
npm install --save-dev @sourcegraph/tslint-config@eslint
```

Then add this tslint.json:

```json
{
  "extends": "@sourcegraph/tslint-config"
}
```

## Making changes

```
npm link
cd <project>
npm link @sourcegraph/tslint-config
npm run lint
```

## Publish a new version

Follow [semver](http://semver.org/).

```
npm version major|minor|patch
git push
git push --tags
npm publish
```

