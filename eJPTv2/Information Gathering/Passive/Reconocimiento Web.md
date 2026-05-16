Herramientas usadas para recolectar información de aplicaciones web antes de la explotación:

• Identificar tecnologías  
• Encontrar archivos sensibles  
• Descubrir endpoints  
• Obtener información del dominio

### robots.txt

Archivo que indica a los bots que rutas no se deben de indexar, es útil para encontrar directorios ocultos.

`http://target.com/robots.txt`
### sitemap.xml

Mapa del sitio que contiene todas las rutas indexadas.

`http://target.com/sitemap.xml`
### Wappalyzer

Es una extensión de los navegadores para identificar tecnologías de un sitio web como:

- Lenguajes
- Servidores
- CMS
- Frameworks
### whatweb

Identifica teconologias web mediante la consola de comandos, (fingerprinting)

`whatweb http://target.com`

	-v      -> verbose
	-a 3    -> nivel de agresividad
### whois

Obtiene información del dominio

- Propietario
- Fecha de registro
- DNS
- Información del registrador
### dnsrecon -d 

Herramienta para enumeración DNS

- Enumera subdominios
- Transferencias de zona
- Información de DNS

```
dnsrecon -d target.com
```

	-d -> dominio
