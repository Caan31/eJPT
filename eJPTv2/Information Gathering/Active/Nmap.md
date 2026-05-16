
Herramienta Nmap Network Mapper es una herramienta de escaneo de redes usada para:

• Descubrir hosts activos
• Detectar puertos abiertos
• Identificar servicios
• Detectar versiones
• Hacer una enumeración

## Escaneo de hosts:

### **-sn**
Envia pings a todas las IP de la red especificada y al detectar las que responden muestran todos los hosts activos.

```
nmap -sn X.X.X.X/X
```

## Escaneo de UDP:

### **-sU**
Envía paquetes UDP a los puertos del hosts, analiza si recibe respuestas o errores y determina el estado de los puertos

## Herramientas de escaneo:

### -sS
Lo que hace es enviar un paquete SYN, si recibe SYN ACK es que tiene puerto abierto, es discreto y bastante usado en pentesting. 

### -Pn
No ping, si el firewall bloquea ICMP, nos saltamos esta comprobación, es recomendable solo hacerlo si tenemos bloqueado el ICMP, ya que esto causa bastante ruido. 

### -sC
Ejecuta los scripts NSE por defecto. 

Se puede ejecutar un script especifico añadiendo el siguiente parametro.

`--script=`
### -sV
Detecta versiones del servicio para poder buscar exploits o tener más información del servicio.

### -p-
Escanea todos los puertos ya que nmap por defecto escanea solo los 1000 mas comunes 

### -p PUERTOS
Se especifica los puertos abiertos que hemos encontrado en la primera fase.

### -p 1-1000
Especificamos un rango de puertos que queremos que escanee 
### -T
Timing template, esto reduce tiempos de espera, aumenta velocidad de envío, depende si queremos hacer poco o menos ruido de T0 al T5.

### -v
very very verbose, esto nos da detalles en tiempo real, el progreso del escaneo solo es algo visual. 

### -O 
detectar el sistema operativo del dispositivo que estás escaneando.

### -oN
Lo guardamos en un archivo para luego mirarlo.

## Primera fase: 

Haremos un escaneo completo de los puertos para identificar los que hay abiertos

```
sudo nmap -sS -Pn -T4 -O -p- X.X.X.X -oN puertos_abiertos
```

## Segunda fase

Una vez sepamos los puertos abiertos, escaneamos nuevamente pero averiguaremos la versión especifica de cada servicio. 

```
sudo nmap -sS -Pn -sCV -T5 -O -vv -pPUERTOS X.X.X.X -oN puertos_versiones
```


## Evasión IDS 

### -f 

fragmenta los paquetes enviados en fragmentos más pequeños para evadir IDS que no reensamblan bien. 

### --data-length 

Agrega datos aleatorios al paquete, para hacerlo menos reconocible

### -g

Especifica el puerto de origen, esto hace parecer que el trafico pueda provenir de un puerto confiable.

### -D 

Usa señuelos, para que parezca que viene de multiples IPs