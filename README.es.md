<div align="center">

# 🎮 Gaming Optimizer

[![Version](https://img.shields.io/badge/version-4.1.0-blue.svg)](https://github.com/derzslows/GamingOptimizer/releases/latest)
[![Windows](https://img.shields.io/badge/Windows-10%20%7C%2011%20(x64)-0078D6.svg?logo=windows)](#%EF%B8%8F-requisitos-del-sistema)
[![.NET](https://img.shields.io/badge/.NET%208%20%C2%B7%20WinUI%203-512BD4.svg?logo=dotnet)](#)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Languages](https://img.shields.io/badge/i18n-English%20%7C%20Espa%C3%B1ol-orange.svg)](#)

**Un optimizador de Windows potente, moderno y totalmente reversible para gaming, rendimiento, latencia y privacidad.**

[English](README.md) · **Español**

</div>

> **Principio rector:** *todo lo que se desactiva se puede volver a activar.* Cada cambio captura su estado previo y es reversible —incluso tras reiniciar—, respaldado por un diario persistente y un punto de restauración de Windows opcional antes de los lotes.

<div align="center">

![Panel](https://github.com/user-attachments/assets/474d4e81-0031-4a40-8e52-e4c9daf4369e)

</div>

---

## 📋 Tabla de contenidos

- [Descripción](#-descripción)
- [Características](#-características)
- [Capturas](#-capturas)
- [Instalación](#-instalación)
- [Requisitos del sistema](#️-requisitos-del-sistema)
- [Novedades de la 4.1.0](#-novedades-de-la-410)
- [Reversibilidad y seguridad](#️-reversibilidad-y-seguridad)
- [Aviso](#️-aviso)
- [Licencia](#-licencia)
- [Autor](#-autor)

---

## 📝 Descripción

**Gaming Optimizer** ayuda a gamers y usuarios avanzados a exprimir Windows. Combina **~170 optimizaciones reversibles**, un **benchmark real** para medir el antes/después, un boost de un clic con la **Sesión de juego**, **perfiles portables** para compartir tu configuración completa, **diagnóstico**, **gestión de controladores**, **monitorización en tiempo real** y un **gestor de apps** completo — en una única interfaz moderna, en **español e inglés**.

A diferencia de los "scripts de tweaks" de un solo uso, aquí cada optimización se aplica con un motor reversible: puedes experimentar con confianza y revertir cualquier cambio, individualmente o todos a la vez.

---

## ✨ Características

### 🎛️ Optimizaciones — ~170, reversibles
Ajustes curados y documentados en **15 categorías**: Gaming, CPU, GPU, Memoria, Almacenamiento, Red, Energía, Latencia/timers, Entrada, Apariencia/DWM, Privacidad/Telemetría, Servicios, Inicio y Sistema. Con búsqueda y filtro, modos **Fácil / Avanzado**, *Aplicar recomendadas* y *Restaurar todo*. Sin *snake‑oil*: solo cambios reales y documentados.

### 📈 Rendimiento — mide, no adivines *(nuevo en 4.1)*
- **Salud gaming (0–100)** adaptada a tu hardware: Hz del monitor frente a su máximo real, plan de energía, XMP/EXPO, Game DVR, deriva de optimizaciones, punto de restauración y más. Lo que no aplica a tu equipo se excluye — nada te penaliza sin motivo. Cada punto pendiente tiene su botón **Arreglar**.
- **Benchmark real (antes / después)**: CPU (mono y multinúcleo), RAM, disco (lectura honesta sin caché) y jitter de latencia del sistema en ~25 segundos. Mide antes y después de optimizar y ve la mejora real por métrica. Cifras comparables en tu propio equipo — sin números inventados.

### ⚡ Sesión de juego — boost de un clic *(nuevo en 4.1)*
Un **boost temporal y 100 % reversible** mientras juegas: plan de energía al máximo, Windows Update / BITS / Delivery Optimization en pausa y timer del sistema a 1 ms. Al terminar la sesión todo vuelve exactamente a como estaba; si cierras la app o reinicias a medias, el Panel te recuerda que sigue activa — nada queda a medias.

### 💾 Perfiles portables (.goprofile) *(nuevo)*
Exporta tu configuración completa a un fichero pequeño y compártelo o restáuralo tras formatear Windows: **optimizaciones (con categorías a la carta), preferencias de la app e incluso tus apps instaladas**. Al importar se muestra una vista previa completa —qué se aplicará, qué no encaja en ese hardware (los tweaks solo‑NVIDIA se omiten limpiamente en AMD), qué requiere confirmación— y el que recibe elige qué categorías aplicar. **Seguro por diseño**: el fichero solo lleva identificadores, nunca comandos. Doble clic en un `.goprofile` y la app se abre directa en la vista previa.

### 📊 Panel
Vista general en tiempo real: puntuación de salud gaming, gráfica de red en vivo (ventana de 60 s, adaptador activo, picos de la sesión), nombres y modelos de hardware, todos los discos con su uso, datos de CPU/GPU/RAM, caché y XMP, activación de Windows, y la tarjeta **Seguridad de cambios** con tu último punto de restauración y los cambios del diario.

### 🔎 Búsqueda global *(nuevo en 4.1)*
Un buscador en la barra lateral que encuentra al instante cualquier optimización, app del catálogo o página — y te lleva directo, ya filtrado.

### 🧰 Herramientas
- **🆔 Identificación de hardware** — todos los identificadores únicos del equipo en un sitio: BIOS/SMBIOS, placa base, CPU (ProcessorID, microcódigo, caché), GPU, módulos de RAM, discos (serie / ID único / GUID), volúmenes, particiones, monitores (EDID + SHA‑256), MAC/GUID de red, Bluetooth, audio, controladoras USB, TPM, Secure Boot, Product ID de Windows, Machine GUID y SID — con **Copiar informe** en un clic.
- **🧩 Drivers** — detector, inspector y gestor completo de controladores: dispositivos, kernel/servicios y módulos kernel cargados, con info de firma y de terceros, **detección de anomalías** y desinstalación de paquetes de terceros.
- **🖥️ Pantalla** — modelo real del monitor, interruptor **HDR**, resolución nativa, escala, frecuencia de refresco (con aviso de "usar el máximo"), rotación y cambio de pantalla principal, leídos del EDID de cada monitor.
- **⚡ Planes de energía y GPU** — revela/gestiona planes (incl. Rendimiento máximo) y utilidades de GPU/driver.
- **🌐 Red** — monitor de tráfico en tiempo real, **inspector de conexiones por proceso** y un panel de diagnóstico gaming: comprobación de conectividad por capas, test de calidad (pérdida de paquetes/latencia/jitter), traceroute y descubrimiento de MTU.
- **🚀 Inicio** — gestiona qué arranca con Windows.
- **📜 Historial de cambios** — revisa todo lo aplicado y revierte entradas individualmente o todas a la vez; el Panel avisa si Windows Update u otra herramienta deshace tus optimizaciones en silencio (**detección de deriva**).

### 🧹 Mantenimiento
- **📦 Apps & Debloat** — un gestor de apps completo en tres pestañas:
  - **Instalar**: ~250 apps curadas vía `winget` (navegadores, gaming, emuladores, desarrollo, monitorización, seguridad…) con búsqueda, categorías, **instalación por lotes** y **ficha de detalles** (ⓘ) por app: info real del sistema en las instaladas, descripción/editor/licencia completas en el resto.
  - **Actualizar**: todas las apps de tu equipo con actualización pendiente — una a una o **todas de golpe con progreso en vivo**; los instaladores rebeldes tienen "Reintentar en ventana".
  - **Quitar**: desinstala bloatware UWP preinstalado, y desinstala apps del catálogo (siempre con confirmación).
- **🧽 Limpieza** — recupera espacio en disco de forma segura, incluida la **caché de shaders** (DirectX, NVIDIA, AMD, Intel) para arreglar el stutter tras actualizar drivers.

### 🔒 Módulo Seguridad ↔ Rendimiento *(Avanzado, opt‑in)*
Permite desactivar opcionalmente **VBS**, **Integridad de memoria (HVCI)**, **mitigaciones Spectre/Meltdown**, **Credential Guard** y el **hipervisor** — cada uno con avisos claros y totalmente reversible. Oculto en modo Fácil y con confirmación explícita.

### Además
♻️ Motor totalmente reversible · 🖼️ **UI responsive** moderna (se adapta a ultrawide/alta resolución) · 🌍 Español e inglés · 🔄 Actualizaciones automáticas.

---

## 📸 Capturas

| Panel | Optimizaciones |
|---|---|
| ![Panel](https://github.com/user-attachments/assets/474d4e81-0031-4a40-8e52-e4c9daf4369e) | ![Optimizaciones](https://github.com/user-attachments/assets/db89651e-5563-49b1-9aeb-7388f95f3e1b) |
| **Herramientas de red** | **Instalador de apps** |
| ![Herramientas de red](https://github.com/user-attachments/assets/4f1969de-54ba-4230-9b52-7365fb29059c) | ![Instalador de apps](https://github.com/user-attachments/assets/26254cb3-97bc-41de-b4dd-1fbac9d14e79) |

---

## 📥 Instalación

1. Descarga **`GamingOptimizer-x.y.z.msi`** desde la [última release](https://github.com/derzslows/GamingOptimizer/releases/latest).
2. Ejecuta el instalador (se te pedirá confirmar permisos de administrador).
3. Si ya tienes una versión anterior, se **actualiza automáticamente**.

La app es autónoma: el runtime de .NET va incluido, no hay que instalar nada más. El instalador asocia además los ficheros **`.goprofile`**, así los perfiles compartidos se abren con doble clic.

---

## ⚙️ Requisitos del sistema

| | |
|---|---|
| **SO** | Windows 10 o Windows 11 (64 bits) |
| **Privilegios** | Administrador (la app corre elevada) |
| **Runtime** | Ninguno — incluido en el instalador |

---

## 🚀 Novedades de la 4.1.0

- 📈 **Página Rendimiento**: salud gaming (0–100) adaptada a tu hardware con arreglos de un clic + **benchmark real antes/después** (CPU, RAM, disco sin caché, jitter de latencia).
- ⚡ **Sesión de juego**: boost temporal de un clic (plan al máximo, updates en pausa, timer a 1 ms), todo por el diario y reversible.
- 🔎 **Búsqueda global** de optimizaciones, apps y páginas.
- 📦 **Apps & Debloat, reconstruido**: pestañas, ~250 apps curadas, instalación por lotes, fichas de detalles por app, pestaña **Actualizar** completa con progreso en vivo y "Reintentar en ventana", y desinstalación con confirmación.
- 💾 **Perfiles**: tus apps instaladas viajan dentro del `.goprofile`, categorías seleccionables al exportar y al importar (a la carta), y los perfiles se abren con doble clic.
- 🧹 Limpieza de caché de shaders ampliada a AMD (OpenGL/Vulkan) e Intel.

<details>
<summary>4.0.x</summary>

- **4.0.3** — Arreglo de la página Pantalla: faltaba el primer monitor con varias pantallas.
- **4.0.2** — **Perfiles portables (.goprofile)**: exporta/importa tu configuración de forma segura entre hardware distinto; Panel más rico (gráfica de red en vivo, tarjeta de seguridad de cambios).
- **4.0.0** — **Rediseño Fluent / Windows 11** completo (Mica, tema claro/oscuro); panel de diagnóstico de red gaming; aviso de frecuencia de refresco + HDR con confirmación temporizada; página de **Historial de cambios** y **detección de deriva**; 8 optimizaciones nuevas; estado de seguridad honesto; instalador autónomo.

</details>

<details>
<summary>3.0.0 y anteriores</summary>

- **3.0.0** — Identificación de hardware y gestor de Drivers; catálogo casi duplicado (86 → 166); módulo avanzado Seguridad ↔ Rendimiento; UI totalmente responsive.
- **2.0.0** — Panel mucho más completo; monitor de tráfico de red e inspector de conexiones por proceso; Apps & Debloat, Limpieza e Inicio rediseñados.

</details>

---

## ♻️ Reversibilidad y seguridad

Las optimizaciones pasan por un motor reversible: `ITweak → ISystemChange → diario persistente`. Cada cambio registra el valor previo antes de aplicarse, así puede revertirse después —incluso entre reinicios—. Los cambios de registro restauran el valor exacto anterior; los de comando/directiva restauran los valores por defecto de Windows. Los lotes pueden crear un **punto de restauración de Windows** antes, e importar un perfil siempre lo hace. **No hay "limpiador" de registro**, y el catálogo de optimizaciones no toca Microsoft Defender, BitLocker ni los servicios de Windows Update — la **Sesión de juego** pausa Windows Update solo mientras juegas, registrado en el diario y restaurado al terminar.

---

## ⚠️ Aviso

Esta herramienta modifica ajustes del sistema. Aunque todo cambio es reversible, algunas optimizaciones —en especial las del módulo **Seguridad ↔ Rendimiento**— reducen protecciones o afectan a la estabilidad y están pensadas para equipos personales y de confianza. Úsala bajo tu responsabilidad y crea un punto de restauración antes de aplicar lotes grandes.

---

## 📄 Licencia

Publicado bajo la **licencia MIT** — ver [LICENSE](LICENSE).

---

## 👤 Autor

**derzslows** — [@derzslows](https://github.com/derzslows)

<div align="center">

⭐ *Si este proyecto te resulta útil, ¡considera dejar una estrella!*

Hecho con ❤️ para gamers y usuarios avanzados de Windows.

</div>
