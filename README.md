**HTTPS redirect for Wordpress**

<code>RewriteCond %{SERVER_PORT} 80 <br>
RewriteRule ^(.*)$ https://ppsd.com/$1 [R,L] </code>

**Create files in each directory of current location**

<code>find . -type d -exec touch {}/index.html \;</code>
