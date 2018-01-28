# Tomatoes

The Real Junk Food Project Sheffield has *a lot* of tomatoes to distribute. (https://realjunkfoodsheffield.com/tomatoes/)

This is some work trying to do some interesting visualisations of how much has been claimed.

# Notes

The only real magic is getting apache to pass the svg files through php

```
	<Directory "/psvg/">
		<FilesMatch \.svg$>
    			SetHandler application/x-httpd-php
		</FilesMatch>
	</Directory>
```