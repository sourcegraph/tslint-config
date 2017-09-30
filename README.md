
# Sourcegraph TSLint config

[![Version](https://img.shields.io/npm/v/@sourcegraph/tslint-config.svg)](https://www.npmjs.com/package/@sourcegraph/tslint-config)
[![Downloads](https://img.shields.io/npm/dt/@sourcegraph/tslint-config.svg)](https://www.npmjs.com/package/@sourcegraph/tslint-config)

TSLint rules for TypeScript projects at Sourcegraph.

## Usage

```
npm install --save-dev @sourcegraph/tslint-config
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

