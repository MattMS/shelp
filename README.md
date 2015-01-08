# Shell help

This was created to fill in for the various `man` and `--help` pages
missing decent examples.

The focus is clear examples and explanations of shell tasks.


## View online or install

You can view these pages on
[GitHub](https://github.com/MattMS/shelp/tree/master/command#readme)
or install the
[Node.js](http://nodejs.org/) package for console access.

	npm install -g shelp

It needs to be installed globally to provide the `shelp` command:

	shelp npm ls


## Goals

- All content is in basic Markdown.
  72 columns is preferred, where possible.

- Content is sent to stdout so it can be piped to [less](command/less/)
  or other display tools.

- Each example should only have 1 paragraph before and/or after it.
  This is not a fixed rule, but encourages simple explanations.

- All that said, any help is better than no help.
  It can always be cleaned up later.
