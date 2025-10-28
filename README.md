# Simulación de Ataque Controlado con Metasploit y Detección en SIEM

![Kali Linux](https://img.shields.io/badge/Kali_Linux-557C94?style=for-the-badge&logo=kali-linux&logoColor=white)
![Metasploit](https://img.shields.io/badge/Metasploit-2.7.8-FF0000?style=for-the-badge&logo=metasploit&logoColor=white)
![Wazuh](https://img.shields.io/badge/Wazuh-SIEM-00BFFF?style=for-the-badge&logo=wazuh&logoColor=white)
![VirtualBox](https://img.shields.io/badge/VirtualBox-183A61?style=for-the-badge&logo=virtualbox&logoColor=white)
![Nmap](https://img.shields.io/badge/Nmap-Network_Scanner-FF6600?style=for-the-badge&logo=nmap&logoColor=white)

## 📋 Descripción del Proyecto

Este proyecto consiste en una simulación de ciberataque controlado en un entorno aislado, con el objetivo de demostrar la explotación de vulnerabilidades en sistemas vulnerables y la capacidad de detección mediante un SIEM (Security Information and Event Management). El ejercicio simula un ataque real utilizando Metasploit contra una máquina virtual vulnerable y monitorea las actividades con Wazuh, Suricata y otras herramientas de observabilidad.

![Status](https://img.shields.io/badge/Status-Completado-success)
![Versión](https://img.shields.io/badge/Versión-1.0-blue)
![Licencia](https://img.shields.io/badge/Licencia-MIT-green)

## 🎯 Objetivos

![Objetivo 1](https://img.shields.io/badge/Objetivo-Simulación_ataque_Metasploit-important)
![Objetivo 2](https://img.shields.io/badge/Objetivo-Detección_SIEM-informational)
![Objetivo 3](https://img.shields.io/badge/Objetivo-Análisis_forense-success)

- Simular un ataque controlado utilizando el framework Metasploit
- Explotar vulnerabilidades conocidas en sistemas intencionalmente vulnerables
- Demostrar la detección de actividades maliciosas en logs y SIEM
- Evaluar la efectividad de las reglas de detección y la capacidad de respuesta
- Documentar el proceso de ataque y defensa para mejorar las posturas de seguridad

## 🏗️ Entorno de Laboratorio

### Arquitectura

![Red](https://img.shields.io/badge/Red-Aislada_Host--only-yellow)
![Seguridad](https://img.shields.io/badge/Seguridad-Sin_acceso_Internet-critical)

- **Red Aislada**: Configuración Host-only/NAT en VirtualBox
- **Segmento de Red**: 10.0.2.0/24
- **Sin Conectividad a Internet**: Prevención de riesgos de seguridad

### Máquinas Virtuales

![Kali](https://img.shields.io/badge/Kali_Linux-Atacante-557C94)
![Metasploitable](https://img.shields.io/badge/Metasploitable2-Objetivo-FF0000)
![Wazuh](https://img.shields.io/badge/Wazuh-SIEM-00BFFF)

- **Kali Linux (Atacante)**: IP 10.0.2.10
  - Metasploit Framework
  - Nmap, Netcat, Wireshark/Tshark
- **Metasploitable2 (Objetivo)**: IP 10.0.2.30
  - Servicios vulnerables: VSFTPD, Samba
  - Configuraciones intencionalmente inseguras
- **Wazuh (SIEM/Monitoreo)**: IP 10.0.2.20
  - Wazuh Server 
  - Agentes desplegados en todas las máquinas
  - Suricata para detección de intrusos en red

## 📊 Metodología

### Fase 1: Preparación del Entorno
![Fase 1](https://img.shields.io/badge/Fase-1_Preparación-blueviolet)
- Configuración de red aislada en VirtualBox
- Implementación de máquinas virtuales
- Configuración de herramientas de monitoreo

### Fase 2: Reconocimiento
![Fase 2](https://img.shields.io/badge/Fase-2_Reconocimiento-orange)
- Escaneo de red con Nmap
- Enumeración de servicios y versiones
- Identificación de vulnerabilidades

### Fase 3: Explotación
![Fase 3](https://img.shields.io/badge/Fase-3_Explotación-red)
- Uso de Metasploit para explotación de vulnerabilidades
- Ejecución de exploits contra servicios identificados
- Obtención de acceso al sistema objetivo

### Fase 4: Post-Explotación
![Fase 4](https://img.shields.io/badge/Fase-4_Post--Explotación-lightgrey)
- Enumeración del sistema comprometido
- Escalada de privilegios
- Establecimiento de persistencia

### Fase 5: Detección y Análisis
![Fase 5](https://img.shields.io/badge/Fase-5_Detección-green)
- Monitoreo de logs y alertas en Wazuh
- Análisis de tráfico de red con Suricata
- Correlación de eventos de seguridad

## 🛠️ Herramientas Utilizadas

![Metasploit](https://img.shields.io/badge/Metasploit-Explotación-FF0000)
![Nmap](https://img.shields.io/badge/Nmap-Escaneo-FF6600)
![Wazuh](https://img.shields.io/badge/Wazuh-SIEM-00BFFF)
![Suricata](https://img.shields.io/badge/Suricata-IDS-yellow)
![VirtualBox](https://img.shields.io/badge/VirtualBox-Virtualización-183A61)
![Kali Linux](https://img.shields.io/badge/Kali_Linux-Penetration_Testing-557C94)

## 👩‍💻 Autora

**Ingrid K.**  

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/ingrid-k)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ingridkaufmannok@gmail.com)
