Técnicas para romper hashes y obtener contraseñas.

• Ataques de diccionario  
• Fuerza bruta  
• Uso de GPU (Hashcat)

---

## John The Ripper

Herramienta para crackear hashes.

```
john fichero --wordlist=/DICCIONARIO
```

---

## Listar formatos (John)

```
john --list=formats
```

---

## Hashcat

Herramienta avanzada para cracking con GPU.

```
hashcat --help
```

---

## Ataque con Hashcat

```
hashcat -a 0 -m 0 example.hash /DICCIONARIO
```

---

## Parámetros importantes

### -a

Modo de ataque.

	-a 0   # diccionario  
	-a 3   # fuerza bruta

---

### -m

Tipo de hash.

	-m 0   # MD5  
	-m 1000 # NTLM



https://crackstation.net/