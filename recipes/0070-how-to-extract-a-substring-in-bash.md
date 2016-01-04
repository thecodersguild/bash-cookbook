#How to Extract a Substring in Bash in Mac OS X Terminal

To extract a substring from a string variable use colons to specify the position and the optional length:

    ${string:position}
    ${string:position:length}
    
This echos `barbaz`:

    $ string=foobarbaz
    $ echo ${string:3}

This echos `obar`:

    $ string=foobarbaz
    $ echo ${string:2:5}

For more examples, see:

- [Bash String Manipulation Examples – Length, Substring, Find and Replace](http://www.thegeekstuff.com/2010/07/bash-string-manipulation/)



