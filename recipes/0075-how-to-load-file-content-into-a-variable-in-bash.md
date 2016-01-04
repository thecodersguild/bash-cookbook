#How to Load File Content into a Variable in Bash

Assuming you have an ASCII text file named `foobar.txt` and you want to load its contents into a variable use the following syntax _(note these are **parenthesis, not braces**!):_

    variable=$(cat foobar.txt)
    
This is a full example that will echo `Hello World!`:

    $ echo Hello World! > foobar.txt
    $ message=$(cat foobar.txt)
    $ echo $message


Remember; **do not add spaces around the equals ('`=`') sign**:

    $ echo Hello World! > foobar.txt
    $ message = $(cat foobar.txt)
    $ echo $message

