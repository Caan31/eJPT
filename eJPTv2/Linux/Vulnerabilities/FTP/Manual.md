Servicio que permite transferencia de archivos entre cliente y servidor.

• Subida y descarga de archivos  
• Puede permitir acceso anónimo  
• Usa puerto 21

---

## Fuerza bruta (Hydra)

Ataque de credenciales contra FTP.

```
hydra -L USERS -P PASSWORD IP -t4 ftp 
```

## Acceso FTP

Conexión al servicio.

```
ftp IP
```

## Login anónimo

```
USER: anonymous
PASS: anonymous
```

## Comandos útiles

```
ls
get file.txt
put file.txt
```


• Probar acceso anónimo primero  
• Revisar permisos de escritura  
• Puede permitir subir webshells
