##How to Get Bash to Recognize a Shell Script

Many programs recognize files based on their extensions, but not Bash. To indicate to Bash that it should process a file as a shell script [**you need to add a _"shebang"_ header**](https://en.wikipedia.org/wiki/Shebang_%28Unix%29) as **the first line** in the file:

	#!/usr/bin/env bash

Note that you might see this in some files instead:

    #!/bin/bash

This blog post explains [why the former is better than the latter](http://www.cyberciti.biz/tips/finding-bash-perl-python-portably-using-env.html).

###The .sh extension
An `.sh` extension is only a convention and does not indicate to Bash that it is a shell script. This differs from the Windows command processor that looks for the `.bat` file extensions to indicates it should process the file as a _"batch"_ file.

However, many people who write shell scripts use a different extension or omit the extension entirely because *nix systems does not recognize the `.sh` extension as special.



