<h1 align="center">Reporte Técnico de Pentesting – HTB Conversor</h1>

<p align="center">
  <img src="./Evidencia/conversor_pwned.png" alt="HTB Conversor Pwned" width="650">
</p>

Este repositorio contiene un reporte técnico completo de pruebas de penetración
realizadas sobre la máquina **Conversor** de la plataforma **Hack The Box**.

## Contenido
- Reconocimiento y enumeración  
- Análisis de la aplicación web  
- Revisión de código fuente (white-box)  
- Explotación (RCE vía Path Traversal + Cron)  
- Post-explotación (extracción de credenciales en SQLite)  
- Crackeo de hash (MD5)  
- Movimiento lateral (SSH)  
- Escalamiento de privilegios (sudo / needrestart)  
- Captura de flags (user / root)  

## Técnicas utilizadas
- Network reconnaissance (ICMP, Nmap)  
- Web enumeration (Gobuster)  
- Source code review (exposición en /about)  
- File upload abuse (Path Traversal / arbitrary file write)  
- RCE chaining (cron job execution)  
- Credential extraction (SQLite)  
- Password cracking (John the Ripper + rockyou.txt, MD5)  
- Remote access (SSH)  
- Privilege escalation (sudo misconfiguration: needrestart config injection)  

## Reporte
**[Reporte completo en PDF](Reporte_HTB_Conversor.pdf)**

## Exploits
El exploit desarrollado y utilizado durante la fase de explotación se encuentra
disponible en el siguiente archivo:

 **[exploit.py](./Exploits/exploit.py)**
 **[doc.xslt](./Exploits/doc.xslt)**

## Aviso
Este contenido tiene fines **educativos** y fue desarrollado en un entorno
controlado (Hack The Box). No debe utilizarse contra sistemas sin autorización.

## Autor
**KeruDWL**  
2025
