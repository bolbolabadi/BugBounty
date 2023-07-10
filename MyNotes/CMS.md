# Find CMS

### Wordpress
cat all-live-subs.txt | httpx -silent -H "User-Agent: Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)" -mc 200,301,302 -match-regex "X-Powered-By: W3 Total Cache|wp-content|wp-includes|xmlrpc.php" -o all-wordpress.txt -timeout 10 

