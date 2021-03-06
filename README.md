# QRCode Terminal Edition [![Build Status][travis-ci-img]][travis-ci-url]

> Going where no QRCode has gone before.

![Basic Example][basic-example-img]

# Node Library

## Install

Can be installed with:

    $ npm install qrcode-terminal

and used:

    var qrcode = require('qrcode-terminal');

## Usage

To display some data to the terminal just call:

    qrcode.generate('This will be a QRCode, eh!');

If you don't want to display to the terminal but just want to string you can provide a callback:

    qrcode.generate('http://github.com', function (qrcode) {
        console.log(qrcode);
    });

# Command-Line

## Install

    $ npm install -g qrcode-terminal

## Usage

    $ qrcode-terminal --help
    $ qrcode-terminal 'http://github.com'

# Support

- OS X
- Linux
- Windows

# Server-side

[node-qrcode][node-qrcode-url] is a popular server-side QRCode generator that
renders to a `canvas` object.

# Developing

To setup the development envrionment run `npm install`

To run tests run `npm test`

# Contributers

    Gord Tanner <gtanner@gmail.com>
    Micheal Brooks <michael@michaelbrooks.ca>

[travis-ci-img]: https://travis-ci.org/gtanner/qrcode-terminal.png
[travis-ci-url]: https://travis-ci.org/gtanner/qrcode-terminal
[basic-example-img]: https://raw.github.com/gtanner/qrcode-terminal/master/example/basic.png
[node-qrcode-url]: https://github.com/soldair/node-qrcode

