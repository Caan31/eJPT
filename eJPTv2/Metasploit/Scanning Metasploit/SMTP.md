Módulos para enumeración de servicios SMTP (correo).

• Identificar versión  
• Enumerar usuarios  
• Recolección de información

## SMTP Version

Obtiene la versión del servicio SMTP.

Permite identificar:  
• Software (Postfix, Exim, Sendmail)  
• Versión  
• Banner del servidor

```
use auxiliary/scanner/smtp/smtp_version 
```
	
	set RHOSTS IP

## SMTP Enum

Enumera usuarios válidos en el servidor SMTP.

Utiliza comandos como:  
• VRFY  
• EXPN  
• RCPT TO

```
use auxiliary/scanner/smtp/smtp_enum
```
	
	set RHOSTS IP 
	set USER_FILE DICCIONARY
