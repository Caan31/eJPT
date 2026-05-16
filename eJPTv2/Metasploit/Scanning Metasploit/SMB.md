Módulos para enumeración y acceso a servicios SMB (Windows).

• Enumerar versión  
• Usuarios  
• Recursos compartidos  
• Fuerza bruta

## SMB Version

Obtiene información del servicio SMB.

Permite identificar:  
- Versión de SMB  
- Sistema operativo  
- Nombre del host

```
use auxiliary/scanner/smb/smb_version
```
	
	set RHOSTS IP

## SMB Enum Users

Enumera usuarios del sistema.

```
use auxiliary/scanner/smb/smb_enumusers
```
	
	set RHOSTS IP

## SMB Enum Shares

Enumera recursos compartidos.

```
use auxiliary/scanner/smb/smb_enumshares
```
	
	set RHOSTS IP
	set ShowFiles true

## SMB Login (Brute Force)

Ataque de fuerza bruta contra SMB.

```
use auxiliary/scanner/smb/smb_login
```
	
	set RHOSTS IP
	set SMBUser USER
	set PASS_FILE DICCIONARIO


## Acceso manual con credenciales

Permite listar recursos compartidos manualmente:

``smbclient -L \\\\IP\\ -U user ``

