---
title: "U5: Gestión de la Memoria"
author: Gaston Quelali
date: 2024-08-01
layout: post
permalink: /sistemas-operativos/gestion-memoria/
weight: 5
---

## **5.1. Gestión de Memoria**
- **Concepto de Memoria en Sistemas Operativos**:
  - **Analogía**: Imagina la memoria de un computador como un gran estante lleno de cajas. Cada caja puede almacenar algo importante, como datos o instrucciones para que el procesador las ejecute. La gestión de la memoria es el proceso mediante el cual el sistema operativo decide qué va en cada caja, cómo acceder a ellas, y cómo liberar espacio cuando ya no se necesiten.

- **Memoria Física vs. Memoria Virtual**:
  - **Memoria Física**: Es como el espacio físico en tu estante. Solo tienes una cantidad limitada de espacio donde puedes colocar tus cajas (datos). En un computador, esto se refiere a la RAM (Random Access Memory), que es la memoria física disponible.
  - **Memoria Virtual**: Es como tener un estante infinito en la nube que puedes usar cuando se te acabe el espacio físico en tu estante real. El sistema operativo usa la memoria virtual para simular más espacio del que realmente existe, moviendo datos entre la RAM y el almacenamiento secundario (disco duro) según sea necesario.

- **Paginación y Segmentación**:
  - **Paginación**:
    - **Analogía de Paginación**: Imagina que divides tu estante en pequeñas secciones iguales (páginas) y colocas partes de tus cajas en ellas. Si necesitas algo de una caja que no está en tu estante (memoria física), simplemente intercambias una de las secciones con otra que está almacenada en un lugar secundario (memoria virtual). La paginación divide la memoria en partes iguales, facilitando la gestión del espacio disponible.
  - **Segmentación**:
    - **Analogía de Segmentación**: En lugar de dividir el estante en partes iguales, puedes dividirlo según el tamaño de las cajas (segmentos). Una caja puede ser más grande que otra, y el sistema operativo administra el espacio asignando segmentos de tamaño variable, dependiendo de las necesidades del programa.

- **Problemas de Gestión de Memoria**:
  - **Fragmentación**:
    - **Fragmentación Interna**: Es como tener pequeñas partes de tu estante que están parcialmente llenas y no puedes usarlas para almacenar una nueva caja, incluso si hay espacio suficiente.
    - **Fragmentación Externa**: Es cuando tienes varios espacios vacíos en tu estante, pero están tan dispersos que no puedes usarlos eficientemente para almacenar una caja grande.

## **5.2. Administración de Memoria**
- **Asignación de Memoria**:
  - **Asignación Contigua**:
    - **Analogía**: Piensa en reservar un conjunto de casilleros consecutivos para guardar tus pertenencias en un gimnasio. La asignación contigua es similar: se asigna un bloque de memoria consecutiva para un proceso. Esto es simple, pero puede llevar a problemas de fragmentación externa si los bloques libres no son lo suficientemente grandes para los nuevos procesos.
  - **Asignación No Contigua**:
    - **Analogía**: Imagina que puedes guardar tus pertenencias en cualquier casillero disponible en el gimnasio, sin necesidad de que estén uno al lado del otro. En los sistemas operativos, esto permite asignar bloques de memoria en diferentes lugares, ayudando a mitigar la fragmentación externa.

- **Técnicas de Asignación de Memoria**:
  - **Primer Ajuste (First Fit)**:
    - **Analogía**: Es como colocar una caja en el primer espacio libre que encuentres en tu estante, sin preocuparte si hay un espacio mejor más adelante.
  - **Mejor Ajuste (Best Fit)**:
    - **Analogía**: Aquí, te tomas el tiempo para encontrar el espacio que mejor se ajuste a la caja que quieres almacenar, asegurándote de no desperdiciar ningún espacio.
  - **Peor Ajuste (Worst Fit)**:
    - **Analogía**: En lugar de buscar el mejor espacio, buscas el más grande, con la idea de que al dividirlo, podrás usar el resto para almacenar otras cajas más adelante.

- **Memoria Virtual**:
  - **Swapping**:
    - **Analogía**: Imagina que tienes un estante pequeño y muchas cajas. Cuando el estante se llena, tienes que mover algunas cajas a un almacén temporal para hacer espacio para nuevas cajas. En sistemas operativos, el swapping funciona de manera similar, moviendo procesos entre la memoria física y el almacenamiento secundario para optimizar el uso de la memoria.

- **Administradores de Memoria**:
  - **Función del Administrador de Memoria**: 
    - **Analogía**: El administrador de memoria es como el encargado de un almacén. Su trabajo es mantener un inventario de todas las cajas (datos) y asegurarse de que cada una esté en el lugar correcto. El administrador de memoria del sistema operativo se encarga de asignar, rastrear, y liberar memoria según las necesidades de los procesos.

- **Protección de Memoria**:
  - **Analogía**: Es como tener cerraduras en tus casilleros para que solo tú puedas acceder a tus pertenencias. La protección de memoria evita que un proceso interfiera con la memoria de otro proceso, garantizando que cada uno opere de manera segura y sin conflictos.
