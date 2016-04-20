**HTTPS redirect for Wordpress**

<code>RewriteCond %{SERVER_PORT} 80 <br>
RewriteRule ^(.*)$ https://example.com/$1 [R,L] </code>

**Create files in each directory of current location**

<code>find . -type d -exec touch {}/index.html \;</code>

**List and link all first level children**

<code>
<?php
					$directories =  array_filter(glob("./*", GLOB_ONLYDIR));
					for($x = 0; $x < count($directories); $x++){
						//if we're at the current location, make sure to add the active class to represent that
						echo '<li><a href="'.$directories[$x].'">'.str_replace("./", "", str_replace("-", " ", $directories[$x])).'</a></li>';
					}
					?></code>
