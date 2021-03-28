## Level 5

**URL**: [Level 4](http://natas4.natas.labs.overthewire.org/)

 1. Note the following line of code when viewing the page source
	 ```
	 Access disallowed. You are visiting from "http://natas4.natas.labs.overthewire.org/" while authorized users should come only from "http://natas5.natas.labs.overthewire.org/"
	 ```
	 > **Note:** According to the text above, to get the password, we must enter step 4 from step 5.
 2. Go to [http://natas5.natas.labs.overthewire.org/](http://natas4.natas.labs.overthewire.org/) and select cancel to entering password.
 3. Go to Inspect (Ctrl+Shift+I)
 4. Add the HTML element below:
	 ``` html
	 <a href="http://natas4.natas.labs.overthewire.org/"> Go to natas4 </a>
	 ```