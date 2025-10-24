# Tarea 4: 
---
### **Integrantes:**  
- Camila Perez Mercado
- Santiago Hernandes Avila
- Diego Alejandro Rodríguez Guzmán  
### Facultad de Ingeniería Electrónica  - Comunicaciones Industriales 
### Universidad Santo Tomas  
---
## 1) Vigilancia Tecnológica de Tecnologías Industriales

En la actualidad, la automatización industrial depende de una gran variedad de protocolos de comunicación que permiten la interconexión entre controladores, sensores, actuadores y sistemas de supervisión. Entre los más relevantes se encuentran **Modbus**, **AS-Interface (AS-I)** y las **categorías más recientes del Ethernet Industrial**.

### a)**Modbus**
-**Descripción:** Protocolo industrial abierto creado por Modicon (ahora Schneider Electric) para la comunicación maestro-esclavo entre dispositivos electrónicos.
- **Tipo:** Protocolo maestro-esclavo.  
- **Medio físico:** RS-232, RS-485 o Ethernet (Modbus TCP).  
- **Fabricante:** Schneider Electric (origen).  
- **Uso principal:** Intercambio de datos entre PLC, sensores, variadores y SCADA.  
- **Ventajas:**
  - Abierto y ampliamente soportado.
  - Simple de implementar.
  - Compatible entre múltiples fabricantes.  
- **Aplicaciones:** Control de motores, monitoreo de energía, instrumentación industrial.

---

### B) **AS-Interface (AS-I)**
- **Descripción:** Protocolo diseñado para conectar sensores y actuadores a un controlador principal mediante un cable plano de dos hilos.
- **Tipo:** Protocolo maestro-esclavo de bajo nivel.  
- **Medio físico:** Cable plano amarillo AS-I (alimentación y comunicación simultánea).  
- **Uso principal:** Comunicación directa entre sensores y actuadores simples.  
- **Ventajas:**
  - Instalación sencilla y económica.  
  - Permite reducir cableado.  
  - Compatible con sistemas superiores (vía gateways a PROFIBUS o PROFINET).  
- **Aplicaciones:** Sistemas de control de procesos discretos, automatización de fábricas, control de seguridad.  

---

### C) **Categorías Nuevas del Ethernet Industrial**
El **Ethernet Industrial** es la base de comunicación moderna en la automatización. Integra distintas versiones y categorías mejoradas para la industria 4.0.

| **Versión** | **Velocidad** | **Aplicación** | **Protocolos asociados** |
|--------------|----------------|----------------|----------------------------|
| **Ethernet/IP** | 100 Mbps | PLC – HMI – Variadores | Rockwell, Siemens |
| **PROFINET** | 100 Mbps / 1 Gbps | Siemens, automatización de planta | PROFINET RT/IRT |
| **EtherCAT** | 100 Mbps | Control en tiempo real | Beckhoff |
| **Power over Ethernet (PoE)** | — | Transmisión de datos y energía por el mismo cable | Cámaras IP, sensores |
| **Time-Sensitive Networking (TSN)** | 1 Gbps | Comunicación determinista en tiempo real | Industria 4.0, IoT |

Estas nuevas categorías mejoran la **velocidad, sincronización y confiabilidad**, permitiendo la integración entre sistemas industriales, IoT y nube.

---

## 2️) Exploración de Dispositivos Encontrados en la Universidad

A continuación, se detallan los dispositivos observados en el laboratorio, cada uno con su descripción, protocolo de comunicación y características principales.

### **2.1) UP² Board (placa pequeña)**
📸 **Imagen del dispositivo:** 
![Analizador de energía](WhatsApp_Image_2025-10-23_at_21.57.29_2f705b10.jpg) 

**Protocolos de comunicación:** 
- Ethernet
- RS-485 
- USB
- GPIO
- Modbus 
- TCP/IP (software).
 
**Características principales:**
Puede actuar como gateway o servidor IoT conectando PLCs y sensores industriales.

---

### ⚙️ **2.2) Analizador de Redes Eléctricas**

📸 **Imagen del dispositivo:**  
![Analizador de energía](./coloca_aqui_imagen4.jpg)

**Protocolos de comunicación:**  
- Modbus RTU (RS-485)  
- Ethernet
- TCP/IP (según modelo)  

**Características principales:**  
- Permite medir tensión, corriente, potencia y factor de potencia.  
- Registra armónicos y calidad de la energía.  
- Comunicación con SCADA o PLC mediante Modbus.  
- Pantalla LCD para visualización directa de parámetros.  

---

### ⚙️ **2.3) Analizador de Calidad Energética**

📸 **Imagen del dispositivo:**  
*(Colocar aquí la imagen frontal del analizador de calidad energética)*  
![Analizador de energía](./coloca_aqui_imagen4.jpg)
**Protocolos de comunicación:**  
- RS-485 (Modbus RTU)  
- Ethernet (opcional según versión)  

**Características principales:**  
- Evalúa la calidad del suministro eléctrico.  
- Registra eventos, armónicos y distorsiones.  
- Permite almacenamiento de datos históricos.  
- Interfaz de comunicación con software de análisis.  

---

### ⚙️ **2.4) SIMATIC HMI y PLC Siemens (S7-1200)**

📸 **Imagen del dispositivo:**  
![Analizador de energía](./coloca_aqui_imagen4.jpg)

**Protocolos de comunicación:**  
- Profinet 
- Profibus 
- Ethernet/IP 
- Modbus 
- TCP/IP 
(Cualquiera de estos mediante módulos) 

**Características principales:**  
Controla y monitorea procesos industriales, comunica datos con sensores, actuadores y analizadores.
- Interfaz gráfica para monitorear procesos y enviar comandos.  
- Pantalla táctil con alarmas y botones virtuales.  
- Configurable desde TIA Portal.
  
---
### **2.5)Router Linksys Cisco**

📸 **Imagen del dispositivo:**  
![Analizador de energía](./coloca_aqui_imagen4.jpg)

**Protocolos de comunicación:**  
- Ethernet
- Wi-Fi
- IPv4 / IPv6

**Características principales:**  
- Interfaz gráfica para monitorear procesos y enviar comandos.  
- Pantalla táctil con alarmas y botones virtuales.  
- Configurable desde TIA Portal.

---

##  3) IPv4 e IPv6: Concepto, Características y Diferencias

### 🔹 **IPv4 (Internet Protocol Version 4)**
- Longitud: 32 bits.  
- Formato: Decimal con puntos (ejemplo: 192.168.0.1).  
- Espacio de direcciones: ~4.3 mil millones.  
- Soporta: Unicast, broadcast y multicast.  
- Protocolos típicos: TCP, UDP, ICMP.  

### 🔹 **IPv6 (Internet Protocol Version 6)**
- Longitud: 128 bits.  
- Formato: Hexadecimal con dos puntos (ejemplo: 2001:0db8::1).  
- Espacio de direcciones: prácticamente ilimitado.  
- Soporta: Autoconfiguración y seguridad integrada (IPsec).  
- Elimina broadcast, usa multicast y anycast.  

### 🔹 **Diferencias principales:**

| Característica | IPv4 | IPv6 |
|----------------|------|------|
| Longitud | 32 bits | 128 bits |
| Formato | Decimal | Hexadecimal |
| Direcciones posibles | 4.3 mil millones | 3.4×10³⁸ |
| Configuración | Manual o DHCP | Automática (SLAAC) |
| Seguridad | Opcional | Integrada |
| Encabezado | Simple | Más optimizado |

---



