# NGIDS

**[ES]** Este proyecto está diseñado para monitorea el tráfico de red en tiempo real, detecta actividades maliciosas y permite crear reglas personalizadas. Registra métricas detalladas para análisis, ofreciendo flexibilidad y eficiencia en la protección de redes sin depender de herramientas comerciales

**[EN]** This project is designed to monitor network traffic in real-time, detect malicious activities, and allow the creation of custom rules. It logs detailed metrics for analysis, offering flexibility and efficiency in protecting networks without relying on commercial tools.
This project is designed to [Brief description of the tool or project's purpose].

**Autor / Author:** Jorge Luis Sánchez Casanova

**Licencia / License:** MIT License  

**Repositorio / Repository:** https://github.com/jorgelsc-dev/ngids.git


## Descripción / Description

# **[ES]**

# Descripción del Proyecto: Sniffer de Red en Python con Almacenamiento en Base de Datos

Este proyecto es un **sniffer de red avanzado desarrollado en Python** diseñado para capturar, analizar y almacenar paquetes de red en tiempo real. Su arquitectura combina el uso de **sockets**, **SQLite3** y **threading**, proporcionando una solución eficiente y extensible para el monitoreo y análisis de tráfico de red.

## Funcionamiento General

1. **Captura de Paquetes**  
   Utiliza sockets en modo RAW para interceptar paquetes directamente desde la interfaz de red. Esto permite capturar tanto cabeceras como datos de paquetes, incluyendo protocolos como TCP, UDP, ICMP y otros.

2. **Desempaquetado de Datos**  
   Cada paquete capturado es analizado para extraer información clave, como direcciones IP, puertos, protocolos y contenido útil. Este análisis se realiza en tiempo real para asegurar la disponibilidad inmediata de los datos.

3. **Almacenamiento en Base de Datos**  
   Los datos de los paquetes se almacenan en una base de datos SQLite3. Esto permite mantener un historial detallado de todo el tráfico capturado, facilitando su consulta y análisis posterior.

4. **Procesamiento Concurrente**  
   Implementa **threading** para gestionar de manera eficiente la captura y almacenamiento de datos. Los hilos permiten manejar múltiples paquetes simultáneamente, maximizando el rendimiento incluso en redes de alto tráfico.

## Características Clave

- **Captura en tiempo real**: Intercepta y analiza paquetes a medida que atraviesan la red.  
- **Desempaquetado avanzado**: Extrae información detallada de los paquetes para un análisis completo.  
- **Persistencia de datos**: Almacena los paquetes en SQLite3, garantizando un historial estructurado y accesible.  
- **Multitarea optimizada**: Utiliza threading para procesar datos concurrentemente, mejorando el rendimiento en redes saturadas.  
- **Compatibilidad multiplataforma**: Funciona en sistemas basados en Linux y otros compatibles con sockets RAW.

## Aplicaciones Potenciales

- **Monitoreo de seguridad**: Detecta patrones anómalos o tráfico sospechoso en la red.  
- **Análisis forense**: Proporciona un historial detallado del tráfico para investigaciones post-incidente.  
- **Estudio de protocolos**: Permite analizar el comportamiento y estructura de diferentes protocolos de red.  
- **Desarrollo de herramientas de red**: Puede utilizarse como base para desarrollar sistemas IDS, herramientas de análisis de red o soluciones personalizadas.

## Tecnologías y Bibliotecas Utilizadas

- **Python**: Lenguaje principal para la implementación del sniffer.  
- **Socket**: Para capturar paquetes a nivel de red.  
- **SQLite3**: Para almacenar datos de manera estructurada y persistente.  
- **Threading**: Para el manejo concurrente de la captura y procesamiento de paquetes.

## Ventajas del Proyecto

- **Simplicidad y eficiencia**: Diseñado para ser ligero y fácil de adaptar.  
- **Flexibilidad**: La combinación de Python y SQLite3 permite modificar y extender las funcionalidades según las necesidades del usuario.  
- **Educativo**: Ideal para aprender conceptos de redes, manejo de bases de datos y programación concurrente.

Este sniffer es una herramienta poderosa para administradores de red, investigadores de ciberseguridad y desarrolladores que buscan entender y analizar el tráfico de red en detalle. Su diseño modular y extensible permite personalizarlo para satisfacer diferentes requisitos, desde el monitoreo básico hasta el análisis avanzado.

# **[EN]**

# Project Description: Python Network Sniffer with Database Storage

This project is an **advanced network sniffer developed in Python**, designed to capture, analyze, and store network packets in real-time. Its architecture integrates **sockets**, **SQLite3**, and **threading**, offering an efficient and extensible solution for network traffic monitoring and analysis.

## General Functionality

1. **Packet Capture**  
   The sniffer uses RAW sockets to intercept packets directly from the network interface. This allows capturing both headers and payloads, supporting protocols like TCP, UDP, ICMP, and others.

2. **Packet Unpacking**  
   Each captured packet is analyzed to extract critical information, such as IP addresses, ports, protocols, and other relevant content. This analysis is performed in real-time to ensure immediate data availability.

3. **Database Storage**  
   Packet data is stored in an SQLite3 database, enabling a detailed record of all captured traffic for easy querying and further analysis.

4. **Concurrent Processing**  
   The project leverages **threading** to efficiently manage data capture and storage. Threads handle multiple packets simultaneously, ensuring high performance even in networks with heavy traffic.

## Key Features

- **Real-Time Capture**: Intercepts and analyzes packets as they traverse the network.  
- **Advanced Unpacking**: Extracts detailed information from packets for comprehensive analysis.  
- **Data Persistence**: Stores packets in SQLite3 for structured and accessible historical data.  
- **Optimized Multitasking**: Uses threading to process data concurrently, enhancing performance in high-traffic environments.  
- **Cross-Platform Compatibility**: Operates on Linux-based systems and other platforms supporting RAW sockets.

## Potential Applications

- **Security Monitoring**: Detects anomalous patterns or suspicious traffic in the network.  
- **Forensic Analysis**: Provides a detailed traffic history for post-incident investigations.  
- **Protocol Studies**: Allows analysis of the behavior and structure of different network protocols.  
- **Network Tool Development**: Serves as a foundation for building IDS systems, network analysis tools, or custom solutions.

## Technologies and Libraries Used

- **Python**: The primary language for implementing the sniffer.  
- **Socket**: For capturing packets at the network layer.  
- **SQLite3**: For storing data in a structured and persistent manner.  
- **Threading**: For concurrent handling of packet capture and processing.

## Project Advantages

- **Simplicity and Efficiency**: Designed to be lightweight and easy to adapt.  
- **Flexibility**: The combination of Python and SQLite3 allows for extending and customizing functionalities based on user needs.  
- **Educational Value**: Ideal for learning about networking, database management, and concurrent programming.

This sniffer is a powerful tool for network administrators, cybersecurity researchers, and developers seeking to understand and analyze network traffic in detail. Its modular and extensible design makes it adaptable to various use cases, from basic monitoring to advanced analysis.


## Instalación / Installation

Para instalar y ejecutar este proyecto, sigue los siguientes pasos:  
To install and run this project, follow these steps:

1. **Clonar el repositorio / Clone the repository**:

   ```bash
   git clone https://github.com/jorgelsc-dev/ngids.git
   ```
