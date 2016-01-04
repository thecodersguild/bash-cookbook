##How to Execute a Bash Shell Script on Mac OS X 

You write a shell script and try to run it and Bash says _"Permission denied"_; **why?**

Let's show an example:

    $ echo 'echo Hello!' > foo.sh 
    $ ./foo.sh
    -bash: ./foo.sh: Permission denied

You need to **grant file execution permissions**:

    $ chmod +x foo.sh 
    $ ./foo.sh
    Hello!

