Servicio que permite compartir archivos e impresoras en red entre sistemas (Windows/Linux).

• Compartición de archivos  
• Autenticación por usuario  
• Usa puerto 445

---

## Fuerza bruta (Hydra)

Ataque de credenciales contra SMB.

```
hydra -L USERS -P PASSWORD IP smb
```

## SMBMap

Enumera recursos compartidos y permisos.

```
smbmap -H IP -u USER -p PASSWORD
```

## SMBClient (Listar recursos)

Lista shares disponibles.

```
smbclient -L IP -U USER
```

## SMBClient (Conexión)

Accede a un recurso compartido.

```
smbclient  //IP/ -U USER
```

## Enum4linux

Herramienta para enumeración completa de SMB.

```
enum4linux -a IP 
```



• SMB suele tener información sensible  
• Buscar shares con permisos de escritura
