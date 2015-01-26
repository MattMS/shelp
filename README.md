# Shell help

Shelp was created to help out the various `man` and `--help` pages
missing decent examples.

The aim is examples of common shell tasks with details on when and why
you would use them.


## View online or install

You can
[view these pages on GitHub](https://github.com/MattMS/shelp/tree/master/command#readme)
or
[install the package from NPM](https://www.npmjs.com/package/shelp)
for console access:

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
