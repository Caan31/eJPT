Módulos para enumerar y atacar servicios FTP.

• Identificar versión  
• Fuerza bruta de credenciales  
• Acceso anónimo

## FTP Versión

Obtiene la versión del servicio FTP.

Permite identificar:  
- Software  
- Versión  
-  Posibles vulnerabilidades

```
use scanner/ftp/ftp_version
```
	
	set RHOSTS IP

## FTP Login (Brute Force)

Realiza ataque de fuerza bruta contra el servicio FTP.

```
use scanner/ftp/ftp_login
```
	
	set USER_FILE DICCIONARY
	set PASS_FILE DICCIONARY



### THREADS

Número de intentos simultáneos.

• Más rápido = más ruido  
• Menos = más sigiloso