# screen

`Ctrl + d` to exit screen.


## Detach then return

Start `screen` and then a command:

	screen
	top

Type `Ctrl + a` then `d` to detach from screen.
This returns to the terminal, where screen was called.

When ready to return to the screen:

	screen -r


## Keyboard controls

`Ctrl + a` then:

- `?` (`Shift + /`) shows commands and defaults.

- `c` create new screen.

- `n` for next screen, `p` for previous.

- `x` to lock the screen.


## Links

- [GNU Screen (ArchWiki)](https://wiki.archlinux.org/index.php/GNU_Screen)
