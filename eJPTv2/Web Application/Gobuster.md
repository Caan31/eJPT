Herramienta para descubrir directorios, archivos y subdominios.

• Fuzzing de rutas web  
• Descubrimiento de endpoints ocultos  
• Muy usada en enumeración

---

## Directory Bruteforce

```
sudo gobuster dir -u http://IP -w /DICCIONARY -t 4 -x php,txt,html
```

---

## Parámetros importantes

### -u

URL objetivo.

	-u http://192.168.1.10

---

### -w

Diccionario de rutas.

	-w /usr/share/wordlists/dirb/common.txt

---

### -t

Número de threads.

	-t 4

---

### -x

Extensiones a buscar.

	-x php,html,txt

---

### -s

Filtrar por códigos de estado.

	-s 200,301,302

---

### -b

Excluir códigos de estado.

	-b 404