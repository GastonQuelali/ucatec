---
title: "2. Medios de Transmisión y Equipos de Red"
layout: post
category: redes
permalink: /medios-transmision/
weight: 2
---

## 2.1. Medios de Transmisión

### Concepto
Los medios de transmisión son los canales físicos o inalámbricos a través de los cuales se envían señales y datos entre dispositivos en una red. Se dividen principalmente en dos categorías: medios guiados (cables) y no guiados (inalámbricos).

### Historia y Evolución
- **Cables de Cobre (Par Trenzado):** Uno de los primeros medios de transmisión utilizados, especialmente en redes telefónicas, evolucionó para soportar redes Ethernet.
- **Fibra Óptica:** Introducida en las telecomunicaciones en la década de 1970, revolucionó la transmisión de datos al permitir velocidades mucho más altas y largas distancias sin pérdida significativa de señal.
- **Medios Inalámbricos:** La tecnología inalámbrica comenzó con la radio en la primera mitad del siglo XX y ha evolucionado con estándares como Wi-Fi, Bluetooth y 5G.

### Tipos de Medios de Transmisión

#### 1. Par Trenzado
- **Definición:** Consiste en dos conductores de cobre aislados, trenzados entre sí para reducir interferencias electromagnéticas.
- **Características:** Disponible en categorías (Cat5e, Cat6, Cat6a) que determinan su velocidad y alcance.
- **Usos Prácticos:** Redes LAN, telefonía.
- **Evolución:** Los cables Cat6 y superiores soportan velocidades de hasta 10 Gbps, mientras que futuras categorías podrían mejorar aún más estas capacidades.

#### 2. Fibra Óptica
- **Definición:** Utiliza hilos de vidrio o plástico para transmitir datos mediante pulsos de luz.
- **Características:** Alta velocidad (hasta 100 Gbps), larga distancia (hasta 40 km sin repetidores), inmune a interferencias electromagnéticas.
- **Usos Prácticos:** Backbone de redes, conexiones de larga distancia, ISP.
- **Evolución:** La fibra óptica está en constante evolución con tecnologías como WDM (Multiplexación por División de Longitud de Onda) para aumentar la capacidad.

#### 3. Medios Inalámbricos
- **Definición:** Utilizan ondas de radio, microondas o infrarrojas para la transmisión de datos sin necesidad de cables físicos.
- **Características:** Varían según la tecnología; Wi-Fi (hasta 9.6 Gbps con Wi-Fi 6), Bluetooth (hasta 2 Mbps), 5G (hasta 10 Gbps).
- **Usos Prácticos:** Redes domésticas y corporativas, dispositivos móviles, IoT.
- **Evolución:** La tecnología inalámbrica sigue avanzando hacia mayores velocidades y menor latencia con la llegada de Wi-Fi 7 y 6G.

## 2.2. Equipos de Red

### Concepto
Los equipos de red son dispositivos que permiten la interconexión de los diferentes componentes de una red, facilitando la comunicación entre ellos. Esto incluye routers, switches, hubs, firewalls, y otros dispositivos especializados.

### Equipos Clave

#### 1. Router
- **Definición:** Un router dirige el tráfico de datos entre diferentes redes, conectando múltiples redes y gestionando el tráfico de paquetes entre ellas.
- **Historia:** Desarrollado en los años 1980 para interconectar diferentes tipos de redes.
- **Características:** NAT, soporte para múltiples interfaces, protocolos de enrutamiento.
- **Usos Prácticos:** Conectar redes domésticas o corporativas a Internet, interconectar oficinas remotas.
- **Evolución:** Con la virtualización y SDN, los routers están evolucionando hacia soluciones más centradas en software.

#### 2. Switch
- **Definición:** Un switch conecta dispositivos dentro de una red local, operando en la capa 2 (nivel de enlace) del modelo OSI, enviando los datos únicamente al dispositivo de destino.
- **Historia:** Reemplazaron a los hubs para mejorar la eficiencia de las redes Ethernet en la década de 1990.
- **Características:** VLAN, soporte para QoS, administración a través de SNMP.
- **Usos Prácticos:** Conectar computadoras, impresoras y otros dispositivos en una red local.
- **Evolución:** Integración con SDN y capacidades avanzadas como la priorización de tráfico multimedia.

