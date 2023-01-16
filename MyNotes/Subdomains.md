# Passive
### https://github.com/OWASP/Amass
amass enum -passive -d [exampledomain.com]

### https://github.com/projectdiscovery/subfinder
subfinder -all -d [exampledomain.com] -silent

## Certs
### https://github.com/UnaPibaGeek/ctfr
python3 ctfr.py -d [exampledomain.com] -o [OUTPUT PATH]

# Active
## DNS Brute force

### https://github.com/projectdiscovery/dnsx
 dnsx -silent -d [exampledomain.com] -w [PATH TO SUBDOMAINS WORDLIST]
