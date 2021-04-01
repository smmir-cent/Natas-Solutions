## Level 9

**URL**: [Level 8](http://natas8.natas.labs.overthewire.org/)

 1. [View sourcecode](http://natas8.natas.labs.overthewire.org/index-source.html)
	 ``` php
	   $encodedSecret = "3d3d516343746d4d6d6c315669563362";  
		function encodeSecret($secret) {  
			return bin2hex(strrev(base64_encode($secret)));  
		}  
		if(array_key_exists("submit", $_POST)) {  
			if(encodeSecret($_POST['secret']) == $encodedSecret) {  
					print "Access granted. The password for natas9 is <censored>";  
				} else {  
				print "Wrong secret";  
				}  
		}
	```

2. According to the following line, we need to do the reverse operation of the encodeSecret function with the value given for $encodedSecret:
	 ``` 
	 if(encodeSecret($_POST['secret']) == $encodedSecret)
	 ```
	 	 
 3. Execute the following code and get the input secret value and submit:
	 ```php
	 echo base64_decode(strrev(hex2bin("3d3d516343746d4d6d6c315669563362")));
	```
