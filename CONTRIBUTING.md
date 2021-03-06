Contributing
===

## Prerequisites

1. Install the appropriate [EditorConfig](http://editorconfig.org) plugin for your IDE / editor. This helps keep the code style consistent.
2. Install [PhantomJS](http://phantomjs.org). Make sure it's on your path / available when calling `phantomjs` from the command line.
2. `npm install -g grunt-cli`
3. `npm install`

## Running the tests

- All tests: `npm test`
- Just the browser ones: `phantomjs phantom.js`
- Just the Node ones: `grunt test-node`

## Before creating the pull-request

Make sure you do the following:

- Run `grunt`

Note: The build script will generate new `*.min.{css,js}` files. If, for example, you only changed the JavaScript then don't bother committing `emojify.min.css`.

## Publishing

If you have rights to publish to npm, do the following first:

- Run `update.sh`. This will update the project with the latest emoji from [emoji-cheat-sheet.com](http://www.emoji-cheat-sheet.com). 
- Run `grunt`