---
title: Setup HTML5
---

Lime and OpenFL may be used to create [HTML5](https://developer.mozilla.org/en-US/docs/Glossary/HTML5) applications and games for web browsers by [compiling to JavaScript](https://haxe.org/manual/target-javascript.html)

## Automatic Install

There is no automatic setup available for HTML5.

## Manual Install

There is generally no setup required for the HTML5 target.

## Build & Run

To compile an HTML5 application, run `lime build html5`.

To compile and launch an HTML5 application with one command, run `lime test html5`. This will start a local development server, and launch the page in a web browser.

### Minification

Adding either the `-minify` option or the `-final` option to your build command will apply more advanced minification to the generated JavaScript. By default, [Closure Compiler](https://developers.google.com/closure/compiler) will be used to minify, but you can specify `-yui` to use [YUI Compressor](https://yui.github.io/yuicompressor/) instead. Both minification tools require Java to be installed.

### Launch Options

The default port used by the local development server is port `3000`. To customize this port, specify the `--port` option with a value such as `--port=8080`.

To compile and start the local development server, but skip launching in a web browser, add the `-nolaunch` option.

## Using JavaScript libraries

To use an external JavaScript library with Lime, you need [Haxe externs](https://haxe.org/manual/lf-externs.html). See also [Haxe: Using external JavaScript libraries](https://haxe.org/manual/target-javascript-external-libraries.html).

Members of the Haxe community have already created open source externs for a number of popular JavaScript libraries, so be sure to search [Haxelib](https://lib.haxe.org/search) or [Github](https://github.com/search) to see if JS externs exist for your library before you try to create your own.

## Forums

If you encounter any problems when setting up Lime for HTML5, please visit the [forums](http://community.openfl.org/c/help).
