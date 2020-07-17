# gfPats

### copy all json files to .gf folder
``` cp *.json ~/.gf/ ```

##  gf and paramspider tricks <3 
```
paramspider host.com ; cat output/host.com | gf rce | tee -a attack/possible-rce.txt 

```
## subfinder /waybackurl/gau  / httprobe
```
subfinder -d host.com -silent | httprobe -c 50 -t 20000 | waybackurl | gf rce2 | tee -a attack/possible-rce.txt 
```
