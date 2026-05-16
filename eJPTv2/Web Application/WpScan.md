Herramienta para enumerar y analizar vulnerabilidades en WordPress.

• Detecta plugins y temas  
• Enumera usuarios  
• Identifica vulnerabilidades

---

## Escaneo básico

```
wpscan --url http://IP -v
```

## Enumerar usuarios

```
wpscan --url http://IP -e u
```

---

## Enumerar plugins

```
wpscan --url http://IP -e p
```

---

## Enumerar todo

```
wpscan --url http://IP -e u,p,t
```

---

## Fuerza bruta

```
wpscan --url http://wordpress.local -U admin -P /usr/share/wordlists/rockyou.txt
```
