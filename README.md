<div align="center">

```
███████╗     ██╗██████╗ ████████╗
██╔════╝     ██║██╔══██╗╚══██╔══╝
█████╗       ██║██████╔╝   ██║   
██╔══╝  ██   ██║██╔═══╝    ██║   
███████╗╚█████╔╝██║        ██║   
╚══════╝ ╚════╝ ╚═╝        ╚═╝   
```

**`eLearnSecurity Junior Penetration Tester · Cheatsheets & Notas`**

[![Cert](https://img.shields.io/badge/Certificaci%C3%B3n-eJPTv2-ff6b35?style=flat-square&logo=elearnsecurity&logoColor=white)](https://security.ine.com/certifications/ejpt-certification/)
[![Plataforma](https://img.shields.io/badge/INE-Security-00bfff?style=flat-square&logo=ine&logoColor=white)](https://ine.com/)
[![Estado](https://img.shields.io/badge/Estado-Cheatsheet%20viva-00ff88?style=flat-square)](#)
[![Idioma](https://img.shields.io/badge/Idioma-Espa%C3%B1ol-9fef00?style=flat-square)](#)

</div>

---

## `$ whoami`

```bash
> Repo      :  eJPT — Cheatsheets personales
> Autor     :  Arabot
> Objetivo  :  Preparar y aprobar el eLearnSecurity Junior Penetration Tester (eJPTv2)
> Formato   :  Notas Obsidian → Markdown limpio para GitHub
> Idioma    :  Español 🇪🇸  (contenido 100% en castellano)
> Estado    :  [ Cheatsheet viva · Se actualiza conforme repaso ]
```

> Notas organizadas por tema con comandos listos para copiar, pensadas para:
> - **Repaso rápido** antes y durante la práctica de laboratorios.
> - **Material público** para cualquiera preparando el eJPT en español.
> - **Referencia personal** — el *por qué* de cada herramienta, no solo el *cómo*.

---

## `$ cat sobre_el_ejpt.txt`

El **eLearnSecurity Junior Penetration Tester (eJPTv2)** de INE Security es una certificación práctica de pentesting de nivel inicial. Examen 100% hands-on en un entorno de laboratorio real:

```
🎯  Modalidad   →  100% práctico (laboratorio real, no test)
⏱️  Duración    →  48 horas
🧰  Entorno     →  Kali Linux + máquinas Windows/Linux objetivo
📚  Temario    →  Pentesting básico, redes, web, Metasploit, post-explotación
🏆  Aprobado   →  ≥ 70 % de respuestas correctas
```

---

## `$ ls temas/`

> Cada tema tiene sus subapartados con comandos y técnicas explicadas.

### 🔍 Information Gathering

| Apartado | Contenido | Enlace |
|----------|-----------|:------:|
| Active  | Nmap (escaneo de hosts, puertos, versiones, evasión IDS) | [📄](eJPTv2/Information%20Gathering/Active/Nmap.md) |
| Passive | Reconocimiento Web (whois, dnsrecon, robots.txt, whatweb…) | [📄](eJPTv2/Information%20Gathering/Passive/Reconocimiento%20Web.md) |

### 🕸️ Web Application

| Apartado | Contenido | Enlace |
|----------|-----------|:------:|
| Gobuster | Fuzzing de directorios, archivos y subdominios | [📄](eJPTv2/Web%20Application/Gobuster.md) |
| WpScan   | Enumeración y vulnerabilidades en WordPress | [📄](eJPTv2/Web%20Application/WpScan.md) |

### 💣 Metasploit

| Apartado | Contenido | Enlace |
|----------|-----------|:------:|
| Sessions | Manejo de sesiones (background, shell_to_meterpreter…) | [📄](eJPTv2/Metasploit/Sessions.md) |
| Searchsploit | Búsqueda de exploits en Exploit-DB local | [📄](eJPTv2/Metasploit/Searchsploit.md) |
| Keylogging | Captura de teclas con Meterpreter | [📄](eJPTv2/Metasploit/Keylogging.md) |
| Msfvenom Payloads | Generación de payloads y handlers | [📄](eJPTv2/Metasploit/Payloads/Msfvenom%20Payloads.md) |
| Scanning · FTP | Enumeración / brute force FTP | [📄](eJPTv2/Metasploit/Scanning%20Metasploit/FTP.md) |
| Scanning · SSH | Enumeración / brute force SSH | [📄](eJPTv2/Metasploit/Scanning%20Metasploit/SSH.md) |
| Scanning · SMB | Versión, usuarios, shares, brute force | [📄](eJPTv2/Metasploit/Scanning%20Metasploit/SMB.md) |
| Scanning · SMTP | Versión y enumeración de usuarios | [📄](eJPTv2/Metasploit/Scanning%20Metasploit/SMTP.md) |
| Scanning · MySQL | Versión, brute force, schema dump | [📄](eJPTv2/Metasploit/Scanning%20Metasploit/MySQL.md) |
| Scanning · WEB | HTTP version, headers, directorios | [📄](eJPTv2/Metasploit/Scanning%20Metasploit/WEB.md) |
| Scanning · Ports | TCP/UDP port scan | [📄](eJPTv2/Metasploit/Scanning%20Metasploit/Ports.md) |

### 🐧 Linux

**Vulnerabilities**

| Servicio | Manual | Metasploit |
|----------|:------:|:----------:|
| Banner Grabbing | [📄](eJPTv2/Linux/Vulnerabilities/Banner%20Grabbing/Manual.md) | — |
| FTP             | [📄](eJPTv2/Linux/Vulnerabilities/FTP/Manual.md) | [📄](eJPTv2/Linux/Vulnerabilities/FTP/Metasploit.md) |
| SSH             | [📄](eJPTv2/Linux/Vulnerabilities/SSH/Manual.md) | [📄](eJPTv2/Linux/Vulnerabilities/SSH/Metasploit.md) |
| SMB             | [📄](eJPTv2/Linux/Vulnerabilities/SMB/Manual.md) | [📄](eJPTv2/Linux/Vulnerabilities/SMB/Metasploit.md) |
| SMTP            | — | [📄](eJPTv2/Linux/Vulnerabilities/SMTP/Metasploit.md) |
| PHP             | [📄](eJPTv2/Linux/Vulnerabilities/PHP/Manual.md) | — |
| Shellshock (CVE-2014-6271) | [📄](eJPTv2/Linux/Vulnerabilities/Shellshock%20-%20CVE%202014-6271/Manual.md) | [📄](eJPTv2/Linux/Vulnerabilities/Shellshock%20-%20CVE%202014-6271/Metasploit.md) |
| XODA            | — | [📄](eJPTv2/Linux/Vulnerabilities/Xoda/Metasploit.md) |

**Privilege Escalation** · [Sudo (GTFOBins)](eJPTv2/Linux/Privilege%20Escalation/Sudo.md) · [Cron Jobs](eJPTv2/Linux/Privilege%20Escalation/Cron%20Jobs.md)

**Post Exploitation** · [Shells](eJPTv2/Linux/Post%20Exploitation/Shells.md) · [Reverse Shells + TTY](eJPTv2/Linux/Post%20Exploitation/Reverse%20Shells.md) · [Credential Dumping](eJPTv2/Linux/Post%20Exploitation/Credential%20Dumping.md) · [Persistence](eJPTv2/Linux/Post%20Exploitation/Persistence.md) · [Clearing](eJPTv2/Linux/Post%20Exploitation/Clearing.md)

### 🪟 Windows

**Vulnerabilities**

| Servicio / CVE | Manual | Metasploit |
|----------------|:------:|:----------:|
| SMB            | — | [📄](eJPTv2/Windows/Vulnerabilities/SMB/Metasploit.md) |
| RDP            | — | [📄](eJPTv2/Windows/Vulnerabilities/RDP/Metasploit.md) |
| HTTP (Rejetto HFS) | — | [📄](eJPTv2/Windows/Vulnerabilities/HTTP/Metasploit.md) |
| WebDAV         | [📄](eJPTv2/Windows/Vulnerabilities/WebDAV/Manual.md) | [📄](eJPTv2/Windows/Vulnerabilities/WebDAV/Metasploit.md) |
| WinRM          | [📄](eJPTv2/Windows/Vulnerabilities/WinRM/Manual.md) | [📄](eJPTv2/Windows/Vulnerabilities/WinRM/Metasploit.md) |
| Tomcat 8.5.19  | — | [📄](eJPTv2/Windows/Vulnerabilities/Tomcat%208.5.19/Metasploit.md) |
| EternalBlue (MS17-010) | — | [📄](eJPTv2/Windows/Vulnerabilities/EternalBlue%20-%20MS17-010/Metasploit.md) |
| BlueKeep (CVE-2019-0708) | — | [📄](eJPTv2/Windows/Vulnerabilities/BlueKeep%20-%20CVE%202019-0708/Metasploit.md) |

**Credential Dumping** · [MimiKatz](eJPTv2/Windows/Credential%20Dumping/MimiKatz.md) · [Kiwi (Meterpreter)](eJPTv2/Windows/Credential%20Dumping/Kiwi.md) · [Pass The Hash](eJPTv2/Windows/Credential%20Dumping/Pass%20The%20Hash.md) · [Configuration Files](eJPTv2/Windows/Credential%20Dumping/Configuration%20Files.md)

**Privilege Escalation** · [UAC](eJPTv2/Windows/Privilege%20Escalation/UAC.md) · [Bypassing UAC](eJPTv2/Windows/Privilege%20Escalation/Bypassing%20UAC.md) · [Kernel Sploit](eJPTv2/Windows/Privilege%20Escalation/Kernel%20Sploit.md) · [Access Token Impersonation](eJPTv2/Windows/Privilege%20Escalation/Access%20Token%20Impersonation.md) · [PrivescCheck](eJPTv2/Windows/Privilege%20Escalation/PrivescCheck.md)

**Post Exploitation** · [Meterpreter Modules](eJPTv2/Windows/Post%20Exploitation/Modules.md) · [Persistence (MSF)](eJPTv2/Windows/Post%20Exploitation/Persistence/Metasploit.md) · [Persistence (RDP)](eJPTv2/Windows/Post%20Exploitation/Persistence/RDP.md) · [Clearing Event Logs](eJPTv2/Windows/Post%20Exploitation/Clearing%20Event%20Logs.md) · [Alternate Data Streams](eJPTv2/Windows/Alternate%20Data%20Streams.md)

### 🔧 Misceláneo

| Tema | Descripción | Enlace |
|------|-------------|:------:|
| Cracking | John the Ripper, Hashcat, modos `-a` y `-m` | [📄](eJPTv2/Cracking.md) |
| Transferring Files | Mover archivos atacante ↔ víctima (HTTP, certutil, wget, curl) | [📄](eJPTv2/Transferring%20Files%20Python.md) |
| Pivoting | Autoroute, port forwarding y movimiento lateral con MSF | [📄](eJPTv2/Pivoting.md) |

---

## `$ tree .`

```
EJPT/
├── README.md                                ← este índice
└── eJPTv2/
    ├── Cracking.md
    ├── Pivoting.md
    ├── Transferring Files Python.md
    ├── Information Gathering/
    │   ├── Active/Nmap.md
    │   └── Passive/Reconocimiento Web.md
    ├── Web Application/
    │   ├── Gobuster.md
    │   └── WpScan.md
    ├── Metasploit/
    │   ├── Keylogging.md
    │   ├── Searchsploit.md
    │   ├── Sessions.md
    │   ├── Payloads/Msfvenom Payloads.md
    │   └── Scanning Metasploit/ (FTP, SSH, SMB, SMTP, MySQL, WEB, Ports)
    ├── Linux/
    │   ├── Post Exploitation/
    │   ├── Privilege Escalation/
    │   └── Vulnerabilities/
    └── Windows/
        ├── Alternate Data Streams.md
        ├── Credential Dumping/
        ├── Post Exploitation/
        ├── Privilege Escalation/
        └── Vulnerabilities/
```

---

## `$ cat metodologia.txt`

Flujo típico de un examen / laboratorio eJPT:

```
1.  📡  Reconocimiento     →  Nmap (host discovery, puertos, versiones)
2.  🔬  Enumeración        →  por servicio (FTP, SMB, SSH, WEB...)
3.  💥  Explotación        →  manual + Metasploit (vulnerabilidades conocidas)
4.  🪜  Escalada           →  sudo / SUID / kernel (Linux) · UAC / tokens (Windows)
5.  🎒  Post-explotación   →  dump de credenciales, persistencia, limpieza
6.  🌐  Pivoting           →  autoroute + port forwarding para llegar a redes internas
```

---

## `$ cat aviso.txt`

> ⚠️ **Material de estudio personal.** Las técnicas descritas solo deben usarse contra los laboratorios oficiales de **INE Security / eJPT** o sistemas para los que se tenga autorización explícita por escrito. El uso contra sistemas de terceros sin permiso es **ilegal**.

---

## `$ cat contacto.txt`

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-Caan31-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Caan31)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Conectar-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/carlos-andres-aragon-nacimba)
[![HackTheBox](https://img.shields.io/badge/HackTheBox-Perfil-9fef00?style=for-the-badge&logo=hackthebox&logoColor=black)](https://profile.hackthebox.com/profile/019d926f-f2ef-7360-bbab-d3551b8aa9b5)

</div>

---

<div align="center">

```
[ Aprendiendo en público · Cheatsheet viva · Pensada para el examen ]
```

*Si te sirve para preparar tu eJPT, dale una ⭐ al repo — significa mucho.*

</div>
