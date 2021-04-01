## Level 7

**URL**: [Level 6](http://natas6.natas.labs.overthewire.org/)

 1. Go to View sourcecode
 2. The following line represents a directory and the corresponding file:
	 ```
	 include "includes/secret.inc";
	 ```
 4. Go to http://natas6.natas.labs.overthewire.org/includes/secret.inc
 5. In step one, the line below asks us to enter the value of the $secret variable into the main site
	 ```  
	if($secret == $_POST['secret'])
	 ```
5. Enter the $secret value and submit.