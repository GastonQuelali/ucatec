---
title: "Redes 2"
author: Gaston Quelali
date: 2024-09-01
layout: post
collection: redes2
permalink: /redes2/unidad1/
weight: 1
---

## Unidad 1. Dispositivos comunes de red

El diseño y operación de redes requieren la implementación de varios dispositivos especializados, cada uno con funciones específicas para asegurar la conectividad, gestión del tráfico y seguridad de los datos. A continuación, se describen los dispositivos más comunes:

### 1. NIC (Network Interface Card)

La **Tarjeta de Red** o **NIC (Network Interface Card)** es un dispositivo de hardware que permite a un equipo conectarse a una red. Actúa como interfaz entre el dispositivo y la red, traduciendo las señales del equipo en formato adecuado para ser transmitido en la red y viceversa. Las NIC pueden ser alámbricas o inalámbricas.

- **Función principal**: Facilitar la conexión física y lógica de un dispositivo a la red.
- **Uso**: En todos los dispositivos que necesitan acceso a una red, como computadoras, servidores y dispositivos IoT.

### 2. Hub

El **Hub** es un dispositivo simple que opera en la capa física (capa 1 del modelo OSI). Su función es conectar múltiples dispositivos en una red y transmitir los datos recibidos a todos los puertos conectados, sin discriminación. Debido a esta falta de inteligencia en la transmisión, su uso ha disminuido en favor de dispositivos más eficientes como los switches.

- **Función principal**: Conectar dispositivos en una red local, enviando el mismo mensaje a todos los puertos.
- **Uso**: Redes pequeñas o entornos donde la eficiencia y la seguridad no son una prioridad.

### 3. Switch

El **Switch** es un dispositivo más avanzado que el hub, ya que opera en la capa de enlace de datos (capa 2 del modelo OSI). Los switches filtran y dirigen los datos utilizando las direcciones MAC, asegurando que los paquetes se envíen solo al dispositivo destino, mejorando la eficiencia y el rendimiento de la red.

- **Función principal**: Conectar dispositivos en una red local, enviando datos solo al destino específico.
- **Uso**: Oficinas, empresas y redes domésticas con múltiples dispositivos.

### 4. Bridge

El **Bridge** es un dispositivo que conecta dos segmentos de red separados, operando en la capa de enlace de datos (capa 2 del modelo OSI). Su función es filtrar y reenviar el tráfico de red entre los segmentos según las direcciones MAC, ayudando a reducir la congestión en la red.

- **Función principal**: Dividir una red en segmentos y controlar el tráfico entre ellos para reducir la congestión.
- **Uso**: Redes que necesitan dividirse en subredes para mejorar el rendimiento.

### 5. Router

El **Router** es un dispositivo que opera en la capa de red (capa 3 del modelo OSI) y se encarga de enrutar paquetes de datos entre redes diferentes. Utiliza direcciones IP y tablas de enrutamiento para determinar el camino más eficiente para que los datos lleguen a su destino. Además, los routers pueden implementar funcionalidades como NAT (Network Address Translation) y servir como firewall.

- **Función principal**: Enrutar datos entre redes diferentes.
- **Uso**: Hogares, empresas y redes de ISP que conectan varias redes o subredes.

### 6. Gateway

Un **Gateway** es un dispositivo que traduce entre diferentes tipos de redes que pueden usar diferentes protocolos. Los gateways operan en múltiples capas del modelo OSI, pero frecuentemente se asocian con la capa de aplicación (capa 7). Son esenciales para conectar redes que no podrían comunicarse directamente debido a diferencias en el protocolo de comunicación.

- **Función principal**: Traducir y permitir la comunicación entre redes con protocolos diferentes.
- **Uso**: Empresas que integran redes con diferentes tecnologías, como una LAN con la red de telefonía pública o una red con sistemas heredados.

### 7. Access Point (Punto de Acceso Inalámbrico)

El **Access Point (AP)** permite la conexión inalámbrica de dispositivos a una red local. Este dispositivo actúa como un puente entre la red cableada y los dispositivos móviles, extendiendo la cobertura de la red y permitiendo la conectividad en áreas más amplias.

- **Función principal**: Proveer acceso inalámbrico a la red local.
- **Uso**: Oficinas, campus universitarios, redes domésticas y entornos empresariales que requieren conectividad inalámbrica.

### 8. Modem

El **Modem** es un dispositivo que convierte señales digitales en analógicas (modulación) y viceversa (demodulación), permitiendo que los datos se transmitan a través de líneas telefónicas o cables. Es utilizado para conectar redes locales a Internet.

- **Función principal**: Conectar una red local a Internet mediante la modulación de señales.
- **Uso**: Redes domésticas y pequeñas oficinas que acceden a Internet a través de un proveedor de servicios.

### 9. Repeater (Repetidor)

Un **Repeater** amplifica la señal de red para extender su alcance. Es útil en redes grandes o en lugares donde las señales pueden debilitarse por la distancia o por interferencias físicas.

- **Función principal**: Extender el alcance de una red amplificando la señal.
- **Uso**: Edificios grandes, áreas rurales, y redes donde las señales deben cubrir largas distancias.

### 10. Firewall

El **Firewall** es un dispositivo de seguridad que controla y filtra el tráfico entrante y saliente de una red. Puede ser un dispositivo de hardware o un conjunto de reglas de software que bloquea accesos no autorizados y protege la red de amenazas.

