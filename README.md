# quick-password-protect-reference
I've been asked a few times in different situations to quickly lock something from public view on a web server. I'm adding this as a reference for anyone looking quickly password protect a file/folder on a server (including myself).

1. Copy/paste these two files (.htaccess and .htpassword) into the directory you want to password protect.

2. Change the info in the .htaccess file "AuthUserFile" to match the path to your .htpasswd file.

3. Change the info in the .htpasswd file with the password hashed with an algorithm appropriate for your server, no spaces between, just ':'.

4. Test everything! Test it incogneto, test it with the wrong credentials, test it however you can think of - this is just a starter template for doing this, please test it yourself before using it! Please Google everything to make sure everything checks out before using -i'm not a security expert but have used similar ways as this to quickly + <ins>temporarily</ins> lock folders that where for clients.


### Note: If you just want to completely block a folder / item you could also change the permision of the folder / file on the server - this is for granting access through a name/password combo. 