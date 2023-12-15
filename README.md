# fix-dns-wsl2
# Refer to link for possible fix
https://gist.github.com/coltenkrauter/608cfe02319ce60facd76373249b8ca6 

else

# FLush dns by running following commands in powershell as admin
```bash
wsl --shutdown
netsh winsock reset
netsh int ip reset all
netsh winhttp reset proxy
ipconfig /flushdns
``` 
