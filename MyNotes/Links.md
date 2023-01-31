# Fetch Links
### https://github.com/jaeles-project/gospider
```gospider -s "[TARGET URL]" -c 10 -d 5 --blacklist ".(jpg|jpeg|gif|css|tif|tiff|png|ttf|woff|woff2|ico|pdf|svg|txt)" --other-source | grep -e "code-200" | awk '{print $5}'```
