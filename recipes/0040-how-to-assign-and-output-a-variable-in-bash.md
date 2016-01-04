#How to Assign and Output a Variable in Bash

Variables in Bash can be tricky if you have experience with other languages. Read on.

###Variable Assignment

The following assign the value `'bar'` to the variable `foo`:

    foo=bar

This _**DOES NOT**_ assign to the variable `foo` _(so avoid spaces around your '`=`' sign or your will be pulling your hair out!):_

    foo = bar


###Variable Output

This outputs `bar` which is the value of `foo`:

    echo $foo


This also outputs `bar`:

    echo ${foo}    

And this too outputs `bar`:

    echo "${foo}"    

This _**DOES NOT**_ output `bar` _(it outputs `foo`):_

    echo foo

