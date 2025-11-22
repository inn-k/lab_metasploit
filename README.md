# 🛡️ LAB: Simulación de ataque controlado | Detección con SIEM | Metasploit

![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-293137?style=for-the-badge&logo=gnu-bash&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Networking](https://img.shields.io/badge/Networking-008CFF?style=for-the-badge&logo=cisco&logoColor=white)
![Security](https://img.shields.io/badge/Blue_Team-101345?style=for-the-badge&logo=hackthebox&logoColor=white)
![Metasploit](https://img.shields.io/badge/Metasploit-182028?style=for-the-badge&logo=metasploit&logoColor=blue)
![Nmap](https://img.shields.io/badge/Nmap-e0f7ff?style=for-the-badge&logo=nmap&logoColor=white)
![Wazuh](https://img.shields.io/badge/Wazuh-3585f9?style=for-the-badge&logo=wazuh&logoColor=white)
![Suricata](https://img.shields.io/badge/Suricata-f45a1c?style=for-the-badge&logo=suricata&logoColor=white)

Laboratorio práctico orientado a **ciberseguridad defensiva**, que integra técnicas de pentesting controlado con análisis y detección mediante **Wazuh, Suricata y Linux**.  
El objetivo es demostrar cómo un entorno SOC puede identificar, registrar y analizar actividades maliciosas reales en un laboratorio seguro.

---

## 🌟 Descripción del Proyecto
Este proyecto reproduce un **ataque controlado con Metasploit** contra una máquina vulnerable dentro de un entorno totalmente aislado.  
Durante la simulación se generan eventos de seguridad que luego son **detectados, analizados y correlacionados en Wazuh (SIEM)**, complementado con Suricata para la inspección de tráfico de red.

El laboratorio permite observar el ciclo completo: **ataque → explotación → post-explotación → detección → análisis**.

---

## 🎯 Objetivos del Laboratorio
• Simular un ataque controlado utilizando **Metasploit**.  
• Explotar vulnerabilidades conocidas en máquinas intencionalmente vulnerables.  
• Detectar actividades maliciosas mediante **Wazuh y Suricata**.  
• Evaluar reglas de detección, alertas y comportamiento del SIEM.  
• Documentar el proceso completo para reforzar habilidades de análisis defensivo.

---

## 📁 Arquitectura del Entorno
Laboratorio montado sobre **VirtualBox** en red aislada para evitar cualquier tipo de riesgo.

Red: \
• Tipo de red: **Host-Only / NAT combinado**  
• Segmento: **10.0.2.0/24**  
• Sin acceso a Internet (entorno cerrado)

Máquinas Virtuales: 
| Rol | Sistema | IP | Herramientas |
|-----|---------|----|--------------|
| **Atacante** | Kali Linux | 10.0.2.10 | Metasploit, Nmap, Netcat, Wireshark/Tshark |
| **Objetivo** | Metasploitable2 | 10.0.2.30 | VSFTPD vulnerable, Samba, servicios inseguros |
| **SIEM/Monitoreo** | Wazuh Server | 10.0.2.20 | Wazuh + agentes, Suricata como IDS |

---

## 🧠 Metodología
Fase 1 – Preparación del Entorno \
• Configuración de red aislada  
• Instalación de máquinas virtuales  
• Implementación de Wazuh + Suricata  

Fase 2 – Reconocimiento \
• Escaneo de red con **Nmap**  
• Enumeración de servicios  
• Identificación de vulnerabilidades  

Fase 3 – Explotación \
• Uso de **Metasploit**  
• Ejecución de exploits válidos  
• Obtención de sesión en el sistema objetivo  

Fase 4 – Post-Explotación \
• Enumeración del host comprometido  
• Escalada de privilegios  
• Intento de persistencia  

Fase 5 – Detección y Análisis \
• Revisión de alertas y logs en **Wazuh**  
• Análisis de tráfico con Suricata  
• Correlación de eventos y validación de reglas  

---

## 📬 Contacto

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/ingrid-k)  
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ingridkaufmannok@gmail.com)
