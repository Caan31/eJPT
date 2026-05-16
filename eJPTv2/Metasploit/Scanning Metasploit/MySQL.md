Módulos para enumeración y acceso a bases de datos MySQL.

• Identificar versión  
• Fuerza bruta  
• Ejecución de queries  
• Dump de bases de datos

## MySQL Version

Obtiene la versión del servicio MySQL.

Permite identificar:  
• Versión  
• Posibles vulnerabilidades

```
use auxiliary/scanner/mysql/mysql_version
```
	
	set RHOSTS IP

## MySQL Login (Brute Force)

Ataque de fuerza bruta contra MySQL.

```
use auxiliary/scanner/mysql/mysql_login
```
	
	set RHOSTS IP
	set USER_FILE DICCIONARY
	set PASS_FILE DICCIONARY

## MySQL SQL (Ejecutar comandos)

Permite ejecutar queries SQL en la base de datos.

```
use auxiliary/admin/mysql/mysql_sql
```
	
	set RHOSTS IP
	set USERNAME USER  
	set PASSWORD PASS
	set SQL show databases; (LENGUAJE SQL)

## MySQL Schema Dump

Extrae información de la base de datos.

Permite:  
• Listar tablas  
• Obtener estructura  
• Enumerar datos

```
use auxiliary/scanner/mysql/mysql_schemadump
```
	
	set RHOSTS
	set USERNAME USER  
	set PASSWORD PASS


## Acceso manual

Conexión directa al servicio MySQL:

```
mysql -h IP -u USER -p 
```