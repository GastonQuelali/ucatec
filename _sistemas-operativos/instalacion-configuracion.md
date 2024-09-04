---
title: "U8: Instalación y Configuración de Sistemas Operativos"
author: Gaston Quelali
date: 2024-08-01
layout: post
permalink: /sistemas-operativos/instalacion-configuracion/
weight: 8
---

## 8.1: Partición y Formateo de Unidades de Disco Duro

### Explicación de los Conceptos de Partición y Formateo
- **Partición**: Dividir un disco duro en partes separadas que actúan como discos independientes.
- **Formateo**: Preparar una partición para almacenar datos, aplicando un sistema de archivos.

### Tipos de Particiones
- **Particiones Primarias**: Hasta 4 particiones, o 3 primarias y 1 extendida.
- **Particiones Extendidas**: Puede contener múltiples particiones lógicas.
- **Particiones Lógicas**: Subdivisiones dentro de una partición extendida.

### Herramientas y Comandos para Particionar y Formatear
- **Windows**: 
  - Disk Management (`diskmgmt.msc`)
  - `diskpart`
- **Linux**: 
  - `fdisk`
  - `parted`
  - `mkfs`
- **macOS**:
  - Disk Utility
  - `diskutil`

---

## 8.2: Sistemas Operativos para PC

### Comparativa de Sistemas Operativos Comunes para PC
- **Windows**:
  - Uso masivo, soporte amplio de software.
  - Licencia comercial.
- **macOS**:
  - Integración con hardware Apple, interfaz intuitiva.
  - Licencia comercial.
- **Linux**:
  - Open-source, personalización y seguridad.
  - Distribuciones populares: Ubuntu, Fedora, Debian.

### Instalación Paso a Paso y Consideraciones Importantes
- **Windows**:
  1. Crear medio de instalación (USB/DVD).
  2. Configurar BIOS/UEFI para arrancar desde el medio.
  3. Seguir el asistente de instalación.
- **macOS**:
  1. Usar el modo de recuperación o medio de instalación USB.
  2. Seleccionar disco de destino y particionar si es necesario.
  3. Completar la instalación siguiendo los pasos.
- **Linux**:
  1. Crear USB booteable con la distribución deseada.
  2. Configurar BIOS/UEFI para arrancar desde USB.
  3. Seguir el instalador gráfico o en línea de comandos.

---

## 8.3: Sistemas Operativos para Servidor

### Características de los Sistemas Operativos de Servidor
- **Windows Server**:
  - Soporte empresarial, Active Directory, administración centralizada.
- **Ubuntu Server**:
  - Open-source, fácil de usar, soporte de LTS.
- **CentOS**:
  - Open-source, estabilidad a largo plazo, soporte comunitario.

### Procedimiento de Instalación y Configuración Básica
- **Instalación**:
  1. Crear medio de instalación (USB/DVD).
  2. Configurar BIOS/UEFI para arrancar desde el medio.
  3. Seguir el asistente de instalación.
- **Configuración Básica**:
  - Configuración de red, usuarios, y roles de servidor.
  - Instalación de paquetes y servicios necesarios.

---

## 8.4: Sistemas Operativos Portables

### Definición y Ejemplos (Tails, Puppy Linux)
- **Definición**: Ejecutables desde medios extraíbles sin instalación.
- **Ejemplos**:
  - **Tails**: Enfoque en privacidad y anonimato.
  - **Puppy Linux**: Ligero y eficiente, adecuado para hardware limitado.

### Ventajas y Desventajas de Usar Sistemas Operativos Portables
- **Ventajas**:
  - Portabilidad, privacidad, recuperación de sistemas.
- **Desventajas**:
  - Limitaciones de rendimiento, compatibilidad variable.

### Procedimiento de Creación de Sistemas Operativos Portables
- **Paso a Paso**:
  1. Descargar ISO del sistema.
  2. Usar herramientas como Rufus o UNetbootin para crear un USB booteable.
  3. Configurar BIOS/UEFI para arrancar desde USB.
  4. Probar el sistema en un ordenador.

---

## 8.5: Arranque de los Sistemas Operativos

### Explicación del Proceso de Arranque
- **Fases del Proceso de Arranque**:
  1. **POST**: Verificación de hardware.
  2. **Carga del Bootloader**: Desde MBR o GPT.
  3. **Carga del Sistema Operativo**: Kernel a la memoria.
  4. **Inicialización**: Servicios y entorno gráfico.

### Diferencias entre BIOS y UEFI
- **BIOS**:
  - Interfaz de 16 bits, compatibilidad con sistemas antiguos.
  - Soporta discos de hasta 2 TB, particiones MBR.
- **UEFI**:
  - Interfaz moderna de 32/64 bits, arranque rápido.
  - Soporte para discos grandes, particiones GPT.

### Solución de Problemas Comunes en el Arranque
- **Problemas Comunes**:
  - Sistema no encontrado, fallo en el bootloader, pantalla azul/kernel panic.
- **Soluciones**:
  - Verificar secuencia de arranque, reinstalar bootloader, diagnóstico de hardware.

---

## 8.6: Boot

### Descripción Detallada del Proceso de Boot
- **Proceso**:
  1. Carga del bootloader.
  2. Selección del sistema operativo.
  3. Carga del kernel.
  4. Inicialización de drivers y servicios.

### Diferencias entre los Distintos Gestores de Arranque (GRUB, Windows Boot Manager)
- **GRUB**:
  - Utilizado en Linux, personalización avanzada, multiboot.
- **Windows Boot Manager**:
  - Para sistemas Windows, simplicidad, menos personalizable.

---

## 8.7: Multiboot

### Configuración de un Sistema Multiboot
- **Pasos Clave**:
  1. Particionar el disco.
  2. Instalar los sistemas operativos.
  3. Configurar el bootloader (GRUB o Windows Boot Manager).

### Uso de Gestores de Arranque para Manejar Múltiples Sistemas Operativos
- **GRUB**:
  - Configuración de `grub.cfg`, personalización del menú.
- **Windows Boot Manager**:
  - Agregar Linux al menú de arranque de Windows.

---

## 8.8: Virtualización de Sistemas Operativos

### Conceptos Básicos de Virtualización
- **Definición**: Ejecutar múltiples sistemas operativos en un solo hardware mediante máquinas virtuales.
- **Tipos**:
  - **Virtualización Completa**: Emulación completa de hardware.
  - **Paravirtualización**: El sistema huésped está optimizado para virtualización.

### Configuración de Máquinas Virtuales Usando VirtualBox y VMware
- **Configuración Básica**:
  1. Crear una nueva máquina virtual.
  2. Configurar discos y red.
  3. Instalar el sistema operativo.
