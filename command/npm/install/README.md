# npm install

Install a package from NPM repositories.


## Install a command-line tool (globally)

	npm install -g shelp

Or

	npm install --global shelp

You can then run `shelp` in any folder.


## Save a project dependency

Make sure you have run `npm init` to get a `package.json` first!

	npm install express --save

This will add `express` to `dependencies` in `package.json`.


## Save a project development dependency

Save packages you need during development, but users do not need to use
the package.

	npm install coffee-script --save-dev

This will add `coffee-script` to `devDependencies` in `package.json`.
