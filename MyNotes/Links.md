# Fetch Links
## One target
### https://github.com/jaeles-project/gospider
```gospider -s "[TARGET URL]" -c 10 -d 5 --blacklist ".(jpg|jpeg|gif|css|tif|tiff|png|ttf|woff|woff2|ico|pdf|svg|txt)" --other-source | grep -e "code-200" | awk '{print $5}'```


### https://github.com/projectdiscovery/katana
```katana -u "[TARGET URL]" -d 5 -jc -aff -hl -kf -silent -ef jpg,jpeg,gif,css,tif,tiff,png,ttf,woff,woff2,ico,pdf,svg,txt```



## List of targets
### https://github.com/jaeles-project/gospider
```gospider -S "[PATH TO TARGETS FILE]" -c 10 -d 5 --blacklist ".(jpg|jpeg|gif|css|tif|tiff|png|ttf|woff|woff2|ico|pdf|svg|txt)" --other-source | grep -e "code-200" | awk '{print $5}'```

### https://github.com/projectdiscovery/katana
```while read target; do katana -u "$target" -d 5 -jc -aff -hl -silent -kf -ef jpg,jpeg,gif,css,tif,tiff,png,ttf,woff,woff2,ico,pdf,svg,txt >> [PATH TO OUTPUT LINKS FILE] ; done < [PATH TO TARGETS FILE]```
