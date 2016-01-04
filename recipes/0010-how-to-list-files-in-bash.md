##How to Get List Files in Bash in Mac OS X Terminal

Use the `ls` command _(in this example we'll list files in the hard disk's root folder):_

	ls /
	
The output is likely to look something like this although your computer will probably have more files and/or directories than this example:

	Applications     Volumes        sbin
	Library          bin            tmp
	Network          etc            usr
	System           opt            var
	Users            private
	          

To see a list of files in the _**current folder**_ just omit the slash ('`/`'):

	ls 
	
###List File Details in Full Terminal Width, _i.e. "Long" Format:_

Add the Long Format ('`-l`') switch

	ls -l /
	
The results will look something like this:

	drwxrwxr-x+ 394 root  admin  13396 Jan  2 01:44 Applications
	drwxr-xr-x+  77 root  wheel   2618 Dec 26 23:21 Library
	drwxr-xr-x@   2 root  wheel     68 Dec 26 23:17 Network
	drwxr-xr-x@   4 root  wheel    136 Dec 26 23:14 System
	drwxr-xr-x    7 root  admin    238 Dec 26 23:26 Users
	drwxrwxrwt@   5 root  admin    170 Jan  2 22:00 Volumes
	drwxr-xr-x@  39 root  wheel   1326 Dec  3 01:34 bin
	lrwxr-xr-x@   1 root  wheel     11 Dec 26 23:16 etc -> private/etc
	drwxr-xr-x@   8 root  wheel    272 Dec 27 01:56 opt
	drwxr-xr-x@   8 root  wheel    272 Dec 26 23:21 private
	drwxr-xr-x@  59 root  wheel   2006 Dec 26 23:16 sbin
	lrwxr-xr-x@   1 root  wheel     11 Dec 26 23:16 tmp -> private/tmp
	drwxr-xr-x@  13 root  wheel    442 Dec 27 02:11 usr
	lrwxr-xr-x@   1 root  wheel     11 Dec 26 23:16 var -> private/var
		          
Again, your results will likely include more files and directories.		          
			
###List _"All"_; Include Hidden Files and Folders Too _(.dot files & folders)_
Bash and other *nix shells treat files with a leading period ('`.`') as a hidden file.  

To include hidden files and folders in your listing add the _"All"_ Switch ('`-a`'):

	ls -al /

That adds the hidden files to your output: 
 
	drwxr-xr-x   43 root  wheel   1530 Jan  1 21:50 .
	drwxr-xr-x   43 root  wheel   1530 Jan  1 21:50 ..
	-rw-rw-r--    1 root  admin  12292 Dec 29 14:06 .DS_Store
	drwxr-xr-x+   3 root  wheel    102 Dec 28 22:25 .MobileBackups
	drwxr-xr-x+  11 root  wheel    374 Aug 18  2012 .ServerBackups
	drwx------    5 root  wheel    170 Apr  9  2015 .Spotlight-V100
	d-wx-wx-wt    2 root  wheel     68 Dec 26 22:07 .Trashes
	srwxrwxrwx    1 root  wheel      0 Jan  1 21:50 .dbfseventsd
	----------    1 root  admin      0 Sep 15 23:00 .file
	drwx------  621 root  wheel  21114 Jan  3 21:47 .fseventsd
	drwxr-xr-x@   2 root  wheel     68 Dec 26 23:17 .vol
	drwxrwxr-x+ 394 root  admin  13396 Jan  2 01:44 Applications
	drwxr-xr-x+  77 root  wheel   2618 Dec 26 23:21 Library
	drwxr-xr-x@   2 root  wheel     68 Dec 26 23:17 Network
	drwxr-xr-x@   4 root  wheel    136 Dec 26 23:14 System
	drwxr-xr-x    7 root  admin    238 Dec 26 23:26 Users
	drwxrwxrwt@   5 root  admin    170 Jan  2 22:00 Volumes
	drwxr-xr-x@  39 root  wheel   1326 Dec  3 01:34 bin
	lrwxr-xr-x@   1 root  wheel     11 Dec 26 23:16 etc -> private/etc
	drwxr-xr-x@   8 root  wheel    272 Dec 27 01:56 opt
	drwxr-xr-x@   8 root  wheel    272 Dec 26 23:21 private
	drwxr-xr-x@  59 root  wheel   2006 Dec 26 23:16 sbin
	lrwxr-xr-x@   1 root  wheel     11 Dec 26 23:16 tmp -> private/tmp
	drwxr-xr-x@  13 root  wheel    442 Dec 27 02:11 usr
	lrwxr-xr-x@   1 root  wheel     11 Dec 26 23:16 var -> private/var
				
