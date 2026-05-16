Técnicas para escalar privilegios dentro del sistema comprometido.

• Obtener acceso root/admin  
• Aprovechar vulnerabilidades locales  
• Uso de credenciales y configuraciones débiles

## Kernel Exploit

Escalada mediante vulnerabilidades del kernel.


	getprivs -> Muestra privilegios disponibles.


	getsystem -> Intenta escalar privilegios automáticamente.

## Local Exploit Suggester

Sugiere exploits locales según el sistema.

 La sesión debe estar en background:


```
use post/multi/recon/local_exploit_suggester
```
	set SESSION ID
