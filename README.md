# Shell help

I started this after becoming frustrated at various `man` and `--help`
pages that do not provide decent examples.

My thought is to record basic shell tasks I have had to search for in a
central repo that I (and hopefully others) will find useful.


## Getting started

You can view these pages on [GitHub][1] or install for console access.
Make sure you have [Node.js](http://nodejs.org/) installed.

	npm install -g shelp

You need to install it globally to get the `shelp` command.

[1]: https://github.com/MattMS/shelp/tree/master/command


## Goals

- All content in basic Markdown.

- Content is sent to stdout so it can be piped to [less](command/less/)
  or other tools.

- Each code example should only have 1 paragraph before and/or after it.
