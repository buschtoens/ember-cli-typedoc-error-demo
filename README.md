# ember-cli-typedoc-error-demo

This repository show cases an error when trying to run [typedoc](https://github.com/TypeStrong/typedoc)
for a fresh installation of [ember-cli-typescript](https://github.com/emberwatch/ember-cli-typescript).

```
$ yarn run generate-docs
yarn run v0.24.5
$ typedoc --out dist/docs

Using TypeScript 2.3.2 from /home/jan/github/ember-cli-typedoc-error-demo/node_modules/typedoc/node_modules/typescript/lib
/home/jan/github/ember-cli-typedoc-error-demo/node_modules/typedoc/dist/lib/converter/nodes/export.js:42
            symbol.declarations.forEach(function (declaration) {
                               ^

TypeError: Cannot read property 'forEach' of undefined
    at ExportConverter.convert (/home/jan/github/ember-cli-typedoc-error-demo/node_modules/typedoc/dist/lib/converter/nodes/export.js:42:32)
    at Converter.convertNode (/home/jan/github/ember-cli-typedoc-error-demo/node_modules/typedoc/dist/lib/converter/converter.js:126:53)
    at /home/jan/github/ember-cli-typedoc-error-demo/node_modules/typedoc/dist/lib/converter/nodes/block.js:85:29
    at Array.forEach (native)
    at BlockConverter.convertStatements (/home/jan/github/ember-cli-typedoc-error-demo/node_modules/typedoc/dist/lib/converter/nodes/block.js:84:26)
    at /home/jan/github/ember-cli-typedoc-error-demo/node_modules/typedoc/dist/lib/converter/nodes/block.js:62:27
    at Context.withScope (/home/jan/github/ember-cli-typedoc-error-demo/node_modules/typedoc/dist/lib/converter/context.js:107:9)
    at /home/jan/github/ember-cli-typedoc-error-demo/node_modules/typedoc/dist/lib/converter/nodes/block.js:61:25
    at Context.withSourceFile (/home/jan/github/ember-cli-typedoc-error-demo/node_modules/typedoc/dist/lib/converter/context.js:87:9)
    at BlockConverter.convertSourceFile (/home/jan/github/ember-cli-typedoc-error-demo/node_modules/typedoc/dist/lib/converter/nodes/block.js:58:17)
error Command failed with exit code 1.
info Visit https://yarnpkg.com/en/docs/cli/run for documentation about this command.
```

## Prerequisites

You will need the following things properly installed on your computer.

* [Git](https://git-scm.com/)
* [Node.js](https://nodejs.org/) (with yarn or npm)

## Installation

* `git clone git@github.com:buschtoens/ember-cli-typedoc-error-demo.git` this repository
* `cd ember-cli-typedoc-error-demo`
* `yarn`

## Executing typedoc

```
$ yarn run generate-docs
```
