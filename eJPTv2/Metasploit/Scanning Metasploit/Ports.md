Módulos auxiliares usados para descubrir puertos abiertos en un objetivo.

• Escaneo TCP  
• Escaneo UDP  
• Identificación de servicios

### TCP Port Scan

Utiliza conexiones TCP para determinar que puertos están abiertos. 

```
use auxiliary/scanner/portscan/tcp
```
	
	set RHOSTS IP

### UDP Sweep

Escanea puertos UDP para detectar servicios activos.

```
use auxiliary/scanner/discovery/udp_sweep
```
	
	set RHOSTS IP