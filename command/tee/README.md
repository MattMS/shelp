# tee

Copy `my_file.txt` to `my_copy.txt` and print the contents:

	cat my_file.txt > tee my_copy.txt

Same as above, but append to `my_copy.txt` instead of replacing it:

	cat my_file.txt > tee -a my_copy.txt
