Módulos para enumeración de servicios HTTP.

• Identificar servidor web  
• Obtener headers  
• Descubrir directorios  
• Enumerar usuarios  
• Ataques de login


## HTTP Version

Obtiene información del servidor web.

Permite identificar:  
• Tipo de servidor (Apache, Nginx, IIS)  
• Versión

```
use auxiliary/scanner/http_version 
```
	
	set RHOSTS IP

## HTTP Headers

Obtiene los headers HTTP del servidor.

Útil para:  
• Información del servidor  
• Cookies  
• Seguridad

```
use auxiliary/scanner/http_header
```
	
	set RHOSTS IP

## Robots.txt

Obtiene rutas ocultas del archivo robots.txt.

```
use auxiliary/scanner/http/robots.txt
```
	
	set RHOSTS IP

## Directory Scanner

Busca directorios ocultos en el servidor web.

```
use auxiliary/scanner/http/dir_scanner
```
	
	set RHOSTS IP

## Files Directory

Enumera archivos dentro de directorios.

```
use auxiliary/scanner/http/files_dir
```
	
	set RHOSTS IP

## Apache UserDir Enum

Enumera usuarios en servidores Apache con UserDir habilitado.

```
use auxiliary/scanner/http/apache_userdir_enum
```
	
	set RHOSTS IP

## HTTP Login (Brute Force)

Ataque de fuerza bruta contra formularios web.

```
use auxiliary/scanner/http/http_login
```
	
	set AUTH_URI /secure/  -->  RUTA DEL LOGIN 
	unset USERPASS_FILE 
	set VERBOSE false

