---
title: "4. Seguirdad en Redes"
author: Gaston Quelali
date: 2024-08-01
category: redes
layout: post
permalink: /redes/seguridad-redes/
weight: 4
---

La seguridad en redes es una disciplina esencial en el campo de las telecomunicaciones y la informática, que se centra en proteger la integridad, confidencialidad y disponibilidad de la información transmitida a través de redes de comunicación. A medida que las amenazas cibernéticas se han vuelto más sofisticadas, la necesidad de implementar medidas de seguridad robustas en las redes es más crítica que nunca.

### 4.1. Fundamentos de Seguridad en Redes

#### Conceptos Básicos
- **Confidencialidad:** Garantizar que la información solo sea accesible para quienes tienen la autorización adecuada.
- **Integridad:** Asegurar que los datos no sean alterados o manipulados de manera no autorizada durante su transmisión o almacenamiento.
- **Disponibilidad:** Asegurar que los servicios y recursos de red estén disponibles para los usuarios autorizados cuando los necesiten.
- **Autenticación:** Verificar la identidad de los usuarios y dispositivos que intentan acceder a la red.
- **Autorización:** Definir los permisos y accesos que tiene un usuario o dispositivo una vez autenticado.
- **No repudio:** Garantizar que una vez que una acción ha sido realizada en la red, el usuario o dispositivo que la realizó no pueda negar haberla hecho.

#### Amenazas Comunes en Redes
- **Ataques de Intercepción:** Como la escucha clandestina (eavesdropping) y el sniffing, donde un atacante intercepta las comunicaciones entre dos partes.
- **Ataques de Interrupción:** Denegación de servicio (DoS) y ataques distribuidos de denegación de servicio (DDoS), donde un atacante busca hacer que los servicios de red sean inaccesibles.
- **Ataques de Modificación:** Manipulación de datos en tránsito, como el ataque de hombre en el medio (MITM).
- **Ataques de Falsificación:** Suplantación de identidad (spoofing) donde el atacante se hace pasar por otro usuario o dispositivo en la red.

#### Principios de Defensa en Profundidad
- **Capa Física:** Protecciones físicas como cerraduras, control de acceso a hardware, y videovigilancia.
- **Capa de Red:** Implementación de firewalls, routers seguros, y segmentación de redes.
- **Capa de Transporte:** Uso de protocolos seguros como SSL/TLS.
- **Capa de Aplicación:** Configuración de políticas de seguridad en aplicaciones, uso de cifrado y autenticación fuerte.
- **Capa de Datos:** Uso de cifrado de datos en reposo y en tránsito, junto con políticas de respaldo.

### 4.2. Protocolos de Seguridad

#### Protocolo de Seguridad de la Capa de Red (IPSec)
- **Autenticación de Encabezado (AH):** Proporciona autenticación e integridad para los paquetes de datos.
- **Carga de Seguridad Encapsulada (ESP):** Proporciona cifrado, autenticación e integridad.
- **Modos de IPSec:** Modo Transporte (protege solo la carga útil de los paquetes IP) y Modo Túnel (protege todo el paquete IP).

#### Seguridad en la Capa de Transporte (SSL/TLS)
- **SSL (Secure Sockets Layer):** Protocolo precursor de TLS, utilizado para asegurar las comunicaciones a través de Internet.
- **TLS (Transport Layer Security):** Protocolo que proporciona confidencialidad e integridad de los datos entre aplicaciones que se comunican a través de una red.
- **Handshake TLS:** Proceso que negocia los algoritmos criptográficos y establece las claves de sesión.

#### Protocolo SSH (Secure Shell)
- **Autenticación:** SSH permite la autenticación segura a través de contraseñas, claves públicas o autenticación basada en certificados.
- **Túneles SSH:** Crea un túnel seguro para proteger otras comunicaciones de red.

#### Protocolos de Seguridad para Correo Electrónico
- **SMTP sobre TLS:** Asegura la transmisión de correos electrónicos.
- **S/MIME:** Proporciona cifrado y firma digital para correos electrónicos.
- **PGP (Pretty Good Privacy):** Utilizado para cifrar y firmar correos electrónicos.

#### Protocolo WPA3 para Redes Inalámbricas
- **Cifrado más fuerte:** Utiliza SAE (Simultaneous Authentication of Equals) para proteger contra ataques de fuerza bruta.
- **Modo de Equivalencia para Redes Abiertas:** Proporciona cifrado incluso en redes Wi-Fi abiertas.

### 4.3. Seguridad en Redes Inalámbricas

#### Vulnerabilidades Comunes en Redes Inalámbricas
- **Intercepción de Señal:** Las señales inalámbricas pueden ser interceptadas fácilmente debido a su naturaleza omnidireccional.
- **Ataques de AP Falso (Rogue Access Point):** Un atacante establece un punto de acceso no autorizado para interceptar el tráfico de la red.
- **Ataques de Desautenticación:** Interrupción de la conexión entre un cliente y un punto de acceso inalámbrico.

#### Protocolos de Seguridad Inalámbrica
- **WEP (Wired Equivalent Privacy):** Protocolo de seguridad antiguo y débil, fácil de romper.
- **WPA (Wi-Fi Protected Access):** Mejora de WEP, pero con vulnerabilidades conocidas.
- **WPA2:** Protocolo más robusto basado en el estándar IEEE 802.11i, utiliza AES para el cifrado.
- **WPA3:** Última generación de seguridad inalámbrica, mejora la protección contra ataques de fuerza bruta y proporciona cifrado individualizado.

#### Buenas Prácticas de Seguridad en Redes Inalámbricas
- **Cambiar Contraseñas Predeterminadas:** Es crucial cambiar las contraseñas predeterminadas de los puntos de acceso.
- **Desactivar WPS (Wi-Fi Protected Setup):** WPS es vulnerable a ataques de fuerza bruta, por lo que es recomendable desactivarlo.
- **Ocultar el SSID:** Aunque no es una medida de seguridad fuerte, ocultar el SSID puede disuadir a algunos atacantes.
- **Implementar un Firewall:** Uso de firewalls en la red local para controlar el tráfico entrante y saliente.

#### Segmentación de Redes Inalámbricas
- **Redes Invitadas:** Separar la red de invitados de la red principal para evitar que los usuarios no autorizados accedan a recursos críticos.
- **Uso de VLANs:** Segmentar la red mediante VLANs para minimizar el acceso no autorizado y mejorar la gestión del tráfico.
