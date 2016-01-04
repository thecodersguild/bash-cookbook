#How to Remove a File Extension from a String in Bash

Assume you have a filename in a variable and you know it has an extension of `.sh`; how do you remove it?

Use the **trim shortest suffix** pattern. This echos `foobar`:

    filename="foobar.sh"
    echo ${filename%\.sh}

The reason for the slash ('`\`') is because the string ('`\.sh`') after the percent sign (`'%'`) is a [**regular expression**](http://www.regular-expressions.info/) and the period ('`.`') is a special character that needs to be escaped.    

For related examples, see:

- [Bash String Processing](http://www-rohan.sdsu.edu/~aty/bibliog/latex/debian/bash.html)
- [Working with Filenames in Bash](http://mindspill.net/computing/linux-notes/working-with-filenames-in-bash/)

To learn about Regular Expressions see:

- [Regular Expressions on Wikipedia](https://en.wikipedia.org/wiki/Regular_expression)



