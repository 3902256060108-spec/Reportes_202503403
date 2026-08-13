# Proyecto de Virtualización y Redes

## Descripción
ESTUDIANTE: Yessenia Crystabel Mazariegos Carranza 202503403

Este proyecto presenta dos videos prácticos relacionados con la instalación, configuración y comunicación de sistemas GNU/Linux y Windows. Se documentan los procedimientos realizados, las herramientas utilizadas y los principales problemas encontrados durante el desarrollo de las prácticas.

---

# 🎥 Video 1: Instalación y Configuración de GNU/Linux

### Instalación y Configuración de Ubuntu 26.04 LTS en VirtualBox

<a href="https://youtu.be/nn9Dk8Clib4">
  <img src="https://img.youtube.com/vi/nn9Dk8Clib4/maxresdefault.jpg" alt="Miniatura Video 1" width="700">
</a>

▶️ **[Ver Video 1 en YouTube](https://youtu.be/nn9Dk8Clib4?si=DuZpG11gH6z_hnYH)**

### Contenido

En este video se presenta el proceso de instalación y configuración de **Ubuntu 26.04 LTS** mediante una máquina virtual en Oracle VirtualBox.

Se incluyen:

- Presentación y fundamentos de GNU/Linux.
- Descarga de la imagen ISO oficial de Ubuntu.
- Comprobación de integridad mediante **SHA-256**.
- Creación y configuración de la máquina virtual.
- Instalación de Ubuntu 26.04 LTS.
- Configuración posterior a la instalación.
- Actualización del sistema.
- Revisión de controladores y software.
- Instalación/configuración de herramientas de integración de VirtualBox.
- Resolución de problemas encontrados durante la instalación.

---

# 🌐 Video 2: Configuración de Redes Heterogéneas

### Configuración y Validación de Redes Windows ↔ Ubuntu

<a href="https://youtu.be/OWMZO-5bzEA">
  <img src="https://img.youtube.com/vi/OWMZO-5bzEA/maxresdefault.jpg" alt="Miniatura Video 2" width="700">
</a>

▶️ **[Ver Video 2 en YouTube](https://youtu.be/OWMZO-5bzEA)**

### Contenido

En este video se presenta la configuración y validación de redes heterogéneas entre **Windows y Ubuntu**, utilizando máquinas físicas y virtuales.

Se incluyen:

- Fundamentos de redes cableadas.
- Direccionamiento IPv4 e IPv6.
- Máscaras de subred.
- Configuración de adaptadores de red en VirtualBox.
- Conexiones entre sistemas Windows y GNU/Linux.
- Validación mediante:
  - `ipconfig`
  - `ip addr`
  - `ping`
  - `tracert`
  - `traceroute`
  - `netstat`
  - `ss`
- Comprobación de conectividad.
- Revisión del Firewall de Windows.
- Resolución de problemas de comunicación entre los equipos.

---

# 📝 Bitácora de Problemas Encontrados

## Video 1 — Instalación y Configuración de Ubuntu

### 1. Problema con la configuración gráfica de VirtualBox

Durante el primer arranque de Ubuntu apareció un mensaje relacionado con **VMSVGA** y una configuración gráfica no compatible.

**Solución aplicada:**

Se revisó la configuración de pantalla de la máquina virtual y se modificó el controlador gráfico para utilizar una configuración compatible. Posteriormente se reinició la máquina virtual.

---

### 2. Ubuntu tardó demasiado en iniciar

Después de modificar la configuración gráfica, Ubuntu permaneció durante varios minutos en la pantalla de carga.

**Solución aplicada:**

Se esperó a que terminara el proceso de arranque. Finalmente, Ubuntu inició correctamente y mostró el asistente de bienvenida.

---

### 3. Problemas con VirtualBox Guest Additions

Al intentar insertar la imagen de CD de **Guest Additions**, el instalador no se ejecutó automáticamente y posteriormente apareció un error relacionado con permisos.

**Solución aplicada:**

Se verificó que la imagen de Guest Additions estuviera montada correctamente y se revisó el contenido del medio desde Ubuntu.

---

### 4. Controladores adicionales

La opción de controladores adicionales no aparecía directamente dentro de la configuración normal del sistema.

**Solución aplicada:**

Se abrió la herramienta:

```bash
software-properties-gtk
