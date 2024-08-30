---
title: "U3: Sincronización y Comunicación de Procesos"
author: Gaston Quelali
date: 2024-08-01
layout: post
permalink: /sistemas-operativos/sincronizacion-comunicacion/
weight: 3
---

## 3.1. Condiciones de Competencia

### Concepto
Las condiciones de competencia (o *race conditions*) ocurren cuando múltiples procesos o hilos acceden y manipulan datos compartidos de forma concurrente, y el resultado final depende del orden de ejecución de los procesos. Si no se controla adecuadamente, esto puede llevar a comportamientos impredecibles y errores en el sistema.

### Ejemplo
Imaginemos dos procesos que intentan incrementar un contador compartido. Si ambos procesos leen el valor del contador al mismo tiempo, lo incrementan y luego lo escriben, el valor final del contador puede ser incorrecto, ya que ambos procesos habrían leído el mismo valor inicial antes de escribir el incremento.

### Prácticas
- **Simulación de condiciones de competencia:**
- **Discusión de soluciones:** 

## 3.2. El Problema de la Sección Crítica

### Concepto
El problema de la sección crítica es un problema clásico en la computación concurrente, que se refiere a la necesidad de controlar el acceso a la sección crítica de código, donde un recurso compartido es accedido o modificado. La solución debe garantizar que solo un proceso o hilo pueda ejecutar la sección crítica en un momento dado.

### Requisitos de la Solución
1. **Exclusión Mutua:** Solo un proceso puede estar en su sección crítica a la vez.
2. **Progreso:** Si ningún proceso está en la sección crítica, los procesos que desean entrar no deben ser impedidos de hacerlo.
3. **Espera Finita:** No se debe permitir que un proceso espere indefinidamente para entrar en su sección crítica.

### Ejemplo
Considera dos procesos que deben actualizar un archivo compartido. Si ambos intentan escribir en el archivo simultáneamente sin ningún mecanismo de control, los datos podrían corromperse.

### Prácticas
- **Implementación de soluciones clásicas:** 
- **Análisis de exclusión mutua en diferentes contextos:**

## 3.3. Problemas Clásicos de Sincronización

### Concepto
Los problemas clásicos de sincronización son problemas bien conocidos que ilustran las dificultades y técnicas de la sincronización de procesos. Estos problemas son utilizados para enseñar las técnicas básicas de sincronización y para mostrar las trampas comunes en el diseño de sistemas concurrentes.

### Ejemplos

#### 3.3.1. El Problema del Productor-Consumidor
Este problema describe una situación en la que un productor genera datos que son consumidos por un consumidor. La dificultad radica en coordinar a ambos para que el consumidor no intente consumir datos que no han sido producidos, y que el productor no sobrescriba datos que no han sido consumidos.

- **Práctica:** Implementar el problema del productor-consumidor usando semáforos para controlar el acceso al búfer compartido.

#### 3.3.2. El Problema de los Filósofos Comensales
Cinco filósofos se sientan alrededor de una mesa, cada uno con un tenedor a su izquierda y derecha. Para comer, un filósofo necesita ambos tenedores. El problema consiste en evitar que los filósofos caigan en un estado de espera indefinida (deadlock).

- **Práctica:** Implementar una solución al problema usando un protocolo de jerarquía de recursos o semáforos.

#### 3.3.3. El Problema de los Lectores y Escritores
Este problema involucra un recurso que puede ser leído por múltiples procesos simultáneamente, pero solo puede ser escrito por un proceso a la vez. La dificultad es permitir la máxima concurrencia para lectores mientras se garantiza la exclusión mutua para escritores.
