Script en PowerShell para detectar posibles vectores de escalada de privilegios.

• Enumera configuraciones débiles  
• Detecta servicios vulnerables  
• Sugiere vectores de PrivEsc

https://github.com/itm4n/PrivescCheck

## Ejecutar PrivEscCheck

```
powershell -ep bypass -c ". .\PrivescCheck.ps1; Invoke-PrivescCheck"
```

## Qué analiza

• Servicios mal configurados  
• Permisos inseguros  
• Credenciales expuestas  
• Configuración del sistema