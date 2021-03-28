## Level 6

**URL**: [Level 5](http://natas5.natas.labs.overthewire.org/)

 1. This step tells us that we have not logged in.
	 > **Note:** Also, the password save notification was not displayed.
 2. See the cookies.
 3. We have a cookie called loggedin with content 0.
 4. go to the `Developer Tools` (Ctrl-Shift-J or `Tools -> Developer Tools`) `-> Console` and enter javascript command:
	 ```  javascript
	document.cookie="loggedin=1"
	 ```
5. Refresh the page.