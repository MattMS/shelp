# cut

Busybox includes `cut`, thus Alpine Linux does.


## Fields (by delimiters)

Delimit on space, print second word only:

	echo 'a b c' | cut -d ' ' -f 2

Add `--complement` to remove the second word (shows all others).

Remove second and third columns (`c` and `d`), print all others:

	echo 'a b c d e f g' | cut -d ' ' -f 1-2,5-

Can remove multiple column sections, like `-f -2,4-5,7-`.
Make sure there is **no space between the ranges** when typing the command.


## Links

- [use space as a delimiter with cut command @ Stack Overflow](https://stackoverflow.com/questions/816820/use-space-as-a-delimiter-with-cut-command)

- [cut @ Wikipedia](https://en.m.wikipedia.org/wiki/Cut_%28Unix%29)