- **Función principal**: Proteger la red contra accesos no autorizados y ataques.
- **Uso**: Redes empresariales, gubernamentales y domésticas que requieren protección contra amenazas externas.

### 11. Load Balancer (Balanceador de Carga)

El **Load Balancer** distribuye el tráfico de red entre varios servidores o enlaces de red para mejorar el rendimiento y asegurar que ningún recurso se sobrecargue.

- **Función principal**: Distribuir el tráfico para optimizar el rendimiento y evitar sobrecargas.
- **Uso**: Empresas con infraestructuras de servidores o aplicaciones en la nube que manejan grandes volúmenes de tráfico.

## Unidad 2: Direccionamiento IP y División en subredes


### Clases de Direcciones IP

#### Clase A
- **Bits de red:** Primeros 8 bits
- **Bits de hosts:** Últimos 24 bits
- **Empiezan por:** "0" en binario
- **Rango decimal:** 1 a 127

#### Clase B
- **Bits de red:** Primeros 16 bits
- **Bits de hosts:** Últimos 16 bits
- **Empiezan por:** "10" en binario
- **Rango decimal:** 128 a 191

#### Clase C
- **Bits de red:** Primeros 24 bits
- **Bits de hosts:** Últimos 8 bits
- **Empiezan por:** "110" en binario
- **Rango decimal:** 192 a 223

#### Clase D (Multidifusión)
- **Empiezan por:** "1110"

#### Clase E (Investigación)
- **Empiezan por:** "1111"

### Nombre de red y dirección IP de difusión (broadcast)

Supón que tenemos la típica red `192.168.0.0` (clase C) con máscara `255.255.255.0`. Esto es en binario: `11111111.11111111.11111111.00000000`, por tanto, tenemos 24 bits para red y 8 bits para hosts (equipos conectados). Así, el número de equipos conectados será:

$$
Nº\ hosts = 2^n
$$

$$
2^8 = 256 \text{ hosts}
$$

Pues no, incorrecto. Tenemos que tener en cuenta que en redes IP:

- La primera dirección IP (toda la parte de host a ceros), en este caso la `.00000000` (0 en decimal) se reserva para referirse a toda la red, y se le llama nombre de red **(Segmentos)**.
- La última dirección IP (toda la parte de host a unos), en este caso la `.11111111` (255 en decimal) se reserva para dirección de difusión (paquetes que se envían a todos los hosts de la red), y se le llama dirección IP de difusión **(Broadcast)**.

Aplicando este descarte, la fórmula correcta sería:

$$
Nº\ hosts = 2^n - 2
$$

Donde `n` es el número de bits designados a hosts.

En el primer ejercicio, el número de hosts posibles sería `2^8 - 2 = 254`, así que para la red `192.168.0.0` con máscara `255.255.255.0`:

- `192.168.0.0` es el nombre de red.
- Los hosts ocuparían las IPs desde `192.168.0.1` hasta `192.168.0.254`.
- `192.168.0.255` sería la dirección broadcast. Cuando un host envíe un paquete a esa dirección, lo recibirán todos excepto él (porque es el remitente).

#### Direcciones IP sin clase (CIDR)

En el principio de los tiempos:

- Una red clase A tenía siempre una máscara `255.0.0.0` (/8) (16 millones de hosts posibles).
- Una red clase B tenía siempre una máscara `255.255.0.0` (/16) (65532 hosts posibles).
- Una red clase C tenía siempre una máscara `255.255.255.0` (/24) (254 hosts posibles).

Pero luego se diseñó el enrutamiento sin clase (CIDR) (cuidado con el nombre que es falsillo). Casi siempre se usa el sistema sin clase:

- Una red clase A tiene una máscara `255.0.0.0` o superior (≥ /8) (como máximo 16M de hosts posibles).
- Una red clase B tiene una máscara `255.255.0.0` o superior (≥ /16) (como máximo 65532 hosts posibles).
- Una red clase C tiene una máscara `255.255.255.0` o superior (≥ /24) (como máximo 65532 hosts posibles).

Así, la red `192.168.0.0`, que es una red clase C, cuando se usa CIDR puede tener una máscara `/25`, `/26`…:

- Cuando tiene la máscara `255.255.255.0` (`11111111.11111111.11111111.00000000`) (/24) soporta hasta 254 hosts.
- Cuando tiene la máscara `255.255.255.128` (`11111111.11111111.11111111.10000000`) (/25) soporta hasta 126 hosts.
- Cuando tiene la máscara `255.255.255.192` (`11111111.11111111.11111111.11000000`) (/26) soporta hasta 62 hosts.
- Cuando tiene la máscara `255.255.255.224` (`11111111.11111111.11111111.11100000`) (/27) soporta hasta 30 hosts.
- Cuando tiene la máscara `255.255.255.240` (`11111111.11111111.11111111.11110000`) (/28) soporta hasta 14 hosts.
- Cuando tiene la máscara `255.255.255.248` (`11111111.11111111.11111111.11111000`) (/29) soporta hasta 6 hosts.
- Cuando tiene la máscara `255.255.255.252` (`11111111.11111111.11111111.11111100`) (/30) soporta hasta 2 hosts.

A la máscara de subred en notación “/24“, “/8”… se le llama prefijo CIDR.

