#How to Remove a File Extension from a String in Bash

Assume you have a filename in a variable and you know it has an extension of `.sh`; how do you remove it?

Use the **trim shortest suffix** pattern: 

    filename="foobar.sh"
		echo ${filename%\.sh}
    
This echos `foobar`:

For more examples, see:

- [Bash String Processing](http://www-rohan.sdsu.edu/~aty/bibliog/latex/debian/bash.html)



