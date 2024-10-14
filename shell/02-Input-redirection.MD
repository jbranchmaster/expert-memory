# Shell Input Redirection

# How it works
 - [Source](https://superuser.com/questions/1003760/what-does-eof-do)
 - `cat` is the command
 - Here the shell interprets the `<<` operator as an instruction to read input until it finds a line containing the specified delimiter
 - All the input lines up to the line containing the delimiter are then fed into the standard input of the command. e.g we pass `document` to `cat` command and redirect the output to a file.
   ```
   cat << delimiter > test.yaml
   document
   delimiter
   ```
