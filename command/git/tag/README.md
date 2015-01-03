# git tag

Tags are used to mark significant points in the commit history, such as
releases.


## List tags

	git tag

Prints tag names on separate lines.


## Add tag

Annotated tags are preferred over lightweight ones.


### Lightweight

	git tag my_light_tag

Only stores a pointer to the commit.


### Annotated

	git tag -a 1.0 -m "My version 1.0"

Stores the tagger name and email, date and message.


## View tag details

	git show my_tag_name

For lightweight tags this prints the commit details.
For annotated tags this prints the annotated details.
