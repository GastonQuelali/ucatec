---
title: "U7: Sistema de Archivos"
author: Gaston Quelali
date: 2024-08-01
layout: post
permalink: /sistemas-operativos/sistema-archivos/
weight: 7
---

## **7.1. Archivos**
- **Concepto de Archivo**:
  - **Analogía**: Piensa en un archivo como en un libro. Un archivo contiene datos, tal como un libro contiene texto, imágenes o diagramas. Estos datos pueden ser cualquier cosa, desde un documento de texto hasta un programa de software.
  
- **Tipos de Archivos**:
  - **Archivos de Texto**: Como libros llenos de palabras. Contienen datos en un formato legible por humanos.
  - **Archivos Binarios**: Son como manuales técnicos con código especializado. Contienen datos en un formato legible por máquinas, como programas ejecutables.
  - **Archivos de Datos**: Actúan como registros de un inventario, conteniendo datos estructurados, a menudo utilizados por bases de datos.

- **Atributos de los Archivos**:
  - **Nombre**: El título del libro, que permite identificarlo.
  - **Tipo**: Similar al género de un libro (novela, poesía, etc.), el tipo de archivo define cómo deben ser interpretados los datos en su interior.
  - **Tamaño**: La cantidad de páginas en el libro, o el espacio que ocupa el archivo en el disco.
  - **Permisos**: Determina quién puede leer, escribir o ejecutar el archivo, como las reglas de una biblioteca que especifican quién puede acceder a ciertos libros.

- **Operaciones con Archivos**:
  - **Creación**: Es como escribir un nuevo libro. Se reserva espacio en el disco y se le da un nombre.
  - **Lectura**: Similar a abrir un libro para leer su contenido.
  - **Escritura**: Es como agregar nuevas páginas a un libro o editar el contenido existente.
  - **Eliminación**: Como deshacerse de un libro viejo, liberando espacio en el estante.

## **7.2. Directorios**
- **Concepto de Directorio**:
  - **Analogía**: Imagina que un directorio es como una estantería en una biblioteca. Cada estantería contiene libros (archivos) y puede contener otras estanterías (subdirectorios), organizando todo de manera jerárquica.

- **Estructura de Directorios**:
  - **Jerarquía de Directorios**: Es como una organización de estanterías en una biblioteca, donde puedes tener una estantería principal con subestanterías dentro de ella.
  - **Directorios Raíz y Subdirectorios**: El directorio raíz es la estantería principal de la biblioteca, mientras que los subdirectorios son estanterías dentro de otras estanterías.

- **Operaciones con Directorios**:
  - **Creación de Directorios**: Es como agregar una nueva estantería a la biblioteca.
  - **Eliminación de Directorios**: Similar a desmantelar una estantería y mover o eliminar los libros que contiene.
  - **Navegación en Directorios**: Es como recorrer la biblioteca buscando libros en diferentes estanterías.

- **Directorios Especiales**:
  - **Directorio Actual (`.`)**: Es como tu posición actual en la biblioteca.
  - **Directorio Padre (`..`)**: Te lleva a la estantería anterior, como retroceder a la sección de la biblioteca de donde vienes.

## **7.3. Implementación de Sistemas de Archivos**
- **Estructura de un Sistema de Archivos**:
  - **Analogía**: Un sistema de archivos es como el catálogo de la biblioteca, que sabe dónde está cada libro (archivo) y cómo acceder a él. La implementación de un sistema de archivos involucra la manera en que los datos se organizan, almacenan, y se recuperan en el almacenamiento físico.

- **Métodos de Asignación de Espacio**:
  - **Asignación Contigua**:
    - **Analogía**: Es como asignar una sección completa del estante para un solo libro largo. Es fácil de leer, pero si el libro crece, podrías quedarte sin espacio.
  - **Asignación Enlazada**:
    - **Analogía**: Es como tener un libro cuyas páginas están dispersas en diferentes estantes, con notas que indican dónde encontrar la siguiente página. Esto permite un uso flexible del espacio, pero puede ser más lento leer el libro completo.
  - **Asignación Indexada**:
    - **Analogía**: Es como un libro que tiene un índice al comienzo, indicando dónde se encuentra cada capítulo. Facilita la búsqueda rápida, pero requiere más espacio para mantener el índice.

- **Gestión de Espacio Libre**:
  - **Listas Enlazadas**: Mantiene una lista de estantes vacíos donde pueden colocarse nuevos libros.
  - **Mapas de Bits**: Un mapa de bits es como un plano de la biblioteca, donde cada estante está marcado como lleno o vacío, permitiendo una rápida identificación de espacios libres.

- **Montaje y Desmontaje de Sistemas de Archivos**:
  - **Montaje**: Es como abrir una nueva sección de la biblioteca al público. El sistema operativo necesita montar el sistema de archivos para que los usuarios puedan acceder a los datos en él.
  - **Desmontaje**: Es como cerrar una sección de la biblioteca. Antes de desmontar, el sistema asegura que no haya usuarios accediendo a los datos para evitar pérdidas de información.

- **Caché de Sistema de Archivos**:
  - **Analogía**: Es como tener un carrito de libros populares cerca de la entrada de la biblioteca. La caché almacena datos recientemente usados para un acceso más rápido, reduciendo la necesidad de buscar en todo el sistema de archivos.

- **Seguridad y Permisos**:
  - **Analogía**: Al igual que un sistema de membresía en una biblioteca, la seguridad del sistema de archivos controla quién puede acceder y modificar los archivos, protegiendo los datos de accesos no autorizados.