#### 3. Access Point (Punto de Acceso)
- **Definición:** Un punto de acceso inalámbrico (AP) permite que los dispositivos inalámbricos se conecten a una red cableada mediante la transmisión y recepción de señales Wi-Fi.
- **Historia:** Los primeros AP surgieron con la popularización de Wi-Fi en la década de 1990.
- **Características:** Soporte para múltiples bandas (2.4 GHz, 5 GHz), seguridad (WPA3).
- **Usos Prácticos:** Extender la cobertura de una red Wi-Fi en entornos domésticos y corporativos.
- **Evolución:** APs con soporte para Wi-Fi 6 y tecnologías de gestión centralizada para redes corporativas grandes.

#### 4. Firewall
- **Definición:** Un firewall controla el tráfico de red entrante y saliente basado en reglas de seguridad, protegiendo la red contra accesos no autorizados.
- **Historia:** Surgieron en los años 1990, coincidiendo con el aumento del uso de Internet.
- **Características:** Inspección de paquetes, filtrado de contenido, prevención de intrusiones.
- **Usos Prácticos:** Protegen redes corporativas y domésticas, segmentan redes internas para mayor seguridad.
- **Evolución:** Integración con otras funciones de seguridad en dispositivos UTM y NGFW.

## 2.3. Instalación y Configuración de Cableado

### Concepto
La instalación y configuración de cableado implica la disposición física de los cables en una red, asegurando que la señal pueda transmitirse sin interferencias y cumpliendo con las normas de seguridad y eficiencia.

### Tipos de Cableado

#### 1. Cableado Estructurado
- **Definición:** Es un sistema de cableado diseñado para ser flexible, estandarizado y capaz de soportar múltiples tipos de tráfico y dispositivos.
- **Historia:** Desarrollado en los años 1980 para simplificar la instalación y el mantenimiento de redes.
- **Características:** Incluye cables de par trenzado, fibra óptica, paneles de parcheo y otros componentes.
- **Usos Prácticos:** Instalaciones en edificios comerciales, centros de datos.
- **Evolución:** Con la demanda de mayores velocidades y capacidades, el cableado estructurado evoluciona hacia el soporte de tecnologías avanzadas como 40GBASE-T y 100GBASE-T.

### Pasos de Instalación

1. **Planificación:**
   - **Evaluación de Requerimientos:** Determinar la cantidad de dispositivos, la distancia entre ellos, y el ancho de banda necesario.
   - **Elección de Materiales:** Selección de cables adecuados (Cat5e, Cat6, fibra óptica) y componentes (conectores, paneles de parcheo).

2. **Instalación Física:**
   - **Tendido de Cables:** Colocación de cables según el diseño, evitando interferencias eléctricas y respetando las normativas.
   - **Terminado:** Crimpado de conectores RJ45, fusión de fibras ópticas, conexión en paneles de parcheo.

3. **Configuración:**
   - **Pruebas de Conectividad:** Uso de herramientas como certificadores de cable para verificar la integridad de la instalación.
   - **Documentación:** Registrar la ubicación de cada cable y puerto, facilitando el mantenimiento futuro.

### Herramientas de Instalación
- **Crimpadora:** Para instalar conectores RJ45 en cables de par trenzado.
- **Certificadores de Cable:** Para verificar que el cableado cumple con las especificaciones técnicas y estándares.
- **Fusionadora de Fibra:** Utilizada para unir segmentos de fibra óptica con una pérdida mínima de señal.

### Futuro de la Instalación de Cableado
La automatización y los sistemas inteligentes de gestión de cableado están emergiendo como tendencias, facilitando la instalación y el mantenimiento. Además, el cableado estructurado tendrá que adaptarse a las crecientes demandas de ancho de banda, especialmente en entornos de data centers.