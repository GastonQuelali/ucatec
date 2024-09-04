---
title: "U6: Memoria Virtual"
author: Gaston Quelali
date: 2024-08-01
layout: post
permalink: /sistemas-operativos/memoria-virtual/
weight: 6
---

## 6.1. Estrategias de Búsqueda (Paginación)
- **Concepto de Paginación**:
  - **Analogía**: Imagina que tu escritorio está lleno de libros abiertos. Como no tienes suficiente espacio, decides solo dejar los más importantes y almacenar los demás en una estantería cercana. Cada vez que necesites un libro que no esté en tu escritorio, debes ir a la estantería a buscarlo. En un sistema operativo, la paginación funciona de manera similar, moviendo fragmentos de datos entre la memoria principal y el almacenamiento secundario según sea necesario.

- **Memoria Virtual y Paginación**:
  - **Memoria Virtual**: Piensa en la memoria virtual como un escritorio infinito donde puedes trabajar con más libros de los que físicamente caben en tu escritorio. Esta memoria permite que un sistema ejecute más procesos de los que la RAM podría manejar por sí sola, intercambiando datos entre la memoria física y el disco duro.
  - **Paginación**: Se refiere a la división de la memoria virtual en bloques de tamaño fijo llamados "páginas". Estas páginas se almacenan en la memoria física cuando son necesarias y se intercambian con otras según lo requiera el sistema.

- **Estrés de Paginación**:
  - **Page Fault**: Es como descubrir que el libro que necesitas no está en tu escritorio, lo que te obliga a ir a buscarlo en la estantería. En términos de sistemas operativos, un *page fault* ocurre cuando el sistema necesita acceder a una página que no está en la memoria física, lo que genera una pausa mientras se busca y se carga esa página.

- **Estrategias de Búsqueda**:
  - **Buscando en la Estantería**: Al igual que en una biblioteca, la estrategia que uses para buscar un libro influye en cuánto tiempo tardas en encontrarlo. En un sistema, las estrategias de búsqueda determinan cómo el sistema localiza y carga las páginas necesarias en la memoria física.
  - **Paginación Demanda**: Es como traer un libro a tu escritorio solo cuando realmente lo necesitas. La paginación por demanda carga páginas en la memoria solo cuando se requieren, lo que puede reducir el uso innecesario de memoria, pero también puede aumentar los *page faults*.

## 6.2. Algoritmos de Sustitución de Páginas
- **Concepto de Sustitución de Páginas**:
  - **Analogía**: Imagina que tu escritorio está completamente lleno de libros, y necesitas espacio para uno nuevo. Debes decidir cuál de los libros actuales vas a devolver a la estantería para hacer espacio. Los algoritmos de sustitución de páginas en sistemas operativos se encargan de tomar decisiones similares cuando la memoria física está llena y una nueva página necesita ser cargada.

- **Algoritmos Comunes de Sustitución**:
  - **FIFO (First In, First Out)**:
    - **Analogía**: Es como devolver el libro que has tenido en tu escritorio por más tiempo, sin importar si aún lo necesitas o no. Este método es simple pero puede no ser el más eficiente, ya que podría eliminar páginas que aún son necesarias.
  - **LRU (Least Recently Used)**:
    - **Analogía**: Aquí, devuelves el libro que no has consultado en mucho tiempo. Este método asume que si no has usado una página recientemente, es menos probable que la necesites en un futuro cercano. LRU es más eficiente que FIFO, pero requiere más recursos para rastrear el uso de cada página.
  - **Optimal**:
    - **Analogía**: Idealmente, elegirías devolver el libro que no vas a necesitar por un tiempo considerable. El algoritmo óptimo hace exactamente eso, pero en la práctica, es difícil de implementar porque requiere conocimiento del futuro, algo que los sistemas operativos no pueden predecir.

- **Otros Algoritmos de Sustitución**:
  - **Algoritmo de Segunda Oportunidad**:
    - **Analogía**: Es como revisar cada libro antes de devolverlo, dándole una segunda oportunidad si consideras que aún podría ser útil. Este método mejora FIFO al evitar eliminar páginas que han sido referenciadas recientemente, dándoles una segunda oportunidad antes de ser reemplazadas.
  - **Algoritmo del Reloj**:
    - **Analogía**: Imagina un reloj donde cada libro está representado por una posición en el círculo. A medida que avanzas por el reloj, revisas cada libro (página) y decides si debe quedarse o ser reemplazado. Este algoritmo es una variación del de segunda oportunidad y es eficiente en términos de recursos.

- **Evaluación de Algoritmos**:
  - **Coste de Page Faults**:
    - **Analogía**: Considera cuánto tiempo y esfuerzo cuesta ir a buscar un libro que no está en tu escritorio. En sistemas operativos, el coste de los *page faults* es crítico para determinar la eficiencia de un algoritmo de sustitución de páginas. Un buen algoritmo minimiza estos fallos, mejorando el rendimiento del sistema.
  - **Equilibrio entre Complejidad y Eficiencia**:
    - **Decisión Estratégica**: Como un jugador de ajedrez, el sistema operativo debe equilibrar la simplicidad de un algoritmo con su efectividad en el uso de la memoria. Algoritmos más simples como FIFO son fáciles de implementar pero pueden ser ineficientes, mientras que algoritmos más complejos como LRU pueden ofrecer mejores resultados a un coste computacional más alto.
