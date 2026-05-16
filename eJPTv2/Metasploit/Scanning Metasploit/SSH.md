Módulos para enumeración y acceso a servicios SSH.

• Identificar versión  
• Fuerza bruta  
• Acceso remoto

## SSH Version

Obtiene la versión del servicio SSH.

Permite identificar:  
• Software (OpenSSH, etc.)  
• Versión  
• Posibles vulnerabilidades

```
use auxiliary/scanner/ssh/ssh_version
```
	
	set RHOSTS IP 

## SSH Login (Brute Force)

Ataque de fuerza bruta contra SSH.

```
use auxiliary/scanner/ssh/ssh_login
```
	
	set RHOST IP
	set USER_FILE DICCIONARY
	set PASS_FILE DICCIONARY


### STOP_ON_SUCCESS
Detiene el ataque al encontrar credenciales válidas.